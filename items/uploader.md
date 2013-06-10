## New Uploader with raster improvements

We've got raster basics on production now, but it needs much testing and improvement. We should 
continue to support users on the raster issues that arise. We also have a new importer in GeoServer, 
but we still need to write the new uploader. 

### Requirements

The new uploader should needs to support the addition of a raster to a mosiac, and should also support
much better client side validation. It will need lots of testing to ensure it handles all the old
uploader did, but the new one should provide a foundation to build up a much more robust solution.

A 'nice to have' would be to do a similar thing with vector data, let people 'append' a set of data to
an existing storylayer dataset. Should hopefully be similar UI, and our vector stores do already support
that.

### Tech plan
To do this we need to upgrade to GeoServer 2.3.x. This involves porting time components to GeoTools 9.x, and
getting the mapstory security module working properly. And then testing to make sure there are no regressions.

### Wireframes
Some design questions:

Where do people 'add' data to an existing StoryLayer? On the storylayer, like a tab there? In the uploader,
like a step that asks them if they want to create new or add to existing? Both?



### People
Ian, with Justin helping out on the GeoServer side.

### Issues

* https://github.com/MapStory/mapstory/issues/751
* https://github.com/MapStory/mapstory/issues/752
* https://github.com/MapStory/mapstory/issues/753
* https://github.com/MapStory/mapstory/issues/754
* https://github.com/MapStory/mapstory/issues/755
* https://github.com/MapStory/mapstory/issues/756
* https://github.com/MapStory/mapstory/issues/757
