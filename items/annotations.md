### Description

MapStory's annotations are so bad as to be practically unusable. Let's make them at least usable.

### Goal

Our aim for this task is not annotations perfection, just to get them to a decent state. It should be 
possible to upload annotations, to edit any existing annotation, ideally with some bulk editing options,
and to add youtube and pictures.

### Spec / Requirements

There are three main new requirements to support in addition to what is already working now on annotations

**Grid editor for annotations** - Right now to edit an annotation you can select 'edit notes' and select an existing 
note. There is no intuitive way to edit a note that does not have a geometry. A grid editor for annoations will
give editors one single place to manage all their annotations. It should ideally be sortable by at least time and
title. The editor should be able to handle at least 5000 annoations, as there is a story layer with people who have 
notes on 5000 events in it.

**Upload of Annotations** - Somewhere in the interface a user should be able to upload a csv file of annotations.
We can specify the structure of this csv in the documentation, and have users match that. No need for fancy figuring
out of bad files, just give them an error message on the proper format. We probably want to give them the option
to either append their existing annotations or to overwrite them.

**Media** We need to add in an option for users to add a youtube video or picture. Bart did initial work on this,
but it involved inline editing of html. We did this because it was very hard to change the backend model. This 
should be much easier with the change to Django for storing annotations. Ian suggested we just use a single url
field and detect the media type like we do elsewhere on mapstory. So need to just have a 'media' button in addition
to 'description' where users can enter a url for a picture or youtube video. Ideally give them feedback when they
enter a url that is not either. We could also just let them enter a link there, and make it a hyperlink to click
on in the annotation.

### Wireframes
(placeholder)

Questions to be answered by wireframes:

Where do we do bulk upload?
More intuitive dragging of notes
Evolution of 'notes' drop down. Does edit go away, since all fields should be editable? 
Dealing with 5000 notes - bulk delete?

### Tech thoughts / plan

 - refactor backend
 - stick with ext on front end
 - openlayers protocol
 

#### People
@iwillig is the owner of this feature. @ischnieder to help on backend, with @bartvde on code review and advice.

#### Issues

All issues are in https://github.com/opengeo/mapstory/issues?labels=Annotations&milestone=15&page=1&state=open
