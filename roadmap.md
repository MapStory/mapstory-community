## Product Vision

MapStory.org is the atlas of change that everyone can edit. It seeks to organize humanity's shared knowledge about how the world evolves geographically over time, and to make this knowledge easily accessible as an open educational resource. The platform is sustained by the nonprofit MapStory Foundation and dedicated volunteers, contracting partners and sponsors.

The project was originally started by Dr. Christopher Tucker who, as a graduate student at Columbia University, "dreamt of a platform where anyone could search spatially and temporally and find out what the preponderance of social scientists knew about what had been going on. And better yet, let anyone who might know something the social scientists don't improve upon that knowledge through continuous editing." The goal was to provide a compliment to other open knowledge platforms, such as Wikipedia and OpenStreetMap, that focused on spatio-temporal change (or, in other words, historical geography).

This original sentiment still drives the MapStory.org product vision today, although prototyping has helped clarify the technical approach and target audience that form the project's implementation.

As we begin 2017, we understand MapStory.org to be for scholars, students and enthusiasts around the world seeking historical perspective on any topic that can be mapped over time - whether that topic is hyper local, such as the rise of a town, or hyper global, such as the movement of continents. The current MapStory.org platform brings three core technical components together that have never been combined before in order to provide users with a fundamentally unique and comprehensive way to understand how our world evolves over time and space. First, it uses the open source GeoNode as a scalable spatial infrastructure for data. Second, it uses GeoGig as a version-editing tool so that all data in MapStory.org can be continuously improved over time. And third, it adds a mapstory "composer" that was built from scratch so users could go beyond mere data visualization to convey deeper narratives about why and how phenomena play out as they do. These three components are integrated with a traditional open geo stack, including GeoServer and PostGIS.

From the start of MapStory.org, we hoped the project would make a great impact on geography education in both formal and informal learning settings. As the project matures, we also realize it can have an impact in other settings - i.e. supporting international development workers seeking understanding on historical change in far off places, helping journalists explain issues to their readers in visually compelling ways, and even improving public policy decision-making.

## Project Status

The first version of the platform was dubbed a "public prototype in development" and launched in April, 2012. Leveraging the Open Geo software stack, it let a registered user upload spatio-temporal datasets, generate unique styles for the data, and play the data over time and space. Over 2,000 users accessed the prototype and completed projects that appeared in popular media, like the Washington Post, Vox, and the Atlantic Magazine.

In January 2017 a Beta version of MapStory.org was released that represents virtually an entire rebuild of the platform. From a user perspective, the main upgrades were the introduction of a new mapstory "composer" that allows for multi-chapter storytelling, and version editing of StoryLayers. On the back-end, the platform has also been upgraded to the latest version of the GeoNode and incorpated a new OS-Geo importer.

## Project Roadmap

The roadmap below is intended to guide continuous improvement of the Beta release during 2017 and beyond. Each item is a feature organized into 5 themes that form the core of the platform - exploring, importing, editing, storytelling, and identiy management, as well as cross-cutting and infrastructure issues. The current MapStory development team will meet in the first week of January, 2017 to estimate level of effort for features, order them by priority, and determine high-level timeframes for Beta upgrade releases. Timeframes will be turned into Milestones in Github.

### Infrastructure

In order to scale as envisioned, MapStory.org requires a technical infrastructure that can support such scale. In 2017 the infrastructure priorties are to deal with residual technical debt left over from 2016 development, to complete test coverage for the app, and to refine our DevOps process that enables bug reports to migrate from demo to production environments, among others.

**[Technical Debt] (items/technical-debt.md)**

**[Tests] (items/tests.md)**

**[DevOps]

**[Scalability improvements] (items/scalability.md)**

