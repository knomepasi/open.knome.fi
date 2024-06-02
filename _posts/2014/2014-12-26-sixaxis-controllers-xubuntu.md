---
title:       "Sixaxis controllers with Xubuntu"
date:        2014-12-26 23:20:58
serie:       
category:    [ "Ubuntu" ]
tag:         [ "controllers", "howto" ]
---

During the Christmas time I have traditionally worked on some random projects related to computers or other electronic devices. This year is no different.

The winning project this year was connecting Sixaxis controllers via Bluetooth to my Xubuntu laptop to be able to play some retro games under Dosbox in a less retro way...

Here's a brief overview what you need to do to get them working.

***Please note** that the following steps include **enabling PPA's**, and you are following the instructions **at your own risk**.*

Enable connections via Bluetooth
--------------------------------

To be able to pair and connect the Sixaxis controllers correctly via Bluetooth, you will need to install [QTSixA](http://qtsixa.sourceforge.net/). If you want to use your controllers **via** **USB only,** you might want to **stop here**. The controllers are mostly supported out of the box. More information on the QTSixA website.

The steps you need to take at this point are documented thoroughly on the [Sixaxis page of the Ubuntu community help wiki](https://help.ubuntu.com/community/Sixaxis). Here's a *really brief* recap.

### Install QTSixA

`sudo apt-add-repository ppa:falk-t-j/qtsixasudo apt-get updatesudo apt-get install sixad libusb-dev libusb-0.1-4`

### Pair and connect

To pair the controllers, run `sudo sixpair` when your controller is plugged in. Repeat for each controller.

Naturally, if the controllers are already paired with this machine eg. not used with any other host machine since the last use, you can skip this part.

To connect the controllers, run `sixad --start` and press the PS button (for some time) on each controller when the software tells you to. When the controller vibrates, you are connected!

The sixad daemon captures your bluetooth device and will stop the regular bluetooth activity. You can return to a normal state by running `sixad --restore`. If you wish to, you can set sixad to run on boot so you can always connect your controllers on the fly. More information on this and other configuration options can be found at the official [QTSixA website](http://qtsixa.sourceforge.net/).

Map buttons to keyboard events
------------------------------

If you want to use the controllers to play games that do not have direct support for game controllers like I did, you need to map the controller buttons to keyboard events. For this part, you will need additional software.

As I was doing the research, I read about several applications that allow you to remap buttons. I ended using [AntiMicro](https://github.com/Ryochan7/antimicro) since it seemed easy enough – and *just worked*. Your mileage may vary.

### Install AntiMicro

`sudo apt-add-repository ppa:ryochan7/antimicrosudo apt-get updatesudo apt-get install antimicro`

### Configure to your liking

Once you've done that, run AntiMicro to set the key bindings.

If Antimicro doesn't show you "Sticks" and "DPads" separately, but only two columns of buttons, I recommend running the controller mapping (bottom left). For some reason, this was correctly detected on my desktop, but not on my laptop.

The UI itself is pretty straightforward; when you press a button on the controller, the corresponding UI button is highlighted. To change the key binding, simply press that button and pick a key you wish to bind it to. In some cases, you might not be presented with a virtual keyboard; in these cases, you can get it to appear by pressing the "No key" button. You can even do advanced set up, for example key combos.

Finally, you can save the button profiles for easy access in the future. Remember to keep AntiMicro running as long as you use your controllers.

**Enjoy!**
