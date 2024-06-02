---
title:       "Preparing responsive design for Xubuntu"
date:        2014-11-25 16:49:04
serie:       
category:    [ "Ubuntu" ]
tag:         [ "blog", "documentation", "Paperspace", "website", "Xubuntu" ]
---

As some of you might know, [I was appointed as the Xubuntu website lead](https://lists.ubuntu.com/archives/xubuntu-devel/2014-November/010459.html) after taking a 6-month break from leadership in Xubuntu.

Since this position was passed on from [Lyz](http://princessleia.com/) (who is by the way doing fantastic job as our marketing lead!), I wouldn't have wanted to be nominated unless I could actually bring something to the table. Thus, the [xubuntu-v-website blueprint](https://blueprints.launchpad.net/ubuntu/+spec/xubuntu-v-website) lists all the new (and old) projects that I am driving to finish during the Vivid cycle.

Now, please let me briefly introduce you to the field which I'm currently improving...

Responsive design!
------------------

In the past days, I have been preparing responsive stylesheets for [the Xubuntu website](http://xubuntu.org/ "Xubuntu"). While Xubuntu isn't exactly targeted at any device that itself would have a great need for fully responsive design, we do think that it is important to be available for users browsing with those devices as well.

Currently, we have *four stylesheets* in addition to the regular ones. Two of these are actually useful even for people without small-resolution screens; they improve the user experience for situations when the browser viewport is simply limited.

In the first phase of building the responsive design, I have had three main goals. Maybe the most important aspect is to avoid horizontal scrolling. Accomplishing this already improves the browsing experience a lot especially on small screens. The two other goals are to make some of the typography adjust better to small resolutions while keeping it readable *and* keeping links, especially internal navigation, easily accessible by expanding their clickable area.

At this point, I've pretty much accomplished the first goal, but still have work to do with the other two. There are also some other visual aspects that I would like to improve before going public, but ultimately, they aren't release-critical changes and can wait for later.

For now, the new stylesheets are only used in the staging site. Once we release them for the wider public, or if we feel like we need some broader beta testing, we will reach for people with mobile (and other small-resolution) devices on the [Xubuntu development mailing list](https://lists.ubuntu.com/mailman/listinfo/xubuntu-devel) for testing.

If you can't wait to have a preview and are willing to help testing, show up on our development IRC channel #xubuntu-devel on Freenode and introduce yourself. I'll make sure to get a hold of you sooner than later.

### What about Xubuntu documentation?

The Xubuntu documentation main branch has responsive design stylesheets applied already. This change have yet to make it to any release (including the development version), but will land at least in Vivid soon enough.

Once I have prepared the responsive stylesheets for the [Xubuntu online documentation](http://docs.xubuntu.org/) frontpage, I will coordinate an effort to get the online documentation to use the responsive design as soon as possible. Expect some email about this on the development mailing list as well.

While we are at it... Paperspace
--------------------------------

On a similar note... Last night I released the responsive design that I had been preparing for quite some time for Paperspace, or in other words, the WordPress theme for this blog (and the other blogs in this domain). That said, if you see anything that looks off in any browser resolution below 1200 pixels wide, be in touch. Thank you!
