---
title:       "Fixed keyboard in VBox – again"
date:        2011-06-28 05:25:38
serie:       
category:    [ "Ubuntu" ]
tag:         [ "keyboard", "VirtualBox" ]
---

As [I previously mentioned](http://open.knome.fi/2010/09/27/alternative-control/ "Alternative control?"), I had some problems with left Alt and Control keys being switched with each other. After upgrade to Natty, I was having the same problem, but the same fix didn't work. The quick and a bit dirty solution was the [KeyTweak software](http://webpages.charter.net/krumsick/), which easily remapped the keys inside Windows. No more banging head against the wall (for now)!

I'm actually interested in where this bug is coming from? Is it a problem with Ubuntu, Xfce, the X server, VirtualBox or Windows? The keys work as expected outside VirtualBox (as did they work before the first bugfix as well), but as the solution against the previous bug confirmed, the solution might very well be found outside VirtualBox. The solution for the recurred problem clearly isn't a bugfix but a workaround.

Anybody have any ideas? I'm willing to test and produce any debug information while I still have this bug.

*Edit:* It looks like this bug appears under Vinagre (Remote Desktop Viewer) as well! Oh my!
