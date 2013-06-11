## Lat/long maps instead of Web Mercator 

The web mercator projection is overused, distorts data, and does not actually fit the aspect ratios 
of most computers well. Let's serve up MapStory in lat/long (4326).

### Notes

Most all the pieces are there in the core software to support this. Indeed it could be cool to offer
several projections for MapStory users. In particular thinking (ant)arctic projections, like
http://mapstory.org/maps/594/ 

The big work on this item though is to provide base layers in 4326. All major mapping providers
serve in web mercator. At the very least we need to serve up an OpenStreetMap layer and a
satellite layer. Ideally a few styles of OSM. These also need to be reliable, likely a cluster
of servers and really good caching.
