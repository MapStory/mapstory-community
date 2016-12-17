## Product Vision

MapStory.org is the atlas of change that everyone can edit. It seeks to organize humanity's shared knowledge about how the world evolves geographically over time, and to make this knowledge easily accessible as an open educational resource. The platform is sustained by the nonprofit MapStory Foundation and dedicated volunteers, contracting partners and sponsors.

The project was originally started by Dr. Christopher Tucker who, as a graduate student at Columbia University, "dreamt of a platform that I could search spatially and temporally and find out what the preponderance of social scientists knew about what had been going on. And better yet, improve upon that knowledge through continuous editing." The goal was to provide a compliment to other open knowledge platforms, such as Wikipedia and OpenStreetMap, that focused on spatio-temporal change (or, in other words, historical geography).

This original sentiment still drives the MapStory.org product vision today, although prototyping has helped clarify the technical approach and target audience that form the project's implementation.

As we begin 2017, we understand MapStory.org to be for scholars, students and enthusiasts around seeking historical perspective on any topic that can be mapped over time - whether that topic is hyper local, such as the rise of a town hyper global, such as the movement of continents. The current MapStory.org platform brings three core technical components together that have never been combined before in order to provide users with a fundametally unique and comprehensive way to understand how our world evolves of time and space. First, it uses the open source GeoNode as a scalable spatial infrastructure for data. Second, it uses GeoGig as a version-editing tool so that all data in MapStory.org can be continuously improved over time. And third, it adds a mapstory "composer" that we built from scratch so users could go beyond mere data visualization to convey deeper narratives about why and how phenomena play out as they do.


## Project Status

The first version of the platform was dubbed a "public prototype in development" and launched in April, 2012. Leveraging the Open Geo software stack, it let a registered upload spatio-temporal datasets, generate unique styles for the data, and play the data over time and space. Users 

### Immediate (within 2 months - December 31, 2016)

**[Scalability improvements] (items/scalability.md)** - As a user, I need confidence that MapStory.org has test coverage and a DevOps pipeline that will ensure the platform does not regress and can support wide scale public use.

**[Login and account creation] (items/oauth.md)** - As a user, I need to enable MapStory login to work on mapstory.org, http://warper.mapstory.org and http://wiki.mapstory.org

**[Styling](items/styling.md)** - As a user, I need to be able to style layers I use in my story so that my story conveys meaning in the way I envision.

**[Mass editing of change over time] (items/versioning-proto.md)** - As a user, I need to be able participate in community versioned editing of the spatial, temporal and attribute information on features in any StoryLayer that is open for community editing.

**[Story composing] (items/composer-new.md)** - As a user, I need to be able to compose and publish my mapstory, and have it playback for viewers as I expected it to behave when I composed it.

**[Legend Enhancements] (items/legend.md)** - As a user, I need to be able to customize my legend in composer and have it appear the way I set it on a published story.

**[Storyteller Profiles] (items/storytellers.md)** - As a user, I need to be able to manage the actions I take on the platform, and the way that my actions and personal identity are presented to the public.

**[Playback settings] (items/playback-settings.md)** - As a user, I need to be able to control the way my story plays back once it is published.


### Medium (Within 10 months - August 30th, 2017)

**[Raster and uploader improvements] (items/raster.md)** - As a user, I need to import data as raster - single image or temporal sequence.

**[Search Improvements](items/search.md)** - As a user, I need to be able to find layers, stories and users with intuitive search - either by simply entering word searches, or by filtering in time, space, category, storyteller. Eventually I should be able to search within layers themselves to "find" features within a layer.

**[Remote data streams](items/remote-data.md)** - Instead of requiring all data to be uploaded to MapStory it
would be good to let users add remote data. Things like WMS, GeoRSS, KML. Some of these will likely be 'live', like
USGS earthquake maps, where we want them to stay up to date with latest.

**[Organization pages] (items/org-pages.md)** - As a user, I need to manage an Organization Page, which enables me to pool all the storytellers, storylayers and mapstories that represent a group.

**[Time Controls] (items/time-new.md)** - As a user, I need time controls on layers and stories that are intuitive, fast and honor the time information in my layers.

**[StoryPin Improvements] (items/annotations2.md)** - As a user, I need to be able to quickly and intuitively create StoryPin annotations that help me explain activity on the map that is not part of the data in my storylayers.

**[Warper integration] (items/warper.md)** - As a user, I need a map warper that is integrated with the mapstory importer.

**[Mobile](items/mobile.md)** - As a user, I need to be able to perform simple search, playback and profile management operations on mobile. Editing, composing, and uploading will not occur on mobile devices at this time.

**[Statistic upload and join existing geometries](items/table-join.md)** - As a user, I want to upload statistics and join that to sets of geometries maintained on MapStory.

**[Longitudinal Gazetteer](items/longitudinal-gazetteer.md)** - As a user, I want to link Place Names across data layers to support enhanced search, editing and storytelling

**[Internationalization](items/i18n.md)** - MapStory should be available to people regardless of what language they
speak. As a user, I want to make sure the site is all internationalized and start a crowd sourced localization effort.

**[Community Initiatives] (items/community-infra.md)** As a user, I need to be able to lead or participate in a Community Initiative. A Community Initiative is a data collection effort on a theme that encourages users to build out massive layers on the same schema. For example, “MapStory Local” will be a set of massive layers that represent of all of human settlement over time, with similar layers and features as one would see in Openstreetmap or Google Maps.

### Long Term (6 months to 12 months - funding dependent)

**[Developer Tab] (items/developer-tab.md)** - Add a section of the map/layer pages that lets developers know how
they can programmatically access the map and its data, like with openlayers, google maps, wms, wfs, etc.

**[Embed on more platforms] (items/embed.md)** - Get the tech and whitelists in place so MapStory embeds can go on
more platforms.

**[CSW + permissioning infrastructure (GN 2.0 upgrade)] (items/geonode2.md)** - Incorporate pycsw and the richer
permissioning infrastructure from GeoNode 2.0, once it gets stable.

**[Lat/long maps instead of Web Mercator] (items/latlong-maps.md)** - The web mercator projection is overused, distorts data, and
does not actually fit the aspect ratios of most computers well. As a user, I want to serve up MapStory in lat/long (4326).

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

**[Annotations improvements] (items/annotations.md)**- Bulk upload of annotations and a better editor

**[New Uploader] (items/uploader.md)** - New infrastructure for more robust handling, with client side validation and 
being able to add a raster to an existing storylayer. (Ian)

**[Social Login] (items/social-login.md)** - Be able to login to mapstory with facebook and google, and grab the relevant 
picture, name and email. (Marc)

**[Annotations Hotfixes] (items/annotations.md)** Basic tweaks to annotations improvements made in last milestone based on user feedback. (Bart)

**[User support and iterative improvements] (items/user-support.md)** - Constantly improve MapStory based on feedback
from users. 
