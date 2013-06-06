## Introduction

This document contains the current state of the MapStory roadmap. It will be dynamic as progress
is made and priorities shift as we learn more from users. 

### Immediate (within 4 weeks)

**[Annotations Improvements] (items/annotations.md)** - Bulk upload of annotations and a better editor. (Ivan)

**[Raster and uploader improvements] (items/raster.md)** - Iterative improvements for raster handling and 
uploading of data. (Ian)

**[Buttonology] (items/buttonology.md)** - Moving of buttons and slimming of panels for more map real estate. (Bart)

**[Organization pages] (items/org-pages.md)** - Pages for organizations to feature links and work in MapStory. (Done)

**[User support and iterative improvements] (items/user-support.md)** - Constantly improve MapStory based on feedback
from users.

### Short (1 month - 3 months)

**[Community Infrastructure] (items/community-infra.md)** - Better tools and structures for supporting the community, 
and to help the community support itself.

**[New Uploader] (items/uploader.md)** - New infrastructure for more robust handling, with client side validation and 
being able to add a raster to an existing storylayer.

**[Search improvements] (items/search-new.md)** - Search in the map that feels/works more like the site's search. 
Hopefully with some nice map-relevant improvements.

**[New Time Control Investigation] (items/time-new.md)** - First investigation of a new time control that is more intuitive and
responsive. Start with just the 'map' pages, not the full composer, just focused on playback. Depends on incorporating
OpenLayers 3.

**[Scalability improvements] (items/scalability.md)** - Put a cluster of GeoServers behind MapStory, and upgrade to 
Cloudfront caching.

**[OAuth integration with warper and wiki] (items/oauth.md)** - Enable MapStory login to work on 
http://warper.mapstory.org and http://wiki.mapstory.org

**[Versioning Prototype] (items/versioning-proto.md)** - Deployment of GeoGit with GeoNode to allow users to edit select
MapStory layers in a sandbox area on tools.mapstory.org

### Medium (3 month - 9 month)

**[Admin control over 'resources for', 'sections', and 'topics' pages] (items/custom-pages.md)** - The same type of links and media ribbon
in organization pages should be customizable from the 'resources', 'sections' and 'topics' pages.

**[Improve storytellers/profile pages] (items/storytellers.md)** - We should enable links and media ribbon options for users.
And also should redo the whole profile/storyteller editing flow, as it's confusing.

**[Embed on more platforms] (items/embed.md)** - Get the tech and whitelists in place so MapStory embeds can go on
more platforms.

**[Warper integration] (items/warper.md)** - A more seamless workflow to upload scanned map and warp it and add to a StoryLayer.

**[Iconcommons and better mapstory icons] (items/iconcommons.md)** - Create a sharing site for icons, for anyone to post 
open icons. And hook it in to the MapStory platform, so users can select from a wider variety of icons.

**[Developer Tab] (items/developer-tab.md)** - Add a section of the map/layer pages that lets developers know how
they can programmatically access the map and its data, like with openlayers, google maps, wms, wfs, etc.

**[Social Login] (items/social-login.md)** - Be able to login to mapstory with facebook and google, and grab the relevant 
picture, name and email.

**[CSW + permissioning infrastructure (GN 2.0 upgrade)] (items/geonode2.md)** - Incorporate pycsw and the richer
permissioning infrastructure from GeoNode 2.0, once it gets stable.

**[New Time Control Experimentation and Implementation] (items/time-new.md)** - Continue on with investigations and
move towards experimentation and implementation

**[Storytelling refresh] (items/composer-new.md)** - Consider new technologies and new approaches for the story telling 
functionality in map composer functionality (styling, annotations and editing). Possibly split up 
functionality for easier migration.

**[Location Guided MapStories (XYT frames)] (items/guided-stories.md)** - Add the ability for the story teller to 
guide the user, with the map updating zoom level and location for their narrative.

**[Messaging between users] (items/messaging.md)** - Users should be able to send feedback and messages to one another
through the mapstory platform, without having to reveal their email addresses.

### Long Term (9 months to 18 months - funding dependent)

TODO: bring in any old designs from Steven and stuff on the wiki.

Great styling

Table joining

Change to 4326

Audio in mapstories

Internationalization

Collaborative metadata editing, better permissioning

4D

Mobile

Integrated Versioned Editing

Data tools at tools.mapstory.org

### Ideas (catch all)

Integrated Wiki
 - lets us get activity feeds. https://github.com/benjaoming/django-wiki#readme looks interesting

Integrated Map Collaboration tools
 - chat
 - wiki
 - issue tracker
 
Find near, at feature level, in space and time.

Live data streams

Longitudinal Gazetteer

Social network mapping

Analysis and web processing

Animated Sharing - video and animated gif outpus


### Completed

Items that have been fully deployed to production

(non yet, just started this roadmap)

