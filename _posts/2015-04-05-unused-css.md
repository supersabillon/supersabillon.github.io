---
layout: post
title: Find unused CSS
comments : true
tags:
- webdevelopment
- frontend
- css
---

If you ever find yourself trying to optimize your page or are just doing routine maintenance, then getting rid of unused CSS rules is one of the easiest thing you could do. Here's what you do:

Open up Chrome and go to your site. Open up the dev tools (Command + option + I) and go to the Audits tab. Run the Web Page Performance audit and that's it. You should get a *Remove unused CSS rules* option, and if you expand it you should see the styles that contain these CSS rules. 

Be careful not to remove styling that's not used on that specific page but maybe in a different part of your site.