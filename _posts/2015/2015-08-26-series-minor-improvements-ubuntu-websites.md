---
title:       "A series of minor improvements for Ubuntu websites"
date:        2015-08-26 16:41:47
serie:       
category:    [ "Ubuntu" ]
tag:         [ "gist", "website" ]
---

In addition to using developer documentation (see [A compact style for jQuery API documentation](http://open.knome.fi/2015/08/26/compact-style-jquery-api-documentation/)), people who work with communities need to use community and communication related websites. The bigger the community, the more tools it needs.

In a large community like Ubuntu, the amount of maintenance is big and the variety of platforms is huge. On top of these, many of the website aren't directly maintained for the community (which has both good and bad sides). For these reasons, it's sometimes hard and/or slow to get updates landed for the CSS files for the websites.

While workarounds aren't ideal, at least we can fight the problematic styles with modern technology. That said, I've created a gist for a [Stylish style that provides some minor improvements for some ubuntu.com websites](https://gist.github.com/knomepasi/22e5998bca83f53463b9).

Currently, the style brings the following improvements:

- The last line of the chat is completely shown in [Ubuntu Etherpad](http://pad.ubuntu.com/) pads
- <del>Images and code blocks aren't overlapping the content section in [Planet Ubuntu](http://planet.ubuntu.com/), avoiding horizontal scrollbars</del> *fix is in production!*
- In the [Ubuntu wiki](https://wiki.ubuntu.com/), list items do not have a large bottom padding, making the lists more readable
- Also in the wiki, tables are always full width but not too wide, keeping them aligned nicely

If you are constantly hitting other annoying styling issues on the Ubuntu websites, leave me a comment and I'll see whether I can update the gist with a workaround. However, **please report the bugs and issues for concerned maintaining parties as well**, so we can stop using these workarounds as soon as possible. Thank you!
