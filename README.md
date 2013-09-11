![Sharefest](https://raw.github.com/Peer5/ShareFest/master/sharefest/public/img/logo.png)

One-To-Many sharing application. Serverless.
Eliminates the need to fully upload your file to services such as Dropbox or Google Drive.
Put your file and start sharing immediately with anyone that enters the page.
Pure javascript-based. No plugins needed thanks to HTML5 WebRTC Data Channel API - http://webrtc.org

How does it work
================
http://sharefest.me/faq
http://www.youtube.com/watch?v=p2HzZkd2A40&feature=youtu.be&t=15m30s

Sharefest operates on a mesh network similar to Bittorrent network.
The main difference is that currently the peers are coordinated using an intelligent server.
This coordinator controls which parts are sent from A to B and who shall talk with whom.
Peer5 Coordinator (or any other solution) is used to accomplish this.
Each peer will connect to few other peers in order to maximize the distribution of the file.
Supporting Chrome (>26) and Firefox (>19)

First version includes a simple page that one user will drag a file onto to
share, and other users will enter the first user's url and start downloading the file.

Hosted version: http://sharefest.me

TODO:
============
* see issues - https://github.com/Peer5/ShareFest/issues

Quick setup
==============
1. Install [nodejs](http://nodejs.org/)
1. [Download](https://github.com/Peer5/ShareFest/archive/master.zip) this repo and unzip it, or `git clone https://github.com/Peer5/ShareFest.git`
1. `cd ShareFest`
1. Get the [SocialSharePrivacy](https://github.com/patrickheck/socialshareprivacy/#readme) add-on: either [download](https://github.com/patrickheck/socialshareprivacy/archive/master.zip) and unzip it inside `ShareFest/`, or `git submodule update --init`
1. `npm install --dedupe` to install dependencies.
1. `npm start` to start the server
1. http://localhost:13337 should work

Environment Variables
==============
NODE_ENV: development or production
REQUIRE_HTTPS: 1 redirect to HTTPS when http GET request is coming

About
==============
Sharefest started by Peer5 at the SV DevFest 2012 hackathon (San Jose).
It was soon open sourced to GitHub and now being developed by Peer5 and a community of great WebRTC hackers.

License
==============
Apache 2.0 - see LICENSE file
