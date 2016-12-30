## Styling Greatness 

Intuitive styling of maps is of key importance to MapStory's success. We need to match the baseline of what others do through the web, and push the limits. CartoDB and MapBox are the ones really innovating with this. The cartodb approach is probably 
most apt for MapStory - an intuitive GUI to create basic styles and generate some more 
complex ones (intensity, quantiles). And those are always reflected in CSS, which one can 
always edit directly. 

Ideally we also standardize CSS for maps, between CartoCSS and GeoServer's CSS stuff.

## Requirements/Specs
In 2017 the main goal for styling is to address the "clutter" that will emerge with mapstories that have several layers, large amounts of features, and several chapters. Priorities include:

- [ ] Enable a "clustering" method that lets features be grouped together at certain zoom levels and then "broken up" into distict features at closer zooms. 
- [ ] Enable heat map styling
- [ ] Let a user "pick" from a drop-down of publically saved styles on a layer, similar to the way they can pick from a drop-down for basemaps now.




