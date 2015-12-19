---
layout: post
title: 'Enhance your jQuery plugin with two lines of code'
comments : true
tags:
- javascript
- jquery
- plugin
---

While developing a jQuery plugin I thought about how cool it would be if it had a callback capability, but I wasn't sure if I wanted to write tons of lines of code for a feature that wasn't essential.

Then I did some research and realized it would only takes two lines of code to make this happen.

Assuming you're using [good practices](http://www.codereadability.com/what-are-javascript-options-objects/#settingdefaultvalues) to create your default values:

{% highlight javascript linenos %}
var defaults = {

  // define an empty anonymous function so
  // no need to check if it exists before calling it
  myFancyCallback: function() {},

  // ... rest of settings ...
};
{% endhighlight %}

Then later in the program, let's say for example you need the callback to trigger when a close button is clicked:
{% highlight javascript %}
code goes here
{% endhighlight %}
