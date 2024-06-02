---
title:       "Getting some WordPress plugins out to public"
date:        2012-01-17 12:06:01
serie:       
category:    [ "Shimmer Project", "Ubuntu" ]
tag:         [ "development", "WordPress" ]
---

Finally, there is a public repository for some of my [WordPress](http://wordpress.org/) plugins, and more is to follow. For the impatient, the repository is in [my Github, under the name WordPress-plugins](https://github.com/knomepasi/WordPress-plugins/).

Getting these plugins published was not a simple task. Some of them needed – and some of them still need – quite heavy code review, and some even need near complete rewriting! For example, the *Simple Planet* plugin not only uses the new Widget class now, but it's also using Simplepie instead Magpie, of which latter is still working, but deprecated in WordPress.

Plugins already in the repository
---------------------------------

- **Interactive Images**, formerly known as ImgCapt. With Interactive Images, you can upload images and add user-readable notes to them. See example on the [Shimmer for gmusicbrowser](http://shimmerproject.org/project/gmusicbrowser/) -page. To see the current issues with the plugin, see the [Interactive Images issues in Github](https://github.com/knomepasi/WordPress-plugins/issues?labels=Interactive+Images&sort=created&direction=desc&state=open&page=1).
- **One Year Earlier**, formerly known as LastYear. A very simple plugin that fetches an article from a year ago and shows its title and excerpt with a "More"-link as a widget.
- **Simple Planet**, formerly known as myPlanet. Another simple plugin that loads *n* newest articles from the feeds listed in the widget properties.

Plugins to be added to the repository
-------------------------------------

- **Compact &amp; Chronological**, formerly known as Yearly Archives. This is a really simple plugin that shows the chronological archive in a more compact way. See for yourself in the [Search &amp; Browse](http://open.knome.fi/?s=) -page at this website! This is most probably the most widespread plugin I've written, and it only needs a quick review before ending in the repository.
- **Photoslider**, formerly known as PicSlide, which is used in several sites. There are some parts that work as supposed, but while the plugin is relatively mature, I need to set some feasible defaults as well as add per-widget/shortcode -settings and probably extend it with some more options, like transition type. Once the plugin is cleaned up a bit, I will upload it to the repository and continue hacking on it. I am already tracking [issues for Photoslider in Github](https://github.com/knomepasi/WordPress-plugins/issues?labels=Photoslider&sort=created&direction=desc&state=open&page=1).
- **Projects Catalog 2.0**, which is the plugin running the [Shimmer Project](http://shimmerproject.org/) project listings. Before uploading to the repository, the plugin still needs some review, and some parts will probably need to be rewritten, since we plan doing some bigger updated for the Shimmer site.

There is more to come?
----------------------

In addition, I have a plugin adding extra headers in emails describing the rationale of the message (eg. `X-WordPress-Rationale: comment-moderation` for messages that asks the user to moderate comments) that I think should be in the core, efficiently adding a rationale for *every* type of email sent. I will pursue getting this added in the core when I have more time on my hands.

There is some odds and ends around all of my WordPress-installations, and I need to go through that. Some of the stuff is strictly work-related and must stay *work-only*, but some of it might be available to publishing – and maybe even useful for somebody...

In the following weeks, I need to look at the statistics plugins the [WordPress plugin directory](http://wordpress.org/extend/plugins/) can offer to me. Unless I find something suitable, I might end up writing a simple plugin myself.

Now, go check out the brand-new [WordPress-plugins repository](https://github.com/knomepasi/WordPress-plugins/), file any issues and stay tuned for more!
