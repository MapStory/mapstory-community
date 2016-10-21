## Introduction

This document states the active Epics for MapStory.org, beginning from November 1, 2016. User Stories related to these Epics are tracked for progress with issue tickets. This Roadmap will be dynamic as progress is made and priorities shift as we learn more from users.

### Immediate (within 2 months - December 31, 2016)

**[Scalability improvements] (items/scalability.md)** - As a user, I need confidence that MapStory.org has test coverage and a DevOps pipeline that will ensure the platform does not regress and can support wide scale public use.

**[Login and account creation] (items/oauth.md)** - Enable MapStory login to work on http://warper.mapstory.org and http://wiki.mapstory.org

**[Styling](items/styling.md)** - As a user, I need to be able to style layers I use in my story so that my story conveys meaning in the way I envision.

**[Mass editing of change over time] (items/versioning-proto.md)** - As a user, I need to be able participate in community versioned editing of the spatial, temporal and attribute information on features in any StoryLayer that is open for community editing.

**[Scale Versioned Editing](items/integrated-versioning.md)** - Following on our [versioning prototype](items/versioning-proto.md)
work we want to expand that so every StoryLayer is automatically versioned and collaborative.

**[Story composing] (items/composer-new.md)** - As a user, I need to be able to compose and publish my mapstory, and have it playback for viewers as I expected it to behave when I composed it.

**[Legend Enhancements] (items/legend.md)** - As a user, I need to be able to customize my legend in composer and have it appear the way I set it on a published story.

**[Storyteller Profiles] (items/storytellers.md)** - As a user, I need to be able to manage the actions I take on the platform, and the way that my actions and personal identity are presented to the public.

**[Playback settings] (items/playback-settings.md)** - Relating to the time control is some good design work
from the past focusing in on the settings for playback.

### Medium (Within 5 months - March 30th, 2017)

**[Organization pages] (items/org-pages.md)** - As a user, I need to manage an Organization Page, which enables me to pool all the storytellers, storylayers and mapstories that represent a group.

**[Time Controls] (items/time-new.md)** - As a user, I need time controls on layers and stories that are intuitive, fast and honor the time information in my layers.

**[StoryPin Improvements] (items/annotations2.md)** - As a user, I need to be able to quickly and intuitively create StoryPin annotations that help me explain activity on the map that is not part of the data in my storylayers.

**[Warper integration] (items/warper.md)** - As a user, I need a map warper that is integrated with the mapstory importer.

**[Mobile](items/mobile.md)** - As a user, I need to be able to conduct operations on the platform that make sense given the device I am using (desktop, tablet, mobile).

**[Statistic upload and join existing geometries](items/table-join.md)** - As a user, I want to upload statistics and join that to sets of geometries maintained on MapStory.

**[Longitudinal Gazetteer](items/longitudinal-gazetteer.md)** - As a user, I want to link Place Names across data layers to support enhanced search, editing and storytelling

### Long Term (6 months to 12 months - funding dependent)

**[Developer Tab] (items/developer-tab.md)** - Add a section of the map/layer pages that lets developers know how
they can programmatically access the map and its data, like with openlayers, google maps, wms, wfs, etc.

**[Embed on more platforms] (items/embed.md)** - Get the tech and whitelists in place so MapStory embeds can go on
more platforms.

**[CSW + permissioning infrastructure (GN 2.0 upgrade)] (items/geonode2.md)** - Incorporate pycsw and the richer
permissioning infrastructure from GeoNode 2.0, once it gets stable.

**[Lat/long maps instead of Web Mercator] (items/latlong-maps.md)** - The web mercator projection is overused, distorts data, and
does not actually fit the aspect ratios of most computers well. As a user, I want to serve up MapStory in lat/long (4326).

**[Internationalization](items/i18n.md)** - MapStory should be available to people regardless of what language they
speak. As a user, I want to make sure the site is all internationalized and start a crowd sourced localization effort.

**[3D MapStories](items/3d.md)** - There are several cool WebGL toolkits that may let us view MapStories not just in
2D but in 3D, over time. As a user, I want to incorporate these.

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

**[Social network mapping](items/social-network-maps.md)** - Lots of data is being produced about relationships over
geography and time. MapStory should be able to render these and let users make stories with the data.

**[Analysis and web processing](items/analysis.md)** - Provide ways to enable more advanced analysis of MapStory data, 
creating new stories as a result of analysis of other layers. May make sense to go under tools.mapstory.org

**[Animated Sharing](items/animated-sharing.md)** - When we share MapStories on social networks they tend to be a 
single screenshot. We should investigate animated gif and video outputs for MapStory, as that can make social
sharing communicate the motion inherent in the stories.

**[Automate contributions from 3rd parties with widgets](items/widgets.md)** - We should explore ways to plant a simple
'Add to MapStory' button on external sites that focus on spatial-temporal data collection. An example partner interested
in something like this is historyit.com

**[Define algorithms and values behind peer review tools](items/peer-review.md)** - We need to futher define the user experience
of our peer review tools (star rating and flag error). Also explore other features for curating quality and signaling rigor.

### Completed

Items that have been fully deployed to production

**[Audio in mapstories] (items/audio.md)** - Many online proto-MapStories support audio in various ways. We should 
give storytellers options for incorporating audio in to their stories.

**[Better support for icons in styling] (items/icon-styling.md)** - Build the facility for our styler tools to refer
to a remote set of icons. And make compatible with [Iconcommons](items/iconcommons.md).

**[Location Guided MapStories (XYT frames)] (items/guided-stories.md)** - Add the ability for the story teller to 
guide the user, with the map updating zoom level and location for their narrative.

**[Iconcommons and better mapstory icons] (items/iconcommons.md)** - Create a sharing site for icons, for anyone to post 
open icons. 

**[Messaging between users] (items/messaging.md)** - Users should be able to send feedback and messages to one another
through the mapstory platform, without having to reveal their email addresses.

**[Buttonology] (items/buttonology.md)** - Moving of buttons and slimming of panels for more map real estate. 

**[Raster and uploader improvements] (items/raster.md)** - Iterative improvements for raster handling and 
uploading of data.

**[Search improvements] (items/search-new.md)** - Search in the map that feels/works more like the site's search. 
Hopefully with some nice map-relevant improvements.

**[Annotations improvements] (items/annotations.md)**- Bulk upload of annotations and a better editor

**[Community Infrastructure] (items/community-infra.md)** Better tools for supporting the community, and to help the community support itself.

**[New Uploader] (items/uploader.md)** - New infrastructure for more robust handling, with client side validation and 
being able to add a raster to an existing storylayer. (Ian)

**[Social Login] (items/social-login.md)** - Be able to login to mapstory with facebook and google, and grab the relevant 
picture, name and email. (Marc)

**[Annotations Hotfixes] (items/annotations.md)** Basic tweaks to annotations improvements made in last milestone based on user feedback. (Bart)

**[User support and iterative improvements] (items/user-support.md)** - Constantly improve MapStory based on feedback
from users. 
