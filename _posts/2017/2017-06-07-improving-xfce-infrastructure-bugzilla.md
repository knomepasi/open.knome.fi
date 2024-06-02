---
title:       "Improving the Xfce infrastructure: Bugzilla"
date:        2017-06-07 23:55:21
serie:       
category:    
tag:         [ "website", "Xfce" ]
---

Bug management is a vital part of any open source project. Today I'm happy to introduce you to yet another project which aims to improve the Xfce infrastructure – you guessed it – the [Xfce Bugzilla](https://bugzilla.xfce.org/)!

The project to improve the Xfce bug management started quite some time ago. The first tasks in this were unrelated to the infrastructure; the team has done some work to clean up old bugs as well as triaging newer ones. Tasks like that can become extremely tedious if the tools are constantly slowing you down.

To try to remedy this situation we started a project to improve the look and feel of Bugzilla. In addition to just a general facelift we also ended up reorganizing bits here and there and even touch some functionality. I specifically want to highlight a few parts of the project:

- **Make bug filing easier and faster than before.** We've streamlined the bug filing process by removing one unnecessary page load and a click but also by doing a big reorganization in the bug filing page.
- **Make bug handling easier and faster than before.** In addition to a revamp for the bug filing procedure, the individual bug report pages have had a big update as well; information is now more clearly organized and the long bug description and comments have been brought much closer to the top of the page. We have also merged the status and resolution fields to let you choose the right combination with less clicks – and make it obvious which combinations are possible...
- **Allow using search filters on-the-fly.** Whenever you are on a search result page with any filters, you can remove them individually from the search. You can now also click the product, component and assignee fields to add additional filters.
- **Highlight bug statuses.** This is a smaller update, but we're now using color-coded boxes for bug statuses anywhere they are shown. This should both help users digest information and see where work needs to be done.

Today, we're finally at the point where we are quite happy with the changes and are ready to make them the default for the Xfce Bugzilla – all users using the default theme have been converted to the new Xfce skin and templates related to this skin. If you have specifically selected any other theme, you will be still using that; if you want to see the new theme, please go change your preferences.

We hope you like the new improvements and that they can make your life easier. As always, if you find any weirdness or bugs with the new skin and templates, file them in Bugzilla against the [Bugzilla product on Xfce Bugzilla](https://bugzilla.xfce.org/buglist.cgi?component=General&list_id=35566&product=bugzilla.xfce.org&resolution=---). *Please note that this is not the correct place for bugs about Bugzilla itself – a good way to find out whether something is affecting the Xfce skin and related templates is to check the functionality with another skin enabled.*
