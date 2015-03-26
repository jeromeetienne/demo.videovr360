# A Minimal Device for AR
When looking closely at Augmented Reality, i came to realize that AR is possible using today devices.
So it can be deployed to the mass today.
There is no need to wait for some big technology discovery to happen 
and then wait some more for it to be distributed.
To run on today devices is definitely an important feature.

Let's see what would be a *minimal device for AR*...
Here are some requirements
* AR requires to localize the user in the space she or he is moving in
* AR requires to display 3d, the 'augmented content', on top of the 
  current reality.

### About device localisations
In order to display augmented content on top of our reality, AR devices
  need to localise itself in this reality.
Let's how to do that with current tech

**Markers** 
* Simple one is to use the camera of your phone and recognize 
  markers in the images. 
  Thus you know the position of the phone related to the marker which is in our reality
* PRO: it is available now and it is wellknown technology
* CON: it requires to have a marker in our reality. So you have to print it
  and to place it in your reality. It is a burden.
* CON: To recognize the marker consumes significant CPU resources.
  There are a lot of images in the video stream from the camera.
  A phone got a limited amount of CPU power
* PRO: provide orientation/translation of the device relatively to the marker.

**API for Devices orientations**
* Devices orientation is directly available from a [standard w3c API](http://www.w3.org/TR/orientation-event/)
* One could say it is the same for devices location API,
  called [Geolocation API](http://dev.w3.org/geo/api/spec-source.html).
  Nevertheless devices location typically provided in mobile is quite inprecise
  For sure not precise enougth for augmented reality.
* Device orientations API provides usable informations tho, even if limited.
* So you need to develop the augmented content so it fits within those limits.
  What about a UI which will be displayed 'around' the user ?


### Old notes
* Augmented reality minimal devices is surprisingly simple to produce.
  It is in fact very reachable with current technology. Something like tango phones. 
  TODO opaque screen,  depth sensors. Depth sensor is the newest.
  Kinect has been doing it for years. 
  Leap motion is more recent but still is 2 years old.
  Now everybody seems to move in this direction
* What about a device like an iPad but with see thru screen ? 
  With some strong padding around the screen. Like iPad safe ghetto cover. The batteries and other hardware hidden in the handles. Style isn't too classy but it fits the
  utility look. And it is robust so for yet another utility requirement. 
* augmented reality is a lot easier when it comes to latency.
  Augmented reality content is likely something small in the middle of current reality.
  It allows see thru screen. No strong requirement on latency.
* Performance like 15 fps is usable in this specific context. 

**Possible improvement: a see-thru screen**
