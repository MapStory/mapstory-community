## Developer tab

Provide a way for developers to access the service endpoints for MapStory. We do good open standards and
open data API's, and we should make that obvious

### Requirements/spec

The minimum requirement here is to display the OGC web services of the map, like in:

![gp](geoportal-ogc.png "geoportal screenshot")

We can put this in a tab to along with 'share', 'info', etc. I suppose it would list a filtered capabilities
endpoint for each layer, or we'd figure out on the server side how to group the layers in a map in one
capabilities document.

Ideally we go further though. It could not just display the capabilities end points, but be a bit
of self-documenting snippets for that layer, showing how to use it on openlayers, google maps, and
with demo requests. Could have it be a bit self introspecting so each demo request is a valid command 
they could use right then. So the tab would be a bunch of generated resources that subtly teach the
user about OGC requests and the like. And for a developer who doesn't know anything about geo it
is just some nice API's that they can figure out, with a working example right there, and hopefully 
links to more resources. Some ideas for the things to document:

* Static image at a time slice (use a WMS reflector request, then they can play and learn about WMS)
* Dynamic map in openlayers and/or GeoExplorer, ideally working with time animation properly.
* Google map at a time slice, show the exact javascript to use with gmaps api, at a valid time slice.
* Possibly KML - though it'd be good to get time working automatically in GeoServer. Should be able to, all the plumbing is there, just not connected.
* WFS Query, likely best to do a couple to get across the power. With both geojson and with xml. And CQL for filtering, make it simpler
* Desktop GIS, like described above with capabilities end point. It is less 'developer' so maybe call the tab something else or put this in another tab.
* Tile access, just some sample tile requests, to TMS or XYZ tiles


### Tech plan/notes

May need to do some GeoServer WPS calls and possibly make some processes to get sample values.

### Wireframes


### People
Mostly a django person, potentially some geoserver person.


### Issues

