## User Story

As a user, I need an editing interface for StoryLayers that makes it easy to see all features in the layer, to see edits that have already been made to the Storylayer and by whom, and to make new edits to the StoryLayer myself.

## Requirements

The current 0.0 editing interface has a basic sidebar that lets a user add, edit, or delete features on a StoryLayer. As features are edited, an "Edit History" tracks them. Additionally, the user can view a Table of the features, but cannot edit from the table view in a way that edits are tracked. The current editing interface and workflow leaves several issues unaddressed including:

- [ ] Users can't edit from the Table View
- [ ] There is no styling tools in the edit mode. Styling in edit mode should be aimed and communicating to an editor the status of a feature (r a confidence interval). For example, features that are _known_ to be unverified should clearly be indicated as such, while features that have been edited many times should also be clearly indicated as such.
-  [] There is no way for editors to add commentary or "notes" about their edits. For example, an editor may want to note that evidence they have to support an edit, or uncertainty that they have despite making an edit.
- [ ] User should be able to add a new attribute to a StoryLayer after it has been created or uploaded. So, for example, if I have a StoryLayer of "beer breweries" and I begin with a few attributes, like "Brewery Name", "Start Date" and "Brewery Founder"...but during the course of the research I realize I need to collect "Type of Beer", I cannot do so. Letting the StoryLayer owner add or modify attributes as more is learned would greatly improve the crowd-editing nature of the platform.

## User and Design Stories

### People
