Ti.LatLon ![](https://camo.githubusercontent.com/0708b17f8cc6b5aa19d0cf5ef38e978c3cfc38e4/687474703a2f2f696d672e736869656c64732e696f2f62616467652f67697474696f2d312e302e302d3030423443432e737667)
=========

Titanium module for calculation some GIS stuff.

###Usage###

Calculation of distance and bearing between two points:
```javascript
var LL = require('de.appwerft.latlon');
var Origin = new LL.LatLon(53.5523,10.1);
var Destination = new LL.LatLon(54.7,10.4);
console.log(Distance is ' + Origin.distanceTo(Destination));
console.log(Bearing is ' + Origin.bearingTo(Destination));

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

####rhumbDistanceTo####
Returns the distance travelling from 'this' point to destination point along a rhumb line.

####rhumbBearingTo####
Returns the bearing from 'this' point to destination point along a rhumb line.

####rhumbDestinationPoint####
Returns the destination point having travelled along a rhumb line from 'this' point the given
* distance on the  given bearing.

####rhumbMidpointTo####
Returns the loxodromic midpoint (along a rhumb line) between 'this' point and second point.




More details of methods you can find in source of module.


###Credits###

Thakns to [Chris Veness](http://www.movable-type.co.uk/scripts/latlong.html)