## Product Vision

MapStory.org is the atlas of change that everyone can edit. It seeks to organize humanity's shared knowledge about how the world evolves geographically over time, and to make this knowledge easily accessible as an open educational resource. The platform is sustained by the nonprofit MapStory Foundation and dedicated volunteers, contracting partners and sponsors.

The project was originally started by Dr. Christopher Tucker who, as a graduate student at Columbia University, "dreamt of a platform where anyone could search spatially and temporally and find out what the preponderance of social scientists knew about what had been going on. And better yet, let anyone who might know something the social scientists don't improve upon that knowledge through continuous editing." The goal was to provide a compliment to other open knowledge platforms, such as Wikipedia and OpenStreetMap, that focused on spatio-temporal change (or, in other words, historical geography).

This original sentiment still drives the MapStory.org product vision today, although prototyping has helped clarify the technical approach and target audience that form the project's implementation.

As we begin 2017, we understand MapStory.org to be for scholars, students and enthusiasts around the world seeking historical perspective on any topic that can be mapped over time - whether that topic is hyper local, such as the rise of a town, or hyper global, such as the movement of continents. The current MapStory.org platform brings three core technical components together that have never been combined before in order to provide users with a fundametally unique and comprehensive way to understand how our world evolves of time and space. First, it uses the open source GeoNode as a scalable spatial infrastructure for data. Second, it uses GeoGig as a version-editing tool so that all data in MapStory.org can be continuously improved over time. And third, it adds a mapstory "composer" that was built from scratch so users could go beyond mere data visualization to convey deeper narratives about why and how phenomena play out as they do. These three components are integrated with a traditional open geo stack, including GeoServer and PostGIS.

From the start of MapStory.org, we hoped the project would make a great impact on geography education in both formal and informal learning settings. As the project matures, we also realize it can have an impact in other settings - supporting international develop workers seeking understanding on historical change in far off places, helping journalists explain issues to their readers, and even improving public policy decision-making.

## Project Status

The first version of the platform was dubbed a "public prototype in development" and launched in April, 2012. Leveraging the Open Geo software stack, it let a registered upload spatio-temporal datasets, generate unique styles for the data, and play the data over time and space. Over 2,000 users accessed the prototype and completed projects that appeared in popular media, like the Washington Post, Vox, and the Atlantic Magazine.

In January 2017 a Beta version of MapStory.org was released that represents virtually an entire rebuild of the platform. From a user perspective, the main upgrades were the introduction of a new mapstory "composer" that allows for multi-chapter storytelling, and version editing of StoryLayers. On the back-end, the platform has also been upgraded to the latest version of the GeoNode and incorpated the new OS-Geo importer.

## Project Roadmap

The roadmap below is intended to guide continuous improvement of the Beta release during 2017 and beyond. Each item is a feature organized into 5 themes that form the core of the platform - exploring, importing, editing, storytelling, and identiy management, as well as cross-cutting issues and back-end infrastructure and DevOps concerns. The current MapStory development team will meet in the first week of January, 2017 to estimate level of effort for features, order them by priority, and determine high-level timeframes for Beta upgrade releases. Timeframes will be turned into Milestones in Github.

### Exploring

**[Locate StoryLayers and MapStories in Space and Time](items/search.md)**

**[Show StoryLayers and MapStories that are "related" to each other](items/related-content.md)**

**[Refine notification streams to help users follow activity they care about](items/notification-streams)**

### Importing

**[Enable import of raster imgagery] (items/raster.md)**

**[Establish seamless sync between warper.mapstory.org and MapStory importer] (items/warper.md)**

**[Connect importer to remote data streams](items/remote-data.md)**

**[Allow uploads of statistics that can join to common geometries (like states or countries)](items/table-join.md)**

**[Incorporate Longitudinal Gazetteer](items/longitudinal-gazetteer.md)**

### Editing & Reviewing

**[Mass editing of change over time] (items/versioning-proto.md)**

**[Define algorithms and values behind peer review tools](items/peer-review.md)** - We need to futher define the user experience
of our peer review tools (star rating and flag error). Also explore other features for curating quality and signaling rigor.

### Storytelling

**[Styling](items/styling.md)** - As a user, I need to be able to style layers I use in my story so that my story conveys meaning in the way I envision.

**[Story composing] (items/composer-new.md)** 

**[Playback settings] (items/playback-settings.md)** - As a user, I need to be able to control the way my story plays back once it is published.

**[Legend Enhancements] (items/legend.md)** - As a user, I need to be able to customize my legend in composer and have it appear the way I set it on a published story.

**[Time Controls] (items/time-new.md)** - As a user, I need time controls on layers and stories that are intuitive, fast and honor the time information in my layers.

**[StoryPin Improvements] (items/annotations2.md)** - As a user, I need to be able to quickly and intuitively create StoryPin annotations that help me explain activity on the map that is not part of the data in my storylayers.

### Identities

**[Login and account creation] (items/oauth.md)** - As a user, I need to enable MapStory login to work on mapstory.org, http://warper.mapstory.org and http://wiki.mapstory.org

**[Storyteller Profiles] (items/storytellers.md)** - As a user, I need to be able to manage the actions I take on the platform, and the way that my actions and personal identity are presented to the public.

**[Organization pages] (items/org-pages.md)** - As a user, I need to manage an Organization Page, which enables me to pool all the storytellers, storylayers and mapstories that represent a group.

**[Community Initiatives] (items/community-infra.md)** As a user, I need to be able to lead or participate in a Community Initiative. A Community Initiative is a data collection effort on a theme that encourages users to build out massive layers on the same schema. For example, “MapStory Local” will be a set of massive layers that represent of all of human settlement over time, with similar layers and features as one would see in Openstreetmap or Google Maps.

### Cross-cutting

**[3D MapStories](items/3d.md)** - There are several cool WebGL toolkits that may let us view MapStories not just in
2D but in 3D, over time. As a user, I want to incorporate these.

**[Mobile](items/mobile.md)** - As a user, I need to be able to perform simple search, playback and profile management operations on mobile. Editing, composing, and uploading will not occur on mobile devices at this time.

**[Internationalization](items/i18n.md)** - MapStory should be available to people regardless of what language they
speak. As a user, I want to make sure the site is all internationalized and start a crowd sourced localization effort.

**[Animated Sharing](items/animated-sharing.md)** - When we share MapStories on social networks they tend to be a 
single screenshot. We should investigate animated gif and video outputs for MapStory, as that can make social
sharing communicate the motion inherent in the stories.

**[Automate contributions from 3rd parties with widgets](items/widgets.md)** - We should explore ways to plant a simple
'Add to MapStory' button on external sites that focus on spatial-temporal data collection. An example partner interested
in something like this is historyit.com

### Infrastructure/DevOps

**[Scalability improvements] (items/scalability.md)** - 

**[Developer Tab] (items/developer-tab.md)** - Add a section of the map/layer pages that lets developers know how
they can programmatically access the map and its data, like with openlayers, google maps, wms, wfs, etc.

### Ideas (catch all)

**[CSW + permissioning infrastructure (GN 2.0 upgrade)] (items/geonode2.md)** - Incorporate pycsw and the richer
permissioning infrastructure from GeoNode 2.0, once it gets stable.

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


### Completed

Items that have been fully deployed to production

**[Lat/long maps instead of Web Mercator] (items/latlong-maps.md)** - The web mercator projection is overused, distorts data, and
does not actually fit the aspect ratios of most computers well. As a user, I want to serve up MapStory in lat/long (4326).

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
