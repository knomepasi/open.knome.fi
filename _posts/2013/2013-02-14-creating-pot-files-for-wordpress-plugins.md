---
title:       "Creating .pot -files for WordPress plugins"
date:        2013-02-14 14:09:28
serie:       
category:    [ "Ubuntu" ]
tag:         [ "translation", "WordPress" ]
---

Since I've gone through the hassle myself, I thought I'd save your time and tell you how to easily create .pot-files, or translation template files, for WordPress plugins.

Long story short, the command that supports all non-deprecated WordPress translation functions or semantically speaking, gettext keywords, is:

`xgettext -o OUTPUT.pot -L PHP -k__ -k_e -k_n:1,2 -k_x:1,2c -k_ex:1,2c -k_nx:4c,1,2 -kesc_attr_-kesc_attr_e -kesc_attr_x:1,2c -kesc_html__ -kesc_html_e -kesc_html_x:1,2c -k_n_noop:1,2 -k_nx_noop:4c,1,2 *.php`

You might want to add the `--no-wrap` argument depending on your needs. After running the script, go edit OUTPUT.pot and edit the information in the header.

In the foreseeable future, I'm going to finish a simple script that automatically updates the .pot -files for plugins as well as edits the header files automatically based on the plugin information on the main PHP file. The script will be available in [my WordPress -repository on GitHub](https://github.com/knomepasi/WordPress/). Until that, happy hacking on WordPress and translations!
