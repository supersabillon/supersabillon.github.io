---
layout: post
title: Unit test a callback with QUnit async()
comments : true
tags:
- dev
- programming
- testing
- unit testing
---

When working with callbacks you're usually doing async operations, so to unit test a callback you will need to use QUnit's [async()](http://api.qunitjs.com/async/) method.

`async(): Instruct QUnit to wait for an asynchronous operation.`

So try this:

{% highlight javascript %}
QUnit.test('should invoke callback', (assert) => {
  let done = assert.async();
  let callback = () => {
    assert.ok( true, 'test ok callback invoked' );
    done();
  };
  myFunction(callback);
});
{% endhighlight %}

And that's it! If `myFunction` does its job of invoking the callback then your test will pass.