**[Add a Developer's Tab to StoryLayer and MapStory detail pages] (items/developer-tab.md)**

### Exploring

The purpose of Exploring in MapStory.org is to empower visitors to the site (whether they are registered users or not), to find and view StoryLayers and MapStories, and to learn about Storytellers who have created this content. A non-registered user will essentially have read-only powers over content. They can hit play and embed content on another site or share it on social media. The experience should be a bit like visiting YouTube and watching videos. As a space-time atlas, it is very important that visitors be able to Explore along the dimensions of time and space. They should be able to ask themselves "what time periods am I interested in seeing content about?" or "what geographic areas am I interested in seeing content about?"

For a Registered User, exploring is about initiating action. A registered user goes to a StoryLayer, for example, with the intent of potentially improving it through editing, or using it for a mapstory they want to tell. A registered user goes to a MapStory with the intent of potentially using the layers used in that story to go off and make their own story. Registered users are also empowered to be curators or peer reviewers...adding ratings, flags and comments to content as they see it. The initial action of exploring is similar for registered and non-registered users...they want to find content that interests them. But a registered user's powers of action around content once they get to what they are looking for are different.

#### In 2017, the priorities for improving the exploring experience are:

**[Locate StoryLayers and MapStories in Space and Time](items/search.md)**

**[Show StoryLayers and MapStories that are "related" to each other](items/related-content.md)**

**[Enable searching for and playing MapStories on mobile devices](items/mobile.md)**

**[Enable animated GIF or video output for viral sharing](items/animated-sharing.md)**

**[Refine notification streams to help users follow activity they care about](items/notification-streams.md)**

### Importing/Creating StoryLayers

The core foundation of MapStory.org is the spatio-temporal data layers that exist inside of the platform. These StoryLayers are a bit like a wikipedia article in the form of an animated map in the sense that they try to provide the "objective" what/wheren/when, and they can be constantly edited for completeness and accuracy, with edits being tracked by users and versioned. Users can begin StoryLayers by importing raw data, or by creating a new StoryLayer right in the app.

#### In 2017 the priorities for improving the import and creation of StoryLayers are:

**[Enable import of raster imgagery] (items/raster.md)**

**[Establish seamless sync between warper.mapstory.org and MapStory importer] (items/warper.md)**

**[Support data imports with time information extending to 4.5 billion years BCE](/items/geologic-time.md)**

**[Connect importer to remote data streams](items/remote-data.md)**

**[Allow uploads of statistics that can join to common geometries (like states or countries)](items/table-join.md)**

**[Incorporate Longitudinal Gazetteer for place names](items/longitudinal-gazetteer.md)**

**[Enable Community Initiative Leads to define pre-set Schemas for data imported or appended to Initiative StoryLayers] (items/community-infra.md)**

### Editing & Reviewing

The goal of editing and reviewing is to make StoryLayers more complete and accurate. Editing occurs at the level of the features inside a StoryLayer. Reviewing occurs on the layer at a general level - i.e. by rating the layer as a whole or flagging the layer as a whole. Over time, hopefully, the best StoryLayers on a topic will rise to the top, and rather than duplicating StoryLayers, users will begin to just add marginal improvements on existing StoryLayers. For example, we probably only need one dataset (StoryLayer) about the history of post offices in America. Every time a new post office gets opened, or another one closed, we should just be able to edit a Post Offices storylayer.

#### In 2017, the priorities for improving the editing and reviewing experience are:

**[Implement new interface for StoryLayer editing] (items/versioning-proto.md)**

**[Show more editing status information on StoryLayer detail pages](items/Editing-Status-Display.md)**

**[Enable feature editing from a table rather than just on the map](items/table-based-editing.md)**

**[Define algorithms and response rules for peer review tools](items/peer-review.md)**

**[Enable editing of StoryLayers from a mobile device](items/mobile.md)**

### Storytelling

Storytelling is the process of combining objective StoryLayers with other types of subjective annotation and media. The goal of a MapStory is to answer "how" and "why" questions, not just the "what/where/when". Storytellers should be able to use StoryLayers already in the platform provided by others and put those StoryLayers to work for the story they want to tell. This means adding a unique style to StoryLayers, only using part of a StoryLayers total timespan, controlling zoom levels for StoryLayers so we only see the geography that the storyteller wants us to see, adding contextual info, etc.

#### In 2017, the priorities for improving the storytelling experience are:

**[Create scaled-down viewer detail page for single-chaper mapstories ("short stories")](items/playback-settings.md)**

**[Provider story owners more power to customize story detail pages](/items/MapStory_Detail_Page.md)**

**[Implement new interface for MapStory composing] (items/composer-new.md)** 

**[Implement playback modes ("Museum", "Interactive)] (items/playback-settings.md)**

**[Provide mapstory "templates" with pre-set element configurations](items/mapstory-templates.md)**

**[Let storyteller customize their Legend] (items/legend.md)**

**[Upgrade functionality of FeatureBoxes] (items/feature-boxes.md)**

**[Add heatmap and clustered styling](items/styling.md)**

**[Support Geologic Time for all MapStory elements] (items/time-new.md)**

**[Enable StoryPins to be streamed off the map in sidebar] (items/annotations2.md)**

**[Enable multiple users to work on the same MapStory, at the same time](multi-user-mapstorytelling.md)**

**[Enable 3D MapStories](items/3d.md)**

### Identities

Everything in MapStory.org is done by _people_. It is a social platform with high attribution. The right metaphor is to a book authored by lots of people, not a database. Thus, users need a profile that they can control to present their work, and to be able to manage how they are represented across the platform.

#### In 2017, the priorities for improving the management of identities are:

**[Integrate logins across mapstory.org, Wiki, Warper and other tools] (items/oauth.md)**

**[Let users edit basic profile information on a mobile device](items/mobile.md)**

**[Let users control display of their StoryLayers and MapStories on their profile] (items/storytellers.md)**

**[Provide Organization Page owners with analytics] (items/org-pages.md)**

### Cross-cutting

**[Translate MapStory into many languages](items/i18n.md)**

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
