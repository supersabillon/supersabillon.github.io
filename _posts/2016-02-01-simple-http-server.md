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

## command-line http server

You could use an application like XAMPP/MAMP to create a web server, but why when you could easily use a command line instead?

The [http-server](https://www.npmjs.com/package/http-server) package from npm is what you need to quickly start a web server with this command:

`http-server -o`

Run this on your root directory, and use the `-o` option to immediately open a browser window pointing to this location by default: `http://localhost:8080`.

Check the page [https://www.npmjs.com/package/http-server](https://www.npmjs.com/package/http-server) for installation and more options.
