##Storytelling refresh 

As we approach the baseline of needed functionality it is time to refresh a number of our older components.
We've learned a ton as we've had actual users, so we should do some deeper research on this and have it
inform a new round of improvements based on real, iterative feedback. 

To do this properly we also need to redo our core storyteller infrastructure. We are currently based on OpenLayers
2, and Ext.js 3. At the very least these need to be upgraded. But this is also an opportunity to explore new
toolkits and ways of doing things. 

### Requirements

The biggest requirement is to retain as much of the existing functionality for styling, annotations, 
timeline configuration and editing. We may not need a layer tree per se, but we do need a way to display 
more than one layer on the map.

It is worth examining if we need to do all the functionality on a single javascript application, or if there
is some logical split in components that would let us migrate each more slowly. One that potentially jumps out
is doing editing (with versioning eventually) in one app, and styling and annotations in another. 

We can probably get away with 'less' in the styling, as long as it is intuitive. We can probably point
people at qgis for more advanced styling, but should let people do some basics. 

### Tech thoughts / plan

We should strategize on what our end goal for javascript frameworks is. What we want to avoid is a big
mix of frameworks that aren't thought out. It could make sense to have a couple smaller frameworks, where we 
are clear on what each offers and how we use it. But we should probably avoid doing two or more 'big' frameworks.

### Wireframes

Should be sure to also take into account [guided storytelling] (guided-stories.md), as that will be a key 
feature.
