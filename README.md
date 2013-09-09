![Sharefest](https://raw.github.com/Peer5/ShareFest/master/public/img/logo.png)

One-To-Many sharing application. Serverless.
Eliminates the need to fully upload your file to services such as Dropbox or Google Drive.
Put your file and start sharing immidiately with anyone that enters the page.
Pure javascript-based, no plugins needed, thanks to HTML5 WebRTC Data Channel API - http://webrtc.org

How does it work
================
http://www.youtube.com/watch?v=p2HzZkd2A40#t=15m29s

Sharefest operates on a mesh network similar to Bittorrent network.
The main difference is that currently the peers are coordinated using an intelligent server.
This coordinator controls which parts are sent from A to B and who shall talk with whom.
Peer5 Coordinator (or any other solution) is used to accomplish this.
Each peer will connect to few other peers in order to maximize the distribution of the file.
Supporting Chrome (>26, now stable) and Firefox (>19)

First version includes a simple page that one user will drag a file to
share, and a other users will enter the first user's url and start downloading the file.

test it out at: http://sharefest.me

TODO:
============
* local storage
* RESTful API
* tests
* see issues - https://github.com/Peer5/ShareFest/issues

Quick setup after cloning
==============
* install nodejs
* run `git submodule update --init` to clone the _social share privacy_ submodule
* cd into sharefest root directory and do "npm install"
* run `node server.js`

About
==============
Sharefest started by Peer5 at the SV DevFest 2012 hackathon (San Jose).
It was soon open sourced to GitHub and now being developed by Peer5 and a community of great WebRTC hackers.

License
==============
Apache 2.0 - see LICENSE file
