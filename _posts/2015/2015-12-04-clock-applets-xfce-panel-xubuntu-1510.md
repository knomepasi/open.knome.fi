---
title:       "Clock applets in the Xfce panel in Xubuntu 15.10"
date:        2015-12-04 20:21:46
serie:       
category:    [ "Ubuntu" ]
tag:         [ "applet", "panel", "Xfce", "Xubuntu" ]
---

Both Xfce and Xubuntu have had new releases relatively lately. In a way or another, this has resulted in an issue with Xubuntu 15.10 release: the *Orage* clock doesn't show a transparent background even if it is set to show one. (Upstream bug in Xfce: [11915](https://bugzilla.xfce.org/show_bug.cgi?id=11915).)

**Don't be afraid!** Instead of using the Orage applet, you can use the *DateTime* and *Clock* applets to get a transparent background - and while they itself do not allow for changing the color of the text in the applet, you can work around that with a *.gtkrc-2.0* file in your home directory. Here's how.

Set up the applets
------------------

To set up the applets, simply add the DateTime and/or Clock applets to your panel. You can control the format in which the time/date is shown in the applet via their preference dialogs found from their right-click context menus.

Bear in mind, if you wish to have two different clocks in the panel, we will be using the regular panel foreground (text) color for DateTime (white for Greybird) and modify the text color for the Clock applet in the steps below.

Modify the Clock applet color
-----------------------------

To modify the Clock applet foreground color, we will need to make a modification in a theming file. The best way to do this is to use the per-user config file, found at *~/.gtkrc-2.0*. If you don't have this file, simply create one.

The code snippet to modify the Clock applest text color is the following:

`style "panel-clock-custom"{fg[NORMAL]    = "#66CCCC"fg[PRELIGHT]    = "#66CCCC"fg[ACTIVE]    = "#66CCCC"text[NORMAL]    = "#66CCCC"text[PRELIGHT]    = "#66CCCC"text[ACTIVE]    = "#66CCCC"}widget "Xfce*Panel*clock*"    style "panel-clock-custom"`

In this snippet, we're setting the foreground color for all the Clock applets to a certain turquoise – <span style="color: #66cccc;"> #66CCCC </span> – which compliments the 15.10 wallpaper well.

You can substitute this hex color value with any other that fits your needs.

The end result
--------------

For me, the end result looks like this:

![Xfce panel clock applets](http://open.knome.fi/files/2015/12/xfce-panel-clock-applet.png)

Have fun modifying your own!
