---
title:       "Setting up new systems"
date:        2016-09-01 13:47:52
serie:       
category:    [ "Ubuntu" ]
tag:         [ "configuration", "fonts", "laptop", "locale", "Thunderbird" ]
---

In May, I bought a new laptop. In this article, I go through a few of the most essential tweaks I set up with the new laptop.

When possible, I like to customize my system to support my workflow and to make working faster. Once you have customized something and got used to it, there's no going back. This means every time I set up a new system (or an old system again), I have to set up the custom configuration up as well.

Locales
-------

I prefer my interface completely English, but apart from that, I want some locale related things to be set to the Finnish standards.

In **~/.pam\_environment**, I have the following:

`LANG=en_US.UTF-8LC_TIME=en_DK.UTF-8LC_NUMERIC=fi_FI.UTF-8LC_COLLATE=fi_FI.utf8LC_MONETARY=fi_FI.UTF-8LC_PAPER=fi_FI.UTF-8LC_ADDRESS=fi_FI.UTF-8LC_TELEPHONE=fi_FI.UTF-8LC_MEASUREMENT=fi_FI.UTF-8LANGUAGE=enLC_NAME=fi_FI.UTF-8LC_IDENTIFICATION=fi_FI.UTF-8PAPERSIZE=a4`

Thunderbird configuration
-------------------------

I use Thunderbird for all of my mail and feed related activities. However, I don't like the default set of shortcuts. The [Keyconfig extension](http://kb.mozillazine.org/Keyconfig_extension:_Thunderbird) helps me set up my preferred shortcuts and disable shortcuts I don't want to use at all. The most important shortcuts are as follows:

- **B** for Address Book
- **C** for Calendar
- **E** for Edit As New Message
- **F** for Forward
- **W** for (Write) New Message

I use the [Hide Local Folders](https://addons.mozilla.org/en-US/thunderbird/addon/hide-local-folders/) and [Manually sort folders](https://addons.mozilla.org/en-US/thunderbird/addon/manually-sort-folders/) for some fine-grained control over what is shown on my sidepane – and how. I also use some calendars with Thunderbird. The [Lightning](https://addons.mozilla.org/en-US/thunderbird/addon/lightning/) (integrated calendar), [Lightbird](https://addons.mozilla.org/en-US/thunderbird/addon/lightbird/) (standalone calendar UI) and [Provider for Google Calendar](https://addons.mozilla.org/en-US/thunderbird/addon/provider-for-google-calendar/) extensions let me sync my calendars easily.

Finally, I have customized the UI with an **userChrome.css** file, currently holding the following CSS:

`/* do not color folders/servers with new messages blue */#folderTree > treechildren::-moz-tree-cell-text(isServer-true, biffState-NewMail),#folderTree > treechildren::-moz-tree-cell-text(folderNameCol, newMessages-true) {color: inherit !important;}`

Display sizes for fonts
-----------------------

The laptop sports a 13.3" screen with a full HD 1920×1080 resolution. This makes some of the text a bit too small and hard to read, and thus I've done some adjustments to DPI related stuff.

I've set the **Xfce desktop DPI** to **108**.

For Firefox and Thunderbird, setting the value of **layout.css.devPixelsPerPx** to **1.1** both makes the UI a bit more spacy and the text a bit more readable. I usually like small text though, so you might want to increase the value even more.

Scratching the surface
----------------------

Ultimately, these tweaks are just scratching the surface of the level of modidfications I have done already. Not to even talk about modifications and custom workflows I'm using on my desktop...

What kind of modifications do you use?
