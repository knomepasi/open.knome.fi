---
title:       "Hiding backup files in Thunar"
date:        2011-09-05 23:40:28
serie:       
category:    [ "Ubuntu" ]
tag:         [ "natty", "Thunar", "Xfce" ]
---

There *was* one feature in the new Thunar with GIO (since Xubuntu 11.04 Natty) that I didn't like. It was stubbornly showing backup files (\*~). I asked the Thunar developer [Jannis Pohlmann](http://gezeiten.org/) today if there is a solution/workaround for that, and there definitely is!

Close Thunar, add the line `MiscShowBackup=FALSE` at the end of your `~/.config/Thunar/thunarrc` and launch Thunar again and you're not seeing the backup files anymore. What a relief. Thanks Jannis!

On a sidenote, I've finally started making decent, serious backups of my (Open Source) work. The rsync-based script works better than I could have ever imagined. Thanks go to Marko for *that*.
