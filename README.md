mapstory-roadmap
================

This repository is dedicated to maintaining an evolving Product Vision and Roadmap for MapStory. This Roadmap is focused on the purpose and features associated with the platform. 

If you're interested in Developer docs associated with MapStory.org, you should see the Wiki in the main [MapStory repo] (https://github.com/MapStory/mapstory/wiki). 

See [roadmap.md](roadmap.md) for the main Roadmap document.

The [items/](items/) folder contains the actual details on the tasks for the roadmap. 
To read those it is best to just follow the links from the roadmap, as the items will
then be ordered properly.

### Adding to the roadmap

To create a new roadmap item add an entry to `roadmap.md` following the same structure as the 
other links, and create a new page under `items/`. You can use this [template](items/template.md)
to copy and paste in to your new item to follow the general structure of other items.

But there are no hard rules for items and the headings, except to make them useful for project
management and developers. 

### Maintaining the roadmap

The Roadmap should be updated by Product Owners at least once per month.

##### Immediate Term

Any item listed in [immediate term](https://github.com/MapStory/mapstory-roadmap/blob/master/roadmap.md#immediate-within-4-weeks) 
should have an 'owner'- a developer who is primarily responsible for its delivery. All issues generated as part of an item should have a common label (i.e. "4D") and should have a StoryPoint prediction for level-of-effort (we use the Fibonacci sequence to predict effort). The Designer, in coordination with the developer owner and Product Owners, should make decisions on wireframes as soon as possible.

##### Medium Term

Medium term items should have a real commitment to them, be it funding secured or a volunteer developer
agreed to do all the work. They should have the requirements detailed out to sufficient degree to begin
wireframes or technology plan. Medium term items should also be in accomplishable chunks. If it is a huge
scope in long term than just the first couple milestones should get in to medium term.

##### Long Term and Ideas

Long term should be at least somewhat fleshed out. Ideas can just be place holders to remind to fill out the requirements. Long term should also ideally be at least in a funding pitch - the idea to secure funding for it relatively soon.

##### Completed

Completed items should be fully deployed to production. If all the original goals were not accomplished than
another roadmap item can be created to lay out what to do next. But some work towards the end should be 
deployed to production on mapstory.org before marking something as completed.
