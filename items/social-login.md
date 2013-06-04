
### Description

Instead of making people signup for yet another account we should allow them to login with an existing Google or
Facebook account. 

### Goal

There is a decent amount of work complete on this, with login enabled for Google, Facebook and Twitter. To get 
it on production we need to get things working properly with user profiles so that they actually save time.

### Requirements

To get this on production there is only two real requirements, and a few nice to haves.

The one requirement is completing https://github.com/opengeo/mapstory/issues/611  Though we grab the info
somewhere and display it we don't bring it in to the user's editing environment. And they get messages
about how they need to fill out their full name and picture before they show up in search, even though
looking at it their full name and picture are there.

The other is to remove twitter as a login, https://github.com/opengeo/mapstory/issues/718 

Past that a few things would be nice to do.

* https://github.com/opengeo/mapstory/issues/568 working with social login, so users get the information
* A screen after they login to fill out their blurb, so they become full users right then.
* Automatically populate their 'network' link with what they logged in with
* Have 'password reset' work. I feel like this worked at one point but I could be wrong. But ideally it just
generates a password for just their mapstory account. Then they can login without having to use the original social
login they used. It should be able to use the email associated with the account.
* Bring twitter in, with required email sign up.

