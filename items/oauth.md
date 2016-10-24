## MapStory.org integration with wiki and warper

MapStory has a bigger universe than just the site. There is also the wiki and the warper. And more tools will
likely come in the future (like osqa and geogit). One should be able to login to mapstory.org and not have 
to login again at the warper or the wiki. Current thinking is this would be with OAuth, but other options
are fine as well.

### Critical question

* How to represent real names vs unique identifier

### Requirements

* Should be possible to login to MapStory and not have to create an account on the warper or on the wiki.
* Should work with [Social Login] (social-login.md) stuff.
* Document how other services that may be associated with MapStory can share logins

### Tech Plan

The general idea is to use 'OAuth' to do this. To have MapStory be an OAuth provider, that the others can 
tap in to. This probably needs some more research though.

On the OpenGeo end we should do the task of the wiki and mapstory.org. We also have the contractors who 
set up the warper, who can configure it on their end. Their version of rails only supports OAuth 1.0, 
so that's what we should target. Though if that's a pain we could probably get them to upgrade their
rails version.

They also have an idea to just inspect the cookies that MapStory creates and use those directly. We
might investigate this as an option for other integrations as well.

### Issues
https://github.com/MapStory/mapstory/issues/736

https://github.com/MapStory/mapstory/issues/737

https://github.com/MapStory/mapstory/issues/727
