## Usoer Story

As a user visting MapStory.org, I should be able to discover StoryLayers and MapStories based on time spans and geographic locations that interest me

## Requirements/spec

In retro.mapstory.org temporal and geographic search were available. The implementation for Time required the user to manually enter a Start Time and End Time, and layers and stories that had time spans within the range were shared in the search results. In the new MapStory build, this is no longer feasible since MapStories may have multiple chapters and, thus, multiple timelines. StoryLayers will still have a single timeline with a start and end, though. The ideal solution would be if the search could generate and read an earliest date and latest date for every StoryLayer and MapStory. Maybe instead of manually entering a time into a search box, the user can interact with a timeline on which they could draw a timespan that they are interested in filtering content for. Even better would be a visual that showed the user the densities of StoryLayers and MapStories avaialble across a timeline (something like the activity heat map on user profiles in Github).

The implementation for Geographic Search on Retro was a bounding box. The user could draw a box on a map, and layers and stories that fit within the coordinates of the box appeared in the search results. Again, this is made more difficult by the advent of multi-chapter mapstories. Drawing a bounding box on a map still seems like a cool way to search for layers and stories geographically. Even cooler would be a heat map that shows the density of layers and stories available in different locations.

A big leap forward for MapStory search would also be the ability to search at a feature level...rather than just layers and stories. The advent of the Gazetteer will generate linkages between individual features, also opening up possibilities for feature-level search.

### People

### User and Design Stories

