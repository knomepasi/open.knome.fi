---
title:       "Panels disappearing and other frequently asked questions"
date:        2009-07-05 15:57:21
serie:       
category:    [ "Ubuntu" ]
tag:         [ "FAQ", "jaunty", "support", "Xubuntu" ]
---

We give a huge bunch of user support at *\#xubuntu*. After each release, there's a peak for the need of user support. Here's some of the most asked questions after the Xubuntu 9.04 release.

Getting Xubuntu
---------------

### Where can I download Xubuntu?

See <http://xubuntu.org/get> and <http://cdimage.ubuntu.com/xubuntu/releases/9.04/release/>.

### Is there ShipIt service for Xubuntu?

No.

Upgrading and installing
------------------------

### Can I upgrade from (K)Ubuntu 8.10 to Xubuntu 9.04?

Not directly. You can first install the *xubuntu-desktop* meta-package and remove your (K)Ubuntu related packages following the instructions at <http://www.psychocats.net/ubuntu/purexfce>. Now you are on a Xubuntu 8.10 system, and can upgrade to Xubuntu 9.04 normally.

### The installation stops at 15-20%. What's wrong?

You most possibly have too little resources. Try the *alternative CD*.

### What is the difference between the desktop and the alternative CD?

Desktop uses a graphic installer and works as a live CD. You can try it before installing. Alternate uses a text based installer and you don't get to try it first, but it also uses less memory for installing.

### Are Xubuntu and Ubuntu identical?

No. The major difference is the Desktop Environment used; Xubuntu uses Xfce while Ubuntu uses Gnome. However Xubuntu and Ubuntu use the same repositories and base system. Minor differences include different sets of default applications and settings.

### I want ext4 but I don't have that option in the installer. What do I do?

You have to use the alternate CD if you want ext4.

### Why does the Update Manager not have the button to upgrade to Xubuntu 9.04?

You have to install all updates first. If it still doesn't show up, see *Settings &gt; Repositories &gt; Updates* from *Synaptic* and set "Show new distirbution releases" to "Normal releases".

### Can i downgrade from 9.04 to 8.10?

No.

Desktop
-------

### My panels disappeared. How do I get them back?

Press *Alt+F2* and run *xfce4-panel*. See also <https://help.ubuntu.com/community/XubuntuPanels>.

### My desktop icons and files disappeared. How do I get them back?

Press *Alt+F2* and run *xfdesktop*.

### Does Xubuntu 9.04/Xfce 4.6 have a menu editor?

No, it doesn't.

### Can I add Gnome panel applets to my Xfce panel?

Yes you can. Try adding the *XfApplet* applet to your panel.

Drivers
-------

### My resolution is only *X* but I want *Y*! What should I do?

The installer might not have detected your graphics card correctly. Try using a *restricted driver*.

### How can I use (restricted) driver X?

See *Applications &gt; System &gt; Hardware Drivers*.

Sound
-----

### How to use multimedia keys?

Open the *Keyboard settings* (*Applications &gt; Settings &gt; Keyboard*) and open the *Application Shortcuts* tab. Click add and follow the shortcut wizard. The shortcut commands are *amixer sset Master 5%-* for volume down, *amixer sset Master 5%+* for volume up and *mute* for mute.

### I'm having major problems with Pulseaudio. How do I fix it?

Pulseaudio just doesn't work for everybody. You can try if uninstalling it helps; *sudo apt-get remove `--`purge pulseaudio* *gstreamer0.10-pulseaudio* in Terminal or remove both packages from *Synaptic*.

Miscellanous
------------

### Is OpenOffice in Xubuntu?

It's not installed by default, but you can install it from the repositories – just install the package *openoffice.org.*

"My question was not answered here."
------------------------------------

Refer to my previous blog article on [Getting Support](http://open.knome.fi/2009/05/28/getting-support/).
