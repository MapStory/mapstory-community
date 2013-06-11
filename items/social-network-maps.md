## Social network mapping 

Lots of data is being produced about relationships over geography and time. MapStory should be 
able to render these and let users make stories with the data.

### Notes

The GeoTools renderer does not support this, and indeed it may require some fundamental rearchitecting
of the data structures. This type of data is most always done as a relationship between two points,
so to render this we need to render that relationship. Or else get the data to be exported in a way
that includes georeferenced lines. But I think the idea is we want to be able to import just the
points and their relationships, and have MapStory/GeoServer render the relationships, since it
will know more about the geospatial components than the exporting data tool.
