## Intra-platform messaging

Improve MapStory so that registered users can message other registered users. 

### Requirements

Messaging should enable users to send private emails to one another without revealing their email addresses.
No need to flesh out lots of requirements as we will likely just evaluate django messaging systems and pick
one that seems to meet our needs the best.

The messaging should coordinate with our other user email notification from activity feeds, perhaps doing a bit of a 
revamp of that, so that comments, rating and using mapstories goes to the same 'user inbox' as direct 
messages. Then users could respond to other users rating/commenting/using their content with a message
back to them, starting a dialog.

### Tech Plan

First is to evaluate which framework might meet our needs. GeoNode has some experience with it, using one
for the ANZSM project. I believe it was [Django Messaging] (https://code.google.com/p/django-messaging/) There seem to be some
other options at https://www.djangopackages.com/grids/g/messaging/ and another one mentioned on [stack overflow]
(http://stackoverflow.com/questions/4577553/private-messaging-in-django) is [Django PM] (https://code.google.com/p/django-pm/]

After evaluating what to use should see if our activity stuff can hook up to it so those messages also
go to the user's inbox if there is one.

