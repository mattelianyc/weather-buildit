you can build and run the app by DL'ing the repo to your local system and running any kind of simple HTTP server from the root dir of the project within a UNIX-based Terminal -- i.e. python -m SimpleHTTPServer ${PORT}

my thought process behind this solution: To use animations to visualize the weather conditions rather than express through text.  
- As such, when it is raining there is a rain animation; 
- when there are 0 clouds in the sky there are no clouds animating.  The greater the cloud count (a data prop included in the API) the more clouds are displayed.
- When the current weather is foggy there is a fog animation.

tradeoffs:
-  when viewing the app on my public web server I've only tested Google Chrome Browser.  When hitting the URL make sure to do so via "https://" it might say the security credentials are unsecure, howwever, if you click through anyways and click 'allow' geolocation in browser alert popup it will(*fingers crossed*) work.  https://www.mattelia.com 

With more time:
- I’d implement more dynamic visualizations ( i <3 animated software experiences )
- I’d add a toggle button to each of the 5 day weather data ‘containers’.  onClick => the container would expand to show the hourly forecast.

Appreciate your time and consideration.  Hope to hear from ya soon :)