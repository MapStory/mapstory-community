## Scalability

MapStory should be able to scale to any user demand. Ideally caching at most every level and auto deploying 
more servers as resources get maxed out.

### Requirements

There are two major goals of this round of work. 

The first is to enable a cluster of GeoServers behind MapStory. These should stay in sync with one another,
as MapStory is a highly dynamic site. Should have at least two servers in a high availability load-balanced
cluster. And it'd be ideal if we figure out Amazon's auto-scaling possibilities to fire up synced servers
on demand with increased load. This item will be a lot of work to get right, because it needs extensive testing
and a new testing environment with lots of QA.

The second is to enable CloudFront caching. This item actually has most all the tech infrastructure in place,
with a number of improvements that have come in. It needs to be enabled and tested. The backend caching also
does not appear to be consistent, so that also needs to be figured out.

### Tech plan
The very first step is to get to a three tier architecture for MapStory, so we can potentially cluster each tier, 
see [#725] (https://github.com/MapStory/mapstory/issues/725). 

The next step is to upgrade to GeoServer 2.3.0. dbconfig and other thing.

create a testing cluster
migrate all of mapstory data over
test and qa, add new data sets for testing - focused on making sure everything works as it did
try out autoscaling
do scalability tests, focused on big loads and seeing it hold up
deploy.

For CloudFront there are some gotchas to get it working perfectly. From Ian:

Maps won't work at the moment - see #733. The pages won't even render if geoserver is down. This is because during the 
template render, there are REST calls that will cause the whole page to fail. GeoNode2 tries to handle this by 
caching/duplicating all of geoserver's information in it's own models but this approach is still incomplete as 
the page will render but the map will be broken (with no notice to the user) and adds much complexity. 
As a fix for #733, I'd like to resolve the resources up front (before the render) and take appropriate action 
(put notice on the page and avoid pink tiles) if geoserver is down.
