#Dota 2 WebAPI Examples#

WebAPI forum: http://dev.dota2.com/forumdisplay.php?f=411

This GitHub repository serves as a home for source code samples that demonstrate how to use different parts of the Dota 2 WebAPI, and tie it in to other libraries and good practices, such as using Memcached to cache WebAPI results. These are specific examples that I've written in my free time using publicly available WebAPI methods to help give Dota 2 WebAPI newcomers starting points for projects that they might want to build.

<br />

###Example 1: Live League Game Signature Image (live_league_signature.php)###

This example is a feasible forum signature that will show forum-goers the currently-live league matches occuring on Dota 2 at the time. It will rotate through all of the live league games, giving each one 3.5 seconds of visibility before moving onto the next and wrapping back around to the first.

*This image is an example of what the signature looks like, but is not live itself. Visit [this link](http://server.danieljennings.net/live_league_signature.php) to see a live version.*

![Signature](http://server.danieljennings.net/example_live_league_signature.gif)

#####Requirements:#####
* A web server capable of serving PHP pages (e.g. http://httpd.apache.org/)
* PHP5 (http://www.php.net)
* ImageMagick for PHP5 (http://www.php.net/manual/en/imagick.installation.php)
* Memcached for PHP5 (http://www.php.net/manual/en/memcached.installation.php)

#####Demonstrates:#####
* WebAPI: GetLeagueListing
* WebAPI: GetLiveLeagueGames
* Caching: Using Memcached to reduce latency by caching WebAPI results
* Images: Using ImageMagick to render images on-demand.

<br>
