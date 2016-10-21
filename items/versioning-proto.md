## Versioning Prototype

MapStory aims to have full versioning of all StoryLayers. The basis of this will be http://geogit.org 
Since it still needs lots of development we will start by deploying at tools.geonode.org a special GeoNode that has a few
select MapStory layers under versioning. This will let the MapStory community give feedback and use
the new technology. Once that is solid we will figure out how to incorporate the technology in to all
of MapStory.

### User Stories

As a user, I need to add, edit or delete features on any layer that has settings open for community editing.

As a user, I need to be able to scrum the timeline back and forth on a layer rapidly, so that I can gain a quick sense of the data included in that layer

As a user, I need to be able to edit metadata of other users’ StoryLayers, so I can make it more complete and accurate.

As a user, I need to be able to add new attributes to StoryLayers that I own after the point of upload. 

### Requirements

Most all this work is being done by the ROGUE team, so they are driving many of the requirements.

From a MapStory perspective we just want a GeoNode that is stood up in a location we can point users
at. It should have versioning enabled, for at least a couple prime MapStory layers, like the 
Histoire Mondiale, or some MapStory Local layers. 

After that is set up a key step will be to make it so that improvements there are reflected on the MapStory site.

### Tech plan/thoughts

* Should set up a new GeoNode for the versioning. A complete separate interface.
* Would be good to get login working across both GeoNodes, like the work in the [Login roadmap item] (oauth.md)
* They should talk to the same database, so that changes in the versioning interface get reflected
in the main MapStory story.
* To work well will need a way to notify GeoWebCache of the changes made.

### Progress

See: http://geoserver.rogue.lmnsolutions.com/ for the work in progress.
Time layers at http://geoserver.rogue.lmnsolutions.com/maps/35/view and http://geoserver.rogue.lmnsolutions.com/maps/38/view
