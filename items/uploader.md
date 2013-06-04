## New Uploader with raster improvements

We've got raster basics on production now, but it needs much testing and improvement. We should 
continue to support users on the raster issues that arise. We also have a new importer in GeoServer, 
but we still need to write the new uploader. 

### Requirements

The new uploader should needs to support the addition of a raster to a mosiac, and should also support
much better client side validation. It will need lots of testing to ensure it handles all the old
uploader did, but the new one should provide a foundation to build up a much more robust solution.

### Tech plan
To do this we need to upgrade to GeoServer 2.3.x. This involves porting time components to GeoTools 9.x, and
getting the mapstory security module working properly. And then testing to make sure there are no regressions.

### People
Ian, with Justin helping out on the GeoServer side.

### Issues

