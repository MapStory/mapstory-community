## Warper integration

We have warper.mapstory.org, but it's a separate tool. We would like a more seamless workflow to 
upload scanned map and warp it and add to a StoryLayer.

### Requirements/spec

The overall requirement is to create a fairly seamless experience for people to upload unscanned maps, warp
them to be georeferenced, and add to their mapstories. Ideally not even feeling like there's a big difference
between warper.mapstory.org and mapstory.org proper. 

We likely won't hit the goal of being seamless in this first pass. But we should make it so they don't have
to upload the scanned map to the warper, download it, zip it together with others, than upload to mapstory.org.
At least some way to transfer between the two servers, and ideally a nice pass off between the two. 

Should get users working with both tools and see what they suggest.

### Tech plan/notes

Research needed. May want to also investigate some batch processing / separate server for warping and tiling,
tell the users things are 'in process' before trying to serve them up right away.

### Wireframes
(optional, remove if not relevant)

### People

### Issues
