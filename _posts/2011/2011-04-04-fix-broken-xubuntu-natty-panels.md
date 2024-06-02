---
title:       "How to fix broken Xubuntu Natty panels?"
date:        2011-04-04 13:03:47
serie:       
category:    [ "Ubuntu" ]
tag:         [ "natty", "panel", "Xfce", "Xubuntu" ]
---

Since many people have had problems with the Xubuntu Natty panels due to [bug #747137](https://bugs.launchpad.net/ubuntu/+source/xubuntu-default-settings/+bug/747137) (which is fixed now), we thought it would be nice to tell how to fix the panels. Here goes:

1. Log out from Xfce
2. Open a TTY (eg. press Ctrl+Alt+F1)
3. Log in in the TTY
4. Run 'rm -rf $HOME/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml'
5. Log out from the TTH ('logout' should do the trick)
6. Get back to TTY7 (Ctrl+Alt+F7) or if that doesn't work, TTY8 (Ctrl+Alt+F8)
7. Log in and your panels should be now fixed and have the default settings

Note that this problem with the panels only appears on systems already running Natty, new installs shouldn't be affected.
