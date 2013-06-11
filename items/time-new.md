### New Time Control

The current time slider does not work well. While it has been going iterative improvement the 
existing codebase is hard for our current developers to maintain, as we no longer have the original
author. It should be refactored to a nicer control, investigating new technologies like OpenLayers 3.0
and new javascript toolkits. 

### Goal

The first goal is 'investigation'. This is to design a more intuitive time control. And to come up with a 
plan to implement, in a way that lets us support existing users and bring in new technology while making
iterative improvements.

The second goal is a new time slider that works great. It should feel much more intuitive and perform
much better. We will likely limit this to just the 'maps' and 'layer' pages, keeping the map composer
mostly the same. 

### Plan

We should start with a full survey of the functionality we need the time control to fulfil. What people
are actually doing with maps now and what they want to do.

From there we should move to design, with real wireframes.

Meanwhile we can investigate new javascript toolkits and experiment with client side rendering.

Our first goal is the map and layer pages, doing advances there while keeping the map composer the same if possible.

We should not only investigate trying to meet all current map needs with the new technology. We should also
try to make a few super compelling maps, not constrained by handling every use case. From there we can figure
out the constraints for the new time slider. A limit on number of frames? Total number of points in geometries?
IE 10/Chrome/FF only? WebGL? We can hopefully build the new tech with constraints, and for mapstories/users that
don't meet those constraints we fall back on the older time playback, so we can always play something. 

As we investigate this plan should be fleshed out more.


### Requirements
 
To make sure we don't lose functionality this list is an attempt to list what the new time slider should support.

 - variable speed (more than just 2x, but to do that it could combine frames)
 - prebuffering
 - aggressive time sliding - updating when moving slider
 - cumulative and normal playback.
 - Has a way to work with existing Map Composer. Could be a toolkit that integrates with ext.js/geoext, could do 
something half way, could keep old controls on composer and have new one work with it.

### Issues
None yet

### People
Bart and Ivan, with support from Ian for server stuff.

### Notes
https://github.com/MapStory/mapstory/wiki/Proposed-Playback-Options has some interesting thoughts.

Cartodb is planning to release a standard for a format that powers their torque time library. If it's any good
and reusable could be interesting to look in to implementing that in GeoServer. We could potentially then playback
from CartoDB maps.

One thing we should investigate is using Cesium's time slider directly. Like we could just make advanced
time sliding webgl only, use the czml output from geoserver (see https://github.com/AnalyticalGraphicsInc/geoserver/tree/czmlOutput)
and then have the client display that. They already did a demo showing ames data, which looks compelling:
http://dl.dropboxusercontent.com/u/30019282/cesium-mapstory.mp4

We could probably get away with webgl only for advanced time slider. Just need a way to degrade nicely, using
openlayers (could be 2.x if the time stuff is a pain, or 3.x if it's working well).

See also [Playback Settings](playback-settings.md) item.
