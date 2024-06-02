---
title:       "A compact folderpane with Thunderbird 3"
date:        2010-05-20 00:57:18
serie:       
category:    [ "Unaggregated" ]
tag:         [ "design", "folderpane", "Thunderbird", "Xubuntu" ]
---

On my posts earlier ([part 1](http://open.knome.fi/2009/10/05/a-compact-thunderbird-folderpane/) and [part 2](http://open.knome.fi/2009/10/16/a-compact-thunderbird-folderpane-revision-2/)) I was fiddling with the Thunderbird 2 folderpane. It was time to migrate to Xubuntu Lucid, and now I'm pretty much supposed to be using Thunderbird 3. Sadly enough, the default TB3 folderpane is even worse than the TB2 default, and the userChrome -fixes were not compatible with the new folderpane. It's time to open your toolbox and start the journey towards a compact *Thunderbird 3* folderpane.

This is my "All Folders" -view with the default Thunderbird 3 folderpane style.

[![](http://open.knome.fi/files/2010/05/tb3_folderpane_default.png "Default Thunderbird 3 folderpane")](http://open.knome.fi/files/2010/05/tb3_folderpane_default.png)

There's no hope that I am able to see all of my folders at once with the default style. The font size is also quite big, smaller will work for me. My first contact with TB3 leaves me a bit confused, because there is so much going on with all the folder icons. *This takes way too much space*, I'm thinking.

Another thing I dislike in the new default folderpane is the fact it misses the *tree lines*. Fortunately getting them back is well documented, so no worries about that.

My general experience for searching documentation from the web or live support from IRC for tweaking the folderpane is not that good. Too many times I was getting my earlier blog entries as the top 5 search results when trying to find documentation or maybe even examples. The #thunderbird IRC support channel is somewhat unresponsive whenever you pop in there – I might be asking hard and/or weird questions, but you pretty rarely even see anyone saying anything. If I was asking the wrong channel, I of course expect somebody point me to the right direction. *Come on*, Mozilla community!

Anyway, in addition to those issues mentioned, I also played around a bit with the overall feel of the folderpane and tried to make mail reading a nice task rather than a confusing one. These include some nice background coloring as well as shrinking the icons. I think I even made some progress in contrast to the TB2 folderpane tweaks.

The tweaks are still *work in progress*, but here's a screenshot.

[![](http://open.knome.fi/files/2010/05/tb3_folderpane_wip.png "A compact=")](http://open.knome.fi/files/2010/05/tb3_folderpane_wip.png)

You can see that some of the folders do not handle padding correctly (yet). There's also a few other glitches, like the Trash folders, which seem to be visible on TB boot, but disappear when you hover the folderpane.

Here's the [userChrome.css](http://open.knome.fi/files/2010/05/userChrome.css) as well as [envelope.png](http://open.knome.fi/files/2010/05/envelope.png) for showing the envelope symbol for the folders that have unread mail. The envelope icon is from the default Thunderbird 3 icon theme, but at least for now I had to split it out from *folder-pane.png* to be able to show the icon correctly.

To hide the *Local Folders*, I used the [Mail Tweak -extension](http://mailtweak.mozdev.org/).
