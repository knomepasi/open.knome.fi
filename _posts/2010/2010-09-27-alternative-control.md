---
title:       "Alternative control?"
date:        2010-09-27 01:04:28
serie:       
category:    [ "Unaggregated" ]
tag:         [ "keyboard", "VirtualBox" ]
---

For some time, I had a weird problem with *VirtualBox*. The *Ctrl* key was working as *Alt* and the other way around. Madness! This was totally driving me crazy...

Anyway, after a few not-so-serious and a few way-more-serious attempts to fix the issue, I've finally found the solution. In the Xfce Settings Manager, under section Keyboard and tab Layout, there's a check box to either use or not to use system defaults. Apparently, my system default was wrong or this setting was not functioning properly, since as soon as I unchecked the box, VirtualBox seemed to capture the keys right. Hooray!
