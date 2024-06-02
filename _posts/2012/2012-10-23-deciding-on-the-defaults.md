---
title:       "Deciding on the defaults"
date:        2012-10-23 00:08:51
serie:       [ "A day in an open source project" ]
category:    [ "Ubuntu" ]
tag:         [ "configuration", "defaults", "development", "feedback" ]
---

It's not even a week until UDS-R, and it's time to start planning a new release of Xubuntu – again! Planning isn't just thinking of fun new features, it's also about doing some hard work (and some good guesswork) to give our users the best possible experience.

In this article I will try to give some light into a few less-fun and more-work tasks that the Xubuntu team has to rethink at least in some way with each release: default configuration and application set.

Sensible configuration
----------------------

Creating a configuration that suits your workflow isn't always easy. Creating a configuration that works for hundreds and thousands of people at least in a mediocre way is even harder. Not even talking about fitting their workflow coming from the backbone.

Without any research, there is simply no way to judge how good the defaults are. Organizing a full-scale research for every Xubuntu user is impossible. How do we decide what to ship by default then? How can a small amount of people even know which application or configuration is good for the majority?

All and any configuration has left a "trace" in our previous releases. There's always somebody who thinks the *previous* way was the best. But how do we judge if that user belongs to the majority? If something isn't optimal, should we revert or fast forward? Ultimately, how do we make sure our users get the best user experience and that way, the most of our product?

Honestly, I don't know the answer. Every piece of configuration is an educated guess. While our choices can sometimes mean we will lose some users, we can't build the OS trying to make sure nobody is disagreeing or leaving. Instead, the operating system needs to be going somewhere. Sometimes it's innovative, sometimes it's imitating what the other players are doing and at the same time trying to do it a bit better.

Default applications
--------------------

Choosing the default set of applications isn't something the whole developer community agrees on. The variation in the user community is even broader. People love and hate our default applications. Sometimes they haven't even tried them before purging them. There has to be an objective way to compare applications, right? There is, but it's not trivial.

Simply the task of justifying why a current application is not a good for a default and especially why something else is better can be quite a daunting task. To be able to compare applications, you need to know which features are essential (eg. for what feature is this application being included for), which features are good to have and which features are unwanted.

Once we have found the best application available, we need to make sure we're conducting the testing it needs and that the application fits on the CD image. For example, we had to drop GIMP and Gnumeric from the Quantal release to fit on a CD. We might reintroduce these in later versions if we get more free space, but even then, it doesn't hurt to rethink if these applications really contributed to the core Xubuntu experience so much that they should be reintroduced or if there would be better alternatives – or if we simply want to keep them off our images.

Trying to learn from the mistakes
---------------------------------

We are constantly listening to our users; if a change in the default configuration or applications was a big mistake, we sure hear from it. Fortunately, we haven't had too many bursts of negative feedback yet. Even if we did get a dozen of complaints, is that really the majority? Surely, there's a lot more Xubuntu users. Is it again the vocal minority, or is this a valid complaint and concern?

We hope you will continue to let us know if you think we did a good or bad job. Constructive criticism as well as cheers and thank yous are always welcome.
