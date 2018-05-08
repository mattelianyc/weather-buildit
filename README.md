

you can build and run the app by DL'ing the repo to your local system and running any kind of simple HTTP server from the root dir of the project within a UNIX-based Terminal -- i.e. python -m SimpleHTTPServer ${PORT}

my thought process behind this solution:
* To use animations to visualize the weather conditions rather than express through text.  As such, when it is raining there is a rain animation; when there are 0 clouds in the sky there are no more clouds animating across the screen;
* these animations overlay an embedded googe map iframe of the location (hardcoded as DUMBO in this demo.)

tradeoffs:
* the embedded iframe for google map is causing the long loading time, with more time/larger scope than a coding challenge, i would have implemented the actual Google Maps API which wouldve allowed more control over configs effecting loading time + would allow for some cool styling as well
* when viewing the app on my public web server I've only tested Google Chrome Browser.  When hitting the URL make sure to do so via "https://" it might say the security credentials are unsecure, howwever, if you click through anyways and click 'allow' geolocation in browser alert popup it will(*fingers crossed*) work.