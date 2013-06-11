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
open icons. 

**[Better support for icons in styling] (items/icon-styling.md)** - Build the facility for our styler tools to refer
to a remote set of icons. And make compatible with [Iconcommons](items/iconcommons.md).

**[Developer Tab] (items/developer-tab.md)** - Add a section of the map/layer pages that lets developers know how
they can programmatically access the map and its data, like with openlayers, google maps, wms, wfs, etc.

**[Social Login] (items/social-login.md)** - Be able to login to mapstory with facebook and google, and grab the relevant 
picture, name and email.

**[CSW + permissioning infrastructure (GN 2.0 upgrade)] (items/geonode2.md)** - Incorporate pycsw and the richer
permissioning infrastructure from GeoNode 2.0, once it gets stable.

**[New Time Control Experimentation and Implementation] (items/time-new.md)** - Continue on with investigations and
move towards experimentation and implementation. Be sure to incorporate [playback settings](items/playback-settings.md)
work.

**[Storytelling refresh] (items/composer-new.md)** - Consider new technologies and new approaches for the story telling 
functionality in map composer functionality (styling, annotations and editing). Possibly split up 
functionality for easier migration.

**[Location Guided MapStories (XYT frames)] (items/guided-stories.md)** - Add the ability for the story teller to 
guide the user, with the map updating zoom level and location for their narrative.

**[Messaging between users] (items/messaging.md)** - Users should be able to send feedback and messages to one another
through the mapstory platform, without having to reveal their email addresses.

**[Legend Enhancements] (items/legend.md)** - Rework the legend to not take up so much space and be more intuitive.

**[Annotations Improvements Part 2] (items/annotations2.md)** - Rework annotations to learn from users and work
on smaller maps well.

### Long Term (9 months to 18 months - funding dependent)

**[Styling Greatness](items/styling.md)** - Intuitive styling of maps is of key importance to MapStory's success. We 
need to match the baseline of what others do through the web, and push the limits.

**[Statistic upload and join existing geometries](items/table-join.md)** - We replicate lots of data needlessly, making
users upload their own geometries when all they want to do is style based on some new statistics. We should be able
to let them just upload statistics and join that to sets of geometries maintained on MapStory.

**[Lat/long maps instead of Web Mercator] (items/latlong-maps.md)** - The web mercator projection is overused, distorts data, and
does not actually fit the aspect ratios of most computers well. Let's serve up MapStory in lat/long (4326).

**[Audio in mapstories] (items/audio.md)** - Many online proto-MapStories support audio in various ways. We should 
give storytellers options for incorporating audio in to their stories.

**[Internationalization](items/i18n.md)** - MapStory should be available to people regardless of what language they
speak. We should make sure the site is all internationalized and start a crowd sourced localization effort.

**[Better permissioning](items/permissioning.md)** - Right now MapStories and StoryLayers are not very collaborative,
you can't invite someone else to edit data or a story with you. Should bring in better permissioning to enable that,
and to also investigate techniques to get high quality metadata.

**[3D MapStories](items/3d.md)** - There are several cool WebGL toolkits that may let us view MapStories not just in
2D but in 3D, over time. We should incorporate these.

**[Mobile](items/mobile.md)** - Mobile devices are the platform of the future. We need to determine what the MapStory
experience on a mobile device should be.

**[Integrated Versioned Editing](items/integrated-versioning.md)** - Following on our [versioning prototype](items/versioning-proto.md)
work we want to expand that so every StoryLayer is automatically versioned and collaborative.


### Ideas (catch all)

**[Data tools at tools.mapstory.org](items/tools.md)** - Right now people have to do lots of data cleaning
on their desktops. In time we should provide a full suite of data transformation and cleaning tools at 
tools.mapstory.org

**[Integrated Wiki](items/integrated-wiki.md)** - Right now we use mediawiki. Would be cool to find a way so edits
in the wiki are integrated with activity feeds on the MapStory site.

**[Integrated Map Collaboration tools](items/integrated-collab.md)** - People will likely want more tools to 
work on MapStory with one another. Should investigate providing things like chat, wiki, issue trackers, etc.
for their layers and maps.
 
**[Find near in space and time](items/find-near.md)** - At a feature level people should be able to find other
data near where they are in the map, in both space and time. So search by feature, not just bounding box of data.

**[Remote data streams](items/remote-data.md)** - Instead of requiring all data to be uploaded to MapStory it
would be good to let users add remote data. Things like WMS, GeoRSS, KML. Some of these will likely be 'live', like
USGS earthquake maps, where we want them to stay up to date with latest.

**[Longitudinal Gazetteer](items/longitudinal-gazetteer.md)** - Provide a gazetteer that is accurate with names that
evolve over time.

**[Social network mapping](items/social-network-maps.md)** - Lots of data is being produced about relationships over
geography and time. MapStory should be able to render these and let users make stories with the data.

**[Analysis and web processing](items/analysis.md)** - Provide ways to enable more advanced analysis of MapStory data, 
creating new stories as a result of analysis of other layers. May make sense to go under tools.mapstory.org

**[Animated Sharing](items/animated-sharing.md)** - When we share MapStories on social networks they tend to be a 
single screenshot. We should investigate animated gif and video outputs for MapStory, as that can make social
sharing communicate the motion inherent in the stories.


### Completed

Items that have been fully deployed to production

(non yet, just started this roadmap)

