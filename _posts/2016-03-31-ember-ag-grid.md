---
layout: post
title: New ember addon&#58; ember-ag-grid
comments : true
tags:
- ember
- emberjs
- ag-grid
- ember-addon
- javascript
---

Happy to announce my first emberjs addon: [ember-ag-grid](https://github.com/supersabillon/ember-ag-grid).

[Ag-Grid](https://github.com/ceolter/ag-grid/) is an excellent javascript data grid library written by [Niall Crosby](https://github.com/ceolter). It is fast, supports filtering, column pinning, sorting, data csv export, it's super simple to use... the list goes on.

I noticed that the author had addons for AngularJS, React and Angular 2 but no addon for Ember. So I decided to create a very simple wrapper of the ag-grid library.

Using this addon you don't have to worry about loading assets or destroying grid to release resources and you can use this simple HTMLBars helper to initialize your grid: `{% raw %}{{ag-grid gridOptions=gridOptions}}{% endraw %}`.

For more info on installation and options check out the [README.md](https://github.com/supersabillon/ember-ag-grid#installation).

