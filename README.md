OpenNoteScanner
===============

[![Build Status](https://travis-ci.org/ctodobom/OpenNoteScanner.svg)](https://travis-ci.org/ctodobom/OpenNoteScanner)

This little application provides a way on scanning handwritten notes and printed documents.

It automatically detect the edge of the paper over a contrastant surface.

When using the [printed special page template](https://github.com/ctodobom/OpenNoteScanner/raw/master/Page%20Templates/A4%20with%202%20pages.pdf) it automatically detects the QR Code printed on the bottom right corner and scans the page immediately.

After the page is detected, it compensates any perspective from the image adjusting it to a 90 degree top view and saves it on a folder on the device.

It is also possible to launch the application from any other application that asks for a picture, just make sure that there is no default application associated with this action.

Usage
-----

See the [FAQ](FAQ.md).


Screenshots
-----------

[![screenshot1](http://i.imgur.com/1MDisD3m.jpg)](http://imgur.com/a/ypytF/embed#0)
[![screenshot1](http://i.imgur.com/ksvmOlym.png)](http://imgur.com/a/ypytF/embed#3)
[![screenshot1](http://i.imgur.com/Ayy8GGgm.jpg)](http://imgur.com/a/ypytF/embed#1)
[![screenshot1](http://i.imgur.com/tzMLas3m.jpg)](http://imgur.com/a/ypytF/embed#2)

Requirements
------------

Because of the version of OpenCV that is used in the project it needs to run on Android 5.0 (lollipop) or newer.

In order to capture and manipulate images Open Note Scanner depends on having the OpenCV Manager application installed. If not installed Open Note Scanner will ask to download it from https://github.com/ctodobom/OpenCV-3.1.0-Android or from Google Play Store.


How to Install
--------------

Open Note Scanner is available for simplified installation on [Google Play Store](https://play.google.com/store/apps/details?id=com.todobom.opennotescanner), from [Amazon App Store](http://www.amazon.com/Claudemir-Todo-Bom-Open-Scanner/dp/B01EUAU924) and also from [F-Droid Android Open Source Repository](https://f-droid.org/repository/browse/?fdid=com.todobom.opennotescanner).

[<img alt="Get it on Google Play" height="60" src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png" />](https://play.google.com/store/apps/details?id=com.todobom.opennotescanner&utm_source=global_co&utm_medium=prtnr&utm_content=Mar2515&utm_campaign=PartBadge&pcampaignid=MKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1)
[<img src="https://f-droid.org/badge/get-it-on.png"
    alt="Get it on F-Droid"
    height="60"/>](https://f-droid.org/repository/browse/?fdid=com.todobom.opennotescanner)

**Disclaimer:** Google Play version is ad-supported.

Binary APK file is available [directly from GitHub in the releases section](https://github.com/ctodobom/OpenNoteScanner/releases) of the project.

Instructions for building
-------------------------

### Android Studio

Import the project from GitHub using File -> New -> Project from Version Control -> GitHub, fill the URL https://github.com/ctodobom/OpenNoteScanner.git

It will ask for a base directory, normally AndroidStudioProjects, you can change it to your preference.

After this the Open Note Scanner can be built.


### Command Line

Go to your base folder and import it using ```git```:

```
$ git clone https://github.com/ctodobom/OpenNoteScanner.git
```

This should import the Open Note Scanner repository in OpenNoteScanner folder

You need to point the environment variable ```ANDROID_HOME``` to your Android SDK folder and run ```gradle``` to build the project:

```
$ cd OpenNoteScanner
$ export ANDROID_HOME=~/android-sdk-linux
$ ./gradlew assembleRelease
```

Instructions for Contributing
-------------------------
If you're new to open-source, we recommend you to checkout our [_Contributing Guidelines_](https://github.com/ctodobom/OpenNoteScanner/blob/master/CONTRIBUTING.md) and [Setup Guidelines](https://github.com/ctodobom/OpenNoteScanner/blob/master/SETUP_GUIDELINES.md). Feel free to fork the project and send us a pull request.

History
-------

I've started this app on a brazilian holyday "extended weekend" based on the fact that I was unable to find any open source application that does this job. I was mainly inspired on the RocketBook Wave closed source application.

I really do not know if I will extend more the application, but I am writing bellow some objectives to make it better.

Roadmap
-------

* enhance the image gallery of scanned documents
* register a share action in order to obtain documents already pictured through standard camera apps
* implement automatic action based on the RocketBook Wave marking of the page

Donations
---------

My job is on enterprise servers administration and some development consulting. I do collect money from my customers. I am well paid for that.

For being part of open source projects and documenting my work here I really do not charge anything. I am trying to avoid any type of ads also.

If you think that any information you obtained here is worth of some money and are willing to pay for it, feel free to send any amount through paypal or bitcoin.

| Paypal | Bitcoin |
| ------ | ------- |
| [![](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=X6XHVCPMRQEL4) |  <center> [![](http://api.qrserver.com/v1/create-qr-code/?color=000000&bgcolor=FFFFFF&data=bitcoin%3A1H5tqKZoWdqkR54PGe9w67EzBnLXHBFmt9&qzone=1&margin=0&size=200x200&ecc=L)](bitcoin:1H5tqKZoWdqkR54PGe9w67EzBnLXHBFmt9)<br />[1H5tqKZoWdqkR54PGe9w67EzBnLXHBFmt9](bitcoin:1H5tqKZoWdqkR54PGe9w67EzBnLXHBFmt9)</center> |

In order to fund the development of Open Note Scanner, since version 1.0.36 when downloaded from Google Play store the app will show ads on some screens and will also allow for donation through Google Play in-app purchase. There is no difference on the features available from Google Play version and F-Droid releases.


Contributing
------------

If you have any idea, feel free to fork it and submit your changes back to me.

Thanks
------

### Contributors

As an open source application, contribution are always welcome.

Most translations contributions are listed on [CONTRIBUTORS.md file](https://github.com/ctodobom/OpenNoteScanner/blob/master/CONTRIBUTORS.md) and code contributors are listed on [the Changelog file](https://github.com/ctodobom/OpenNoteScanner/blob/master/CHANGELOG.md) and [the commits history](https://github.com/ctodobom/OpenNoteScanner/commits)

Other people helped submitting [Issue Reports](https://github.com/ctodobom/OpenNoteScanner/issues) and giving info through the [Telegram Group](https://t.me/OpenNoteScanner). Their help is appreciated as well.

### External code

This application wouldn't be possible without the great material produced by the community. I would like to give special thanks to the authors of essencial parts I've got on the internet and used in the code:

* [Android-er / GridView code sample](http://android-er.blogspot.com.br/2012/07/gridview-loading-photos-from-sd-card.html)
* [Android Hive / Full Screen Image pager](http://www.androidhive.info/2013/09/android-fullscreen-image-slider-with-swipe-and-pinch-zoom-gestures/)
* [Adrian Rosebrock from pyimagesearch.com for the excellent tutorial on how to handle the images](http://www.pyimagesearch.com/2014/09/01/build-kick-ass-mobile-document-scanner-just-5-minutes/)
* [Gabriele Mariotti / On how to implement sections in the RecyclerView](https://gist.github.com/gabrielemariotti/e81e126227f8a4bb339c)


License
-------

Copyright 2016 - Claudemir Todo Bom

Software licensed under the GPL version 3 available in GPLv3.TXT and
online on http://www.gnu.org/licenses/gpl.txt.

Use parts from other developers, sometimes with small changes,
references on autorship and specific licenses are on individual
source files.
