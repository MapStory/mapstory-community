## Raster improvement

The raster work just landed on production, so needs more iterations of user testing to get solid.

### User Stories

As a user, I need to be able to import my data in more file types, like KML, Raster, GeoJSON

As a user, I need clearer feedback on why my imports fail, and exactly how my data should be organized in order to succeed with imports

As a user, I need to be able to upload statistics for common geometries (like countries, or US states) and apply these stats to geometries, rather than having to upload the geometries again every time.

As a user, I need to georeference a single map/image or sequence of maps/images (raster) and easily import them as a StoryLayer.

As a user, I need to import data that extends to geologic scale.

As a user, I need to import data that lacks time information and then be able to add time information to features as its learned, with versioned editing.

As a user, I need to be able to make edits to cells that are causing my data to fail without having to re-upload an entire file. 

As a user, I need to be able to add metadata and publishing preferences right in the importer modal, rather than going to a separate metadata modal. 

As a user, I would like to upload data that is in different projection formats (requirements TBD)


### Requirements

To be reported by users. This likely will include other user support, so will take a decent bit of 
time, but should get to more solid raster backend. But it should help flesh out other site improvements
related to uploading and beyond.

Some client side improvements will also help, to inform users earlier on when something is wrong.

### People
Ian, and testers

### Issues
* https://github.com/MapStory/mapstory/issues/700
* https://github.com/MapStory/mapstory/issues/723
