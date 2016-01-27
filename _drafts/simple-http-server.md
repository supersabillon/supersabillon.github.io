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

If you do lots of local development I'm sure you've run into multiple issues when running your site locally using the File protocol [file:///](https://msdn.microsoft.com/en-us/library/aa767731):

* Images with relative paths break
* AJAX requests from local files don't work
* External JavaScript libraries and APIs throw restriction errors

You then may describe these behaviors as bugs, when in fact they are not.

This is why running your site in a local web server is so important, because your site will behave the same way it will out in the wild.

## command-line http server
Why deal with WAMP/MAMP when you can easily use a command line to run a web server?
