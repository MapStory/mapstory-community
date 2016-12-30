## User Story

The StoryFrame and StoryPin features in the mapstory composer do not support going back to the geologic time scale that we seek for importer. This means that the storyteller would not be able to match their pins and frames with their layers in this situation.

We need to reconfiguren the time support for thse features.

## Requirement/Spec

As part of this work, we may need to experiment with our timeline itself.
To make sure we don't lose functionality this list is an attempt to list what the new time slider should support.

 - variable speed (more than just 2x, but to do that it could combine frames)
 - prebuffering
 - aggressive time sliding - updating when moving slider
 - cumulative and normal playback.
 - advance one frame at a time
 - set 'desired time length' and have playback work backwards
 - prepares for different zoom levels and XYT frames
 - Allows for different 'pacing' variables (by decade, then by month for example)
 - Has a way to work with existing Map Composer. Could be a toolkit that integrates with ext.js/geoext, could do 
something half way, could keep old controls on composer and have new one work with it.

### Issues

### People

### Notes
Cartodb is planning to release a standard for a format that powers their torque time library. If it's any good
and reusable could be interesting to look in to implementing that in GeoServer. We could potentially then playback
from CartoDB maps.

One thing we should investigate is using Cesium's time slider directly. Like we could just make advanced
time sliding webgl only, use the czml output from geoserver (see https://github.com/AnalyticalGraphicsInc/geoserver/tree/czmlOutput)
and then have the client display that. They already did a demo showing ames data, which looks compelling:
http://dl.dropboxusercontent.com/u/30019282/cesium-mapstory.mp4

We could probably get away with webgl only for advanced time slider. Just need a way to degrade nicely, using
openlayers (could be 2.x if the time stuff is a pain, or 3.x if it's working well).
