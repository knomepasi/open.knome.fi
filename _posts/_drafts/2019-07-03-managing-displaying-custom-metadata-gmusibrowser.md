---
title:       "Managing and displaying custom metadata in gmusibrowser"
date:        2019-07-03 01:31:23
serie:       
category:    [ "Unaggregated" ]
tag:         [ "gmusicbrowser" ]
---

I've used gmusicbrowser as my media manager for many years. Even though the gmusicbrowser codebase is quite stale (the last stable release was made in 2015), it still delivers a great experience without any glaring bugs. One of the reasons why I like it over other alternative is its customizability and modularity with both the visual and the functional side of things.

In this article I want to highlight the customizability in gmusicbrowser regarding managing and displaying custom metadata.

What kind of metadata to store and where?
-----------------------------------------

My music files are more than just music to me; they are sort of a carefully curated collection. While you can store a lot of different data in the default fields, I want to add more to be able to make more connections between the different pieces on the collection and more importantly, add to the metadata that is meaningful for me.

### Custom fields

The custom fields feature allows you to create fields of different types and attach them to each track separately. I personally find the labels field type most useful. My personal favorite is the "flags" field type. Flags are essentially common labels which you can freely create yourself but which are also easily updatable from the UI without requiring to open any dialogs.

Some examples of custom fields I'm using or have used before are (field type flags unless otherwise mentioned):

- **Country** (flags)**.** This fields loosely tracks the originating country for the track; in most cases there's just one value to this field, but in some cases – with multinational groups – it can have multiple values, one per originating country of the musicians appearing.
- **Original** (string). This field is usually used to note the original album or single where the track first appeared or in case it's a previously officially unreleased, the year it was recorded in. In some rare cases this field includes the original track name if it originally appeared with a different name. An good example of this is the album *Everything Will Be Alright Tomorrow* from Faithless, which sports instrumental versions of the tracks from the album *No Roots*.
- **People** (flags). Almost like "featuring", but for situations when the featuring artist isn't officially listed. I try to have at least all guest vocalists listed here.
- **Reference** (flags). A reference to a musician, group or other entity that makes sense. For example, this can be used with cover versions to reference the artist that made the original track popular.

### Plain text files

In addition to the custom fields feature, I want my collection to be mostly accessible without gmusicbrowser as well. I've decided to use plain text files which will be read and displayed by a custom plugin. This allows very easy and universal read access to the files. Additionally, it lets me avoid touching individual media files when updating data for the whole album.

The information that I decided to store outside the gmusicbrowser database and the tags are album-related metadata and lyrics. Each media directory (in most cases, the album directory) has files for the album-related data and lyrics. For the lyrics, the file contains lyrics for all of the tracks in the album separated with *ini-style* section headers.

Displaying the custom fields
----------------------------

One of the obvious problems with all predefined layout is that they are very generic and do not have any mechanism to display custom metadata in a sensible way – at least for me. For this reason, I've made two set of modifications. First, I've created some custom songtree columns to show some of the data in a more compact way. Second, I've created a context pane plugin for displaying more data at once.

### Updated title column for Songtree

I created a modified version of the *Title* column which in addition to the title shows the following information:

- <span style="text-decoration: underline;">***Artist*, if it is different from the *Album artist*.** These are both standard fields, but I feel like this is essential enough to mention. This is very useful especially with compilations or albums with featuring singers.</span>

<span style="text-decoration: underline;">The column has different formatting variations depending on which fields have values, but generally, this information is displayed in a smaller font size and/or gray text in order to separate it from the actual track titles.</span>

### Plugin for the context pane

While the Songtree modifications were a huge improvement over the old title-only display, it's clear that they have their own restrictions. Some of the tracks can easily have part of the extra information disappear when the column isn't wide enough. Additionally some of the data isn't really track-specific; it's rather related to the album as a whole. The natural place for this data is the context pane; it can hold a lot of data at once and it would only show data for the current track, avoiding unnecessary repetition.

This lead me to create a new context pane plugin "Context". The plugin shows both the basic track information nicely formatted as well as all of the custom metadata I've added either in the custom fields or the plain text files.

The conclusion
--------------

At the end of the day, supporting any kind of custom metadata is useless unless the fields are populated for each and every track in the collection – correctly. I've definitely went ahead too fast and backed out when I've realized actually populating the metadata for a specific metadata field would be way too much work.

However, as I see it, metadata can improve your music listening experience and increase the depth of the collection.
