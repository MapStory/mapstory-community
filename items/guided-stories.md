##Location Guided MapStories (XYT frames) 

Add the ability for the story teller to guide the user, with the map updating zoom level 
and location for their narrative.


### Requirements/spec

The core requirement is to create a user interface that lets a user specify at each frame of their map
playback where the 'camera' should be - what zoom level and what center point. This lets them 'guide' the
person watching the story to see the parts of the map that are most relevant to that time and the annotations
they put up to explain it.

Would be nice to allow people set things like 'fly to' for transition between points, as in the 'fly to' 
example in http://ol3js.org/ol3/master/examples/animation.html Could make it so people can select the
transition they want.

The other really nice big feature to at least think about in implementation is to use this for people
to tell stories with static data sets. The 'steps' in their story would just be zoom levels and center
points, along with potentially user set 'times' to stay on the story. So the time slider would not be
moving forward/back in time, but just along their narrative. Might be good to start this as a separate
story telling interface, since people will want to combine the two, but that will take lots of good
thinking on how to expose, to let people set timing of their narrative against a moving historical
time.

### Tech plan/notes

One idea is to store the center and zoom level in a special annotation.


### Wireframes
Main question to answer is what is the composition interface? How do people set the location for the
steps of their story? How does that jive with annotations and other playback options? 



### People
Steven to start, to make designs


### Issues

https://github.com/MapStory/mapstory/issues/187
