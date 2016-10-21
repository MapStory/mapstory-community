## Improve storytellers/profile pages

We should enable links and media ribbon options for users. And also should redo the whole profile/storyteller 
editing flow, as it's confusing.

### User Stories

As a user, I need to be able control the order in which my published storylayers and mapstories appear on my public profile.

As a user, I need to be able to “own” and manage an Organization Page that is represented in the storyteller search and sits at a customized URL (i.e. mapstory.org/OrganizationName)

### Requirements/spec

First requirement is to enable links and media ribbon for users. 

The bigger thing is to rethink how users edit their profile and do all the other actions, and how that
fits with the display of their profile. Indeed even what the split between the 'storyteller page' and the
'profile page' and what that means. And then there's also the 'edit profile' page.

Would be ideal to have more in page javascript editing. The organization pages do some of this decently,
where if you are the owner then you get 'edit' buttons on everything that you can change. So are editing
the things just as you'd see them on display, not in some separate form.

### Tech plan/notes

Tech should hopefully be straightforward, mostly django pages. Could be nice to get some nicer
javascript touches, for in line editing of information.

### Wireframes


### People
Steven to start with some design thinking, then a django resource to implement.

### Issues
https://github.com/MapStory/mapstory/issues/461 is to enable links and media ribbon. It is mostly done, so
may get deployed. But the refresh that is the bulk of this is on:
https://github.com/MapStory/mapstory/issues/742

That should lead to a number of issues and we can unit them with a label.
