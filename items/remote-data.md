## User Story

As a user I want the option to create StoryLayers out of remote data, instead of having all data be uploaded to MapStory.

## Requirements/Specs

Things like WMS, GeoRSS, KML. Some of these will likely be 'live', like USGS earthquake maps, where we 
want them to stay up to date with latest. Probably should start with WMS. GeoNode has had some work done towards this. Hopefully that completes and we can build on it. Handling things in GeoNode/Django is probably the right way to go, so we
can get at all the normal StoryLayer features. Like I think for remote data we still want the 
ability to comment on it, see what stories it's used in, etc.

Ideally we would also figure out some nice caching mechanisms for it. And indeed for some streams
we may want to maintain the historical database, since they are not really guaranteed to do that.
So MapStory would be building up the time series history from the steam.

WMS is the most straightforward, and easiest with existing GeoTools/GeoServer code. But would be
good to do RSS and the like. Should ideally code it as GeoServer datastores, and have it handle
all the caching and updates.

Another one along these lines would be a remote GeoGit datastore. Be able to update from there. Then
we can have people collaborating on data in other locations, but still have MapStory be an interface
for some collaboration, and for building up the stories from the layer.

Would be good to investigate the GeoTools level, and perhaps make an abstraction layer for any type
of remote data.

## Issues

## People
