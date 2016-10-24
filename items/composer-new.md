##Storytelling refresh 

As we approach the baseline of needed functionality it is time to refresh a number of our older components.
We've learned a ton as we've had actual users, so we should do some deeper research on this and have it
inform a new round of improvements based on real, iterative feedback. 

To do this properly we also need to redo our core storyteller infrastructure. We are currently based on OpenLayers
2, and Ext.js 3. At the very least these need to be upgraded. But this is also an opportunity to explore new
toolkits and ways of doing things. 

### Critical Questions

Aspect ratio?

### User Stories

As a user, I need to be able to customize how the Get Feature Info appears for the features in my StoryLayers when I’m working in composer, and if a viewer of my story will be able to click on features to see Get Feature Info or not.

As a user, I need to be able to click on the Get Feature Info / Infobox on a feature of a published story in which the creator of that story has set it so I can click on features.

As a user, when I’m composing a story I need a better way to see all the elements I’ve added to my story - layers, boxes, pins (Table of Contents)

As a user, when composing a story I need to be able to click and drag StoryLayers to different chapters rather than having to add a StoryLayer again in the chapter

As a user, I need to have the zoom resolution on my published story appear as I set it when composing the story.

As a user, I want to be able to set the playback rate for my chapters.

As a user, I need to pick between a set of Templates that correspond with the type of ‘story’ I have in mind.

As a user, I need to add information to the Chapter Info content box that can be interactive with the map interface (i.e. charts, graphs).

As a user, I need to download a story in a print format that is coherent to use as a handout (i.e. pdf).

As a user, I need to show my features in a clustered view if there are a high number of them, to make viewing more graceful at different zoom levels.

As a user, I need to view stories with elevation data (4D - cesium)

As a user, I need to compose a story with other users also composing on that same story, at the same time

As a user, I need to have multiple users be assigned as “authors” of the same story, if they helped to work on it.


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
