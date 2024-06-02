---
title:       "Fuzzy fonts in Firefox 18? No more!"
date:        2013-02-05 12:58:29
serie:       
category:    [ "Ubuntu" ]
tag:         [ "Firefox", "fix" ]
---

Since I upgraded to Firefox 18, I've had blurry fonts on some sites, including Twitter and YouTube. Today I looked a bit into the problem, and found a solution in the Firefox Support forum.

In *about:config*, edit keys in the following way:

1. Set **layers.acceleration.force-enabled** to **true**
2. Set **layers.acceleration.disabled** to **false**

After doing that, restart Firefox and you're ready to go.

Thanks for *juanbaez* for the tip!

If you don't want to edit your configuration, I read that this is fixed in Firefox 19 as well. Downgrading to Firefox 17 reportedly works as well.
