## Statistic upload and join existing geometries

We replicate lots of data needlessly, making users upload their own geometries when all 
they want to do is style based on some new statistics. We should be able to let them just 
upload statistics and join that to sets of geometries maintained on MapStory.

### Notes

OpenGeo did something like this years ago, but it never moved beyond prototype. GeoCommons
also had something that handled this.

There is a Table Joining Service implementation that's been implemented for GeoServer,
that could potentially be used as the basis for this.

Other thing needed would be solid base layer data.

Ideally we also let people upload their own shapes and join other data to them.
