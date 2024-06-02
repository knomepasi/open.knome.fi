---
title:       "Terminal color scheme testing"
date:        2012-01-31 15:57:56
serie:       
category:    [ "Ubuntu" ]
tag:         [ "design", "precise", "terminal", "testing", "Xubuntu" ]
---

In addition to other [appearance improvements](https://blueprints.launchpad.net/ubuntu/+spec/other-p-xubuntu-appearance-improvements "Blueprint: Appearance improvements (Launchpad)") for Xubuntu Precise Pangolin, we are creating a new Terminal color scheme to match the window borders of Greybird. It currently looks about this:

\[caption id="attachment\_588" align="aligncenter" width="300"\][![Xubuntu Precise Pangolin proposed terminal color scheme](http://open.knome.fi/files/2012/01/xubuntu-precise-terminal-colors-300x203.png)](http://open.knome.fi/files/2012/01/xubuntu-precise-terminal-colors.png) Xubuntu Precise Pangolin proposed terminal color scheme\[/caption\]

In addition to those who are testing the daily builds, we'd like to have some feedback on the usability of the color scheme. To do this, backup your `~/.config/Terminal/terminalrc` and replace the original file with [this file](http://open.knome.fi/files/2012/01/xubuntu-precise-terminalrc "Xubuntu Precise Pangolin terminalrc") (remember to rename it as `terminalrc` if you are downloading it directly). Note that this file might override some of your terminal settings, which is why you should backup your terminalrc. If you want, you can just replace any lines with *Color* in the original file with the lines from the new terminalrc.

After you've tested it for some time, get back to us at #xubuntu-devel at Freenode or the [Xubuntu developer mailing list](https://lists.ubuntu.com/mailman/listinfo/xubuntu-devel) and give feedback – both positive and negative. Thanks for helping us out!
