---
title:       "Preparing for Xubuntu 18.04"
date:        2017-10-24 09:55:22
serie:       [ "A day in an open source project" ]
category:    [ "Ubuntu" ]
tag:         [ "artwork", "brand", "community", "documentation", "LTS", "website", "Xubuntu" ]
---

Xubuntu 17.10 was just released, but planning for Xubuntu 18.04 – the next long-term support (LTS) release – began quite some time ago. For our users, LTS releases mostly mean a system that is going to be more stable and supported for longer. For us contributors, this means a bunch of things.

As a repercussion of the longer support cycle and the sought out stable nature of the LTS releases, we do not want to introduce (too many) new components, libraries or other technical changes, as each change has regression potential. This is also a delicate balancing act between getting bugs fixed but keeping enough things as they are.

The LTS releases are also kind of an flagship for Xubuntu – they are the recommended releases for most users and while we can land stable release updates (SRU) to fix bugs and other major flaws, the scope of changes is limited. Since the next LTS release will be released two years later, we want to get things right.

For contributors – particularly us non-developer kinds – this is an ideal situation to revisit and improve artwork and documentation amongst other things. Here are some things I am going to be working on for the next months to get the new LTS look and feel more polished than the previous one.

Branding – or, updated logo
---------------------------

In an [earlier article](https://open.knome.fi/2017/10/20/refreshing-xubuntu-logo/) I wrote about the refreshed Xubuntu logo – the why and the what. Here's the other what.

Practically this change means we will have to touch every package with Xubuntu branding and make sure they use the updated logo. For the most part this is trivial, but landing the changes requires time and some co-operation from the team.

We will also need to make sure the new logo lands on the official website, all related sites and social media before the release – ideally before the first milestone release. Last but not least, we need to communicate this change to our official vendors and provide them the new logo as soon as possible so they can start updating their products.

Wallpapers
----------

As with any release, the LTS release also needs a wallpaper. This needs to be drafted, proposed and polished. The process usually takes from a few days to a few weeks. We'll also want to land the wallpaper relatively early to be able to fix potential issues with it before release.

The Xubuntu team has organized a community wallpaper contest for the last two LTS releases and it's very likely we will be organizing one for 18.04 as well. I was not completely satisfied in how we ran the contest last time, and I've started a discussion to review our policies already, as getting comments from the team can sometimes be quite slow. While the community wallpaper package does not serve any defaults, we will need to end the contest well before the related freezes to double check license issues (like attribution) and leave enough time for uploading them.

Documentation
-------------

Even if there is no need to rewrite sections – or the whole documentation – this time around, there are several tasks for the documentation team as well.

First of all, it's time to refresh both the installer slideshow and the website feature tour. Nothing has been planned yet, but both of these are at least two years old and in need of a facelift – both visually and in terms of content.

We haven't had to touch the documentation much in a long time because the main software selection and features have stayed the same. On the other hand this means that the documentation might be somewhat stale. This might be hard to identify – and possibly even harder to get stale sections refreshed – but we definitely should have a look at our offering before the release. To do this, we need to consider the following questions:

- Does the documentation provide a good overview of the system for new users?
- Does the documentation help users get started?
- Does the documentation answer the most common questions?
- Does the documentation help get the most common (non-hardware specific) issues solved?
- Does the documentation help more advanced users – including those that are familiar with other Linux operating systems but not Xubuntu?
- Is all information in the documentation up-to-date?
- Does the documentation need extending in any area?
- Can we extend the documentation in a useful way without making it too verbose?

But wait! There's more!
-----------------------

My work item list for Xubuntu 18.04 doesn't end here. You can find all of the registered work items on our [status tracker](https://dev.xubuntu.org/).

It's worth noting that not all of the work items in the status tracker have an assignee. This means we are still looking for people who can help us make Xubuntu 18.04 a greater release than its predecessors. *Maybe you can volunteer and pick up a work item or two?*

In addition to the work items, there are a few other activities that we need help with:

- **Test.** By testing the daily and milestone ISOs you can help us make sure there aren't (so many) annoying bugs in the final release.
- **Take part in the community wallpaper contest**. This is not open yet, but once it is, submit your work. You can win and get some swag as well as your work included in an official Xubuntu release!
- **Submit us ideas for improving and extending our documentation.** I mentioned some of the questions we have to ask ourselves with the documentation. Can you help us answer these and even work with us on the writing and proofreading?

Even these tasks just scratch the surface of what needs to be done – and what can be done.

Get your hands dirty *now* and [read more about getting involved with Xubuntu](https://xubuntu.org/contribute/), subscribe to the [Xubuntu development discussion mailing list](https://lists.ubuntu.com/mailman/listinfo/xubuntu-devel) and join our development IRC channel [\#xubuntu-devel](irc://chat.freenode.net/xubuntu-devel) which is active on most days.
