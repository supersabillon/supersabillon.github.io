---
layout: post
title: Simple http server
comments : true
tags:
- server
- http
- webdevelopment
- npm
---

If you do lots of local development I'm sure you've ran into multiple issues when running your site locally using the File protocol (file://):

* Images with relative paths break
* AJAX requests from local files don't work
* External JavaScript libraries and APIs do not work as expected

You then may describe these behaviors as bugs, when in fact they are not.

This is why running your site in a local web server is so important, because your site would behave the same way it would out in the wild.

## command-line http server
Why deal with WAMP/MAMP when you can easily use a command line to run a web server?
