## Animated Sharing 

When we share MapStories on social networks they tend to be a single screenshot. We should investigate 
animated gif and video outputs for MapStory, as that can make social sharing communicate the motion 
inherent in the stories.

### Notes

GeoServer has an animated gif output already. One limitation is that it won't work with base layers like
google or openstreetmap. But if we host our own tiles then it should be possible with cascading the WMS
from those. Will need a UI to let people create it.

Another option is video. See mapstory/mapstory#674 for example. Quicktime may
be a good option, or a more open format. Ideally would be same UI as the animated gif, but would have
less limitations on size/frames. 

To work with twitter cards we'd need H.264 format. See https://dev.twitter.com/docs/cards/types/player-card
