---
title:       "Simple desktops with Xubuntu"
date:        2015-01-26 01:38:00
serie:       
category:    [ "Ubuntu" ]
tag:         [ "accessibility", "configuration", "Xfce", "Xubuntu" ]
---

In 2012, I wrote an article about [default configuration for an operating system and the challenges involved with it](http://open.knome.fi/2012/10/23/deciding-on-the-defaults/). For a related, but slightly different topic, I thought it would be useful to share some of my experiences in setting up environments for more or less technically limited people.

Please note that this is just a pointer and a suggestion and the needs and wants of real people may and will vary.

Relevant visual elements
------------------------

### Panel

The first thing I would suggest to do is to remove any unnecessary panel applets (and panels, where appropriate). Automatically hidden panels can be really hard to use, especially for those users who have limited experience with mice or other problems that affect hand-cursor coordination. These can vary anywhere from bad eyesight to difficulties with accurate movement or simply having a hard time understanding the concept of a cursor.

What is relevant in the panels for a simple desktop experience? If you are striving for the simplest possible configuration, I would say that you only need launchers for applications, window list of open applications, a clock and a shutdown button with no choice of logout, suspend or other actions. With this setup, I recommend using the confirmation dialog to prevent unwanted shutdown cycles.

When deciding which launchers to show, please remember that you can enable access to the full application menu on right-clicking the desktop. Because of that option, it's not always worth the trouble to try to add a launcher for every application, especially if they are used only rarely. Consider picking ones that users need *dail*y*, weekly* or *monthly*, depending on how much you want to avoid right-clicking.

I believe people that want or need a simple desktop don't want to see anything that they think is irrelevant. This is especially true to indicators, because they use symbols that are more or less hard to understand for a technically limited person.

There are a few exceptions: If you're setting up a laptop that's actually unplugged now and then, you might want to show the battery indicator. If you have a laptop that needs to be used in various locations, you'll want to show the network manager as well. If controlling volume is necessary, you might want to consider whether the sound indicator or shortcut keys (Fn+F*x* in laptops) are the better choice.

### Desktop

In addition to the panel launchers, it's wise to add launchers for the desktop as well along with a shutdown button. Make sure the launchers use generic names instead of application names eg. *Email* instead of *Mozilla Thunderbird*. It's usually wise to bump up the icon and label size up as well. If the users will not run several applications at a time, you can simply drop the panel and only use the desktop icons. If you want to show the clock without a panel, you can use a simple *Conky* setup. Conky is available in the Ubuntu repositories.

### Other accessibility considerations

If the users have problems with their eyesight, there are a few things that can help make the system more usable for them.

The first one is adjusting the font and DPI settings. Bumping up the font size by just one step and increasing the DPI value makes the text more easily readable. Xubuntu has a very legible default font, even in smallish fonts, but it's good to remember you can change the font as well

The other thing you can do is change the window border theme. The default Xubuntu theme is designed to be elegant and keep out of the way, but sometimes this is not ideal. If the user has a hard time seeing where a window ends and the other starts, it might be a good idea to try another window border theme. On the other hand, if too many buttons is the problem – or you simply don't need or want to enable some features – you can remove some of the window buttons as well.

There is also many accessibility configuration options under the *Accessibility tab* in Window Manager Tweaks found in the Settings Manager. The one I tend to turn off is rolling up windows with the mouse wheel. This prevents the accidentally "disappearing" windows.

### Accessibility version of Greybird?

Currently, Greybird, the Xubuntu default theme, ships two window border themes: a regular and a compact one. It has been brought up to discussion by me and others that we should ship an accessibility version as well. This accessibility version would sport bigger window buttons as well as a bigger border to grab for resizing the window.

So far, the accessibility on the drawing board phase and not much has been done yet, as it's currently one of the most low priority items for the development teams of Xubuntu and Shimmer. That being said, all constructive feedback is welcome. Furthermore, if we see a lot of people asking for the accessibility version, it's likely that its priority will be bumped up at least a little.

Smoother user experience
------------------------

Since we are talking about a simple desktop experience, I can assume at least part of our target group is people who don't either understand or want to understand why updating is important or how to install updates. For this reason, I'd simply turn on the automatical security updates but turn off all manual updates.

Depending on the situation, I would make sure *apport* will not pop up and ask to send new bug reports. It's self-evident that bug reports are important, but if the user doesn't understand or want to understand the importance, it's better to turn any reporting that needs user input off. The possibility that these users with the simplest possible desktops would run into bugs that haven't been already found is really rare. Moreover, the possibility of developers getting further information from these users are really slim.

While I don't use autologin myself and can't suggest using it for security reasons, setting it up might save a lot of frustration. But please, only use autologin after a good assessment of the situation and understanding the security considerations related to that.

Manual maintenance needs
------------------------

Even though a system can run smoothly without daily maintenance, manual maintenance is sometimes required. I've been maintaining a few computers for family remotely during the years, and the two tools I've needed the most are an SSH server and remote desktop viewing ability – for which I'm currently using an X11vnc setup.

While SSH is usually fine for most of the regular maintenance, being able to view (and use) the desktop remotely has been an invaluable help in situations where the user can't describe the issue accurately enough via text or voice based communication. This is even more useful if the computer is far from you and you have limited possibilities to access it physically.

Naturally, you need to take security considerations into account when accessing a computer remotely. Making servers listen on unusual ports and securing with them firewalls is highly encouraged.

Summary
-------

There are numerous opinions on the best desktop configuration, both in the look and feel. However, if you are setting a system up for somebody else, you will need to consider how they usually use the computer and how you could support their workflow to make the experience smoother.

Xfce allows a great deal of customizability by default. On top of that, the Xubuntu team has worked to bring the users even more tools that can help them configure their system. The options brought by these alone give you a vast amount of different things you can control. This article is just scratching the surface for even those options. If you want to go deeper, there is always more software on the Ubuntu repositories that can help you set up the system in the way you like it.

If you have other ideas and suggestions for simple and/or accessible desktops, feel free to drop them in the comments. If you write (or have written) a blog article about customizing Xubuntu, especially ones that cover accessbility issues, I'd like to hear back from those as well.

Happy configuring!
