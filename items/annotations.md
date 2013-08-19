## Annotations improvements

MapStory's annotations are so bad as to be practically unusable. Let's make them at least usable.

### Goal

Our aim for this task is not annotations perfection, just to get them to a decent state. It should be 
possible to upload annotations, to edit any existing annotation, ideally with some bulk editing options,
and to add youtube and pictures.

This will also cover hot fixes to the overall annotations improvements that were recently promoted.

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

**Media** - We need to add in an option for users to add a youtube video or picture. Bart did initial work on this,
but it involved inline editing of html. We did this because it was very hard to change the backend model. This 
should be much easier with the change to Django for storing annotations. Ian suggested we just use a single url
field and detect the media type like we do elsewhere on mapstory. So need to just have a 'media' button in addition
to 'description' where users can enter a url for a picture or youtube video. Ideally give them feedback when they
enter a url that is not either. We could also just let them enter a link there, and make it a hyperlink to click
on in the annotation.

One smaller improvement that Ivan suggested is it would be nice to hit at least a bit is the selection of dates.
Right now it defaults to the current date when you use the date drop downs. That seems like one of the worst defaults,
since mapstory is all about history. So would be nice to have at least that small improvement, and would be great
to have something more intuitive in general for selection of what the annotation applies to. 

### Wireframes
(placeholder)

Questions to be answered by wireframes:

What is the overall 'notes' interface. We want the grid editor in there, but does it replace existing buttons?
One way to go might be to have 'notes' button open up the grid editor and any additional buttons needed. Does
'edit' drop away because we have an editable grid? 

Where do we do bulk upload? What is the workflow for it? How do you choose to overwrite vs append? Is there
a default action, or does it ask you every time? 

How do you deal with 5000 notes? Is there paging of some sort? Bulk edit actions? Thinking like 'delete', if
you accidentally import the wrong notes or too many.

A nice improvement suggested by Ivan would be to have the date default to the map's current date, instead of
today's date. In general would be nice to flesh out some more intuitive date selection instead of date drop
downs. Perhaps a slider that has the start and end at the time range of the map, that you can slide up and down to select.
Implementation of this may be beyond the scope of this round, but some wireframes would be great. 

Would be awesome to have some exploration of a more intuitive way to add notes. The dialog right now is fairly
clunky. Some that are a bit more intuitive are http://meograph.com and http://historypin.com Tucker likes the 
idea of just dragging a note on to the map. Again this may be beyond scope for this round, but would be good
to have some nice wireframes.


### Tech thoughts / plan

First step is to refactor the annotation backend to use django models with some geospatial and temporal fields
instead of using WFS. This will let us change the annotations model much more easily, as well as do upload without
having to bother with GeoServer's importer code.

Second is to implement an openlayers protocol so our annotations can be treated as features. This will be used with
GeoExt's feature manager and displayed in a grid. We will implement all in Ext.js and associated libraries.
 

#### People
@iwillig is the owner of this feature. @ischnieder to help on backend, with @bartvde on code review and advice.

#### Issues

All issues are in https://github.com/opengeo/mapstory/issues?labels=Annotations&milestone=15&page=1&state=open
