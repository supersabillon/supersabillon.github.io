---
layout: post
title: 'Easy way to remember the difference between .call and .apply'
comments : true
tags:
- javascript
---

The `call` and `apply` methods perform the same thing: they execute a function in the context, or scope, of the first argument that you pass to them.

And the difference is that `apply` lets you invoke the function with arguments as an array; `call` requires the parameters be listed explicitly.

I always had to Google which one was which until I found this somewhere in the interwebs: The A in `apply` is for array, and the C in `call` is for comma.
