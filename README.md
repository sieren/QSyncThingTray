QSyncthingTray
=============
#### A OSX Application for Syncthing written in C++

![Travis CI](https://travis-ci.org/sieren/QSyncthingTray.svg?branch=master "Travis CI
Status")


A little status bar for [Syncthing](http://syncthing.net/) on OS X.

Written in C++ with Qt.

![alt text](https://raw.githubusercontent.com/sieren/QSyncthingTray/master/media/qsyncthingtray.png "Logo Title Text 1")

## Features

+ Shows number of connections at a glance.
+ Presents Syncthing UI in a separate view instead of using the browser.
+ [Syncthing-inotify](https://github.com/syncthing/syncthing-inotify) included and starts with program launch to keep track of file changes even faster.
+ Supports authenticated HTTPS connections.
+ Uses OS X Notifications about current connection status.

Is there a feature missing? Open an issue, send me an [email](mailto:info@s-r-n.de) or fork this project and add it yourself.


## How To Use It
QSyncthingTray does not come with Syncthing bundled. Therefore it needs to be downloaded from [Syncthing](http://syncthing.net/).
Once you specifiy the path to the 'syncthing' binary it will automatically spawn syncthing when you run QSyncthingTray.

QSyncthingTray is downloadable in the [Releases](https://github.com/sieren/QSyncthingTray/releases) section here on GitHub.

To start Syncthing at boot:

+ Go to **System Preferences** and **Users & Groups**
+ Drag QSyncthingTray into the **Login Items** list

## Requirements
QSyncthingTray has been targeted for OS X 10.7, however only been tested on 10.10. Feedback is highly appreciated.

## Build & Run
+ Get a recent version of Qt (5.5+)
+ Use either QtCreator, create an XCode Project with the included script (you might need to specify your qmake path) or a regular Makefile
