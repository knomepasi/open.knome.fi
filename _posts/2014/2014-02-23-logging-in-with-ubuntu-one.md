---
title:       "Logging in with Ubuntu One"
date:        2014-02-23 20:57:48
serie:       
category:    [ "Ubuntu" ]
tag:         [ "Launchpad", "login", "Ubuntu One" ]
---

Since many new contributors have asked about logging in to various Ubuntu-related sites and services and there hasn't been a thorough explanation on what and how, I thought it would be useful to post an article explaining some of the stuff happening in the background.

Note: I am only writing of my own experience and knowledge. I haven't read the source code, or received a technical explanation from anybody who has written, or been involved with setting up the services mentioned, nor do I work for Canonical. Ultimately, your mileage may vary.

Definitions
-----------

[Ubuntu One](https://login.ubuntu.com/) (formerly Ubuntu Single Sign On, or Ubuntu SSO) is the centralized login service that allows you to login to various services. These services include some cloud services, music streaming, mobile app store and more. However, a Ubuntu One account is also needed to access the developer tools and sites like Launchpad, the Ubuntu wikis, Ubuntu Forums, AskUbuntu and more.

[Launchpad](http://launchpad.net/) is the place where a lot of the contributor community cooperation happens. It is used to file bugs, write blueprints, create PPA's, manage translations and much more.

Sources of information
----------------------

The Ubuntu One account will only have limited information of you; to be exact, your name and your email address. You will need to input these when you register for a Ubuntu One account. Whether you have contributed to Ubuntu or not, it's not unlikely to have one.

The Launchpad account requires further information than the information available from Ubuntu One; namely, a username. This is created automatically from your email address, and you can change it later from your Launchpad page, from "Change details", considering you don't have any PPA's enabled.

You can use your existing Ubuntu One account details when logging in to Launchpad. If you or create a new Launchpad account, you will be automatically created a Ubuntu One account that's linked to your Launchpad account.

Sharing information
-------------------

All information from your Launchpad, or any other service, is available for your Ubuntu One account (including your username and team memberships). When you log in to other sites and services with Ubuntu One, you can either decide to share or not share this information. The other sites and services will then determine what kind of access they will give you. This is what causes the most confusion and frustration of new contributors.

For example, the [Ubuntu team wiki](http://wiki.ubuntu.com/) requires you to share a username to be able to attribute each edit correctly. Even if you are able to log in to the team wiki without a Launchpad account, or without sharing the username information, you will be unable to edit pages in this case.

Another example is the [Ubuntu Developer Summit Etherpad](http://pad.ubuntu.com/), which requires a user to be a member of a specific Launchpad group team granting them access. If you have contributed more to the project, it's likely you are a member of that team indirectly via some of your other teams. New contributors who aren't members in many Launchpad teams yet are less likely to even know about this fact. That said, if you are looking for that information, you will need to join the [~ubuntu-etherpad](https://launchpad.net/~ubuntu-etherpad) team; it is moderated so you won't be automatically approved, but anybody applying for that group will be approved without further questions once the moderators do their usual routines.

Setting up accounts
-------------------

**If you have a Ubuntu One account**, [log in to Launchpad](https://login.launchpad.net/+login) with your Ubuntu One credentials. This will create you a Launchpad username and associate it with your Ubuntu One account. You can change your Launchpad username by changing the "name" field in the [Change details](https://launchpad.net/~/+edit) page. This will be your username for all Ubuntu One -related sites and services.

**If you don't have a Ubuntu One account**, the easiest way to create one and associate a Launchpad account with it is to [Create a new Launchpad account](https://login.launchpad.net/+new_account). This will automatically create a Ubuntu One account and guide you through creating the Launchpad account. If you want to change the automatically selected username, go to the [Change details](https://launchpad.net/~/+edit) page.

After you have a Ubuntu One account that has an associated Launchpad account, you are able to log in to other sites and services successfully.

Conclusion
----------

If you contribute to Ubuntu and need to access various services, you will need a Ubuntu One account that has an associated Launchpad account. The associated Launchpad account provides your Ubuntu One account additional information like username or team memberships, which are needed to log in to and work on various sites and services.
