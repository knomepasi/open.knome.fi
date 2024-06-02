---
title:       "Give me the endash!"
date:        2011-10-17 23:38:58
serie:       
category:    [ "Ubuntu" ]
tag:         [ "keyboard" ]
---

For some reason, I had some keyboard problems again\* with my clean Oneiric installation. For some reason **AltGr+-** did not produce endash\*\*, like it did in Natty. There is a fix to this, and this time the credits go to *Radomir* and *Jere*. The fix is applied as follows:

1. Run `xmodmap -pke > ~/.Xmodmap` in terminal or TTY.
2. Open ~/.Xmodmap in a text editor, and find a line similar to: `keycode 61 = minus underscore minus underscore hyphen dead_macron`The most important and distinctive mark should be that you have *minus* and *hyphen* in the definition. The keycode number (and the other key bindings) can be different.
3. Replace `hyphen` with `endash` and save the file.
4. Run `xmodmap .Xmodmap` to get the new settings applied right away. If you have chosen to use system settings in the Layout tab of the Keyboard settings in Xfce Settings Manager, this will work automatically on next boot. If you haven't, or if there is something else weird going on, you might want to add the command to your autostart.

\* The previous problem with Ctrl and Alt being switched head-by-head in VirtualBox disappeared with Oneiric. \*\* Endash is a longer dash which is used when denoting a scale like "13–15 year old boys".
