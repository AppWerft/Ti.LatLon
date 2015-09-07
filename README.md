Ti.LatLon
=========

Titanium module for calculation some GIS stuff.

###Usage###

Calculation of distance and bearing between two points:
```javascript
var LL = require('de.appwerft.latlon');
var Origin = new LL.LatLon(53.5523,10.1);
var Destination = new LL.LatLon(54.7,10.4);
console.log(Distance is: ' + Origin.distanceTo(Destination));
console.log(Distance ist: ' + Origin.bearingTo(Destination));

```

####finalBearingTo###
Returns final bearing arriving at destination destination point from 'this' point; the final bearing
* will differ from the initial bearing by varying degrees according to distance and latitude.

####midpointTo####
Returns the midpoint between 'this' point and the supplied point.

####destinationPoint####
Returns the destination point from 'this' point having travelled the given distance on the
* given initial bearing (bearing normally varies around path followed).

####intersection####
Returns the point of intersection of two paths defined by point and bearing.

####crossTrackDistanceTo####
Returns (signed) distance from ‘this’ point to great circle defined by start-point and end-point.


More method you can find in source of module.


###Credits###

Thakns to [Chris Veness](http://www.movable-type.co.uk/scripts/latlong.html)