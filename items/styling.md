## Styling Greatness 

Intuitive styling of maps is of key importance to MapStory's success. We need to match 
the baseline of what others do through the web, and push the limits.

### User Stories

As a user, I need to apply these basic styles to a layer in composer: simple, unique, graduated, choropleth, heatmap

As a user, I need to be able to save the style I apply in a draft story, and return to the draft and have the style still be there

As a user, I need to have my style persisted on a published story.

### Notes

CartoDB and MapBox are the ones really innovating with this. The cartodb approach is probably 
most apt for MapStory - an intuitive GUI to create basic styles and generate some more 
complex ones (intensity, quantiles). And those are always reflected in CSS, which one can 
always edit directly. 

May involve some fundamental redoing of our stuff, especially getting CSS working well. 

Ideally we also standardize CSS for maps, between CartoCSS and GeoServer's CSS stuff.
