---
title: "C++: RVO and auto"
layout: post
tags: [programming, cpp]
---

A quick overview of my day to day learnings about C++.

### RVO - copy/move elision
A conversation came up in one of our code reviews about Return Value Optimization.  This led me to research when and how return value optimization takes place.  [The reference page][cp-elision] contains the key piece of info I was looking for:

> ... The objects are constructed directly into the storage where they would otherwise be copied/moved to.  ...

The rest of the reference page is good to read for when this optimization occurs.

### AAA - Almost Always Auto

We had some debate about when to use `auto` in our code.  The prevailing wisdom (local to our group) was to use it on primitive types or where it was very obvious what the type that was being created was.  I was of the opinion (and of the practice) that `auto` should only be used in
[range-based `for` loops][rb-for-loop]

One of the guys on our team sent out [this blog post][AAA] in response to the conversation.  I found it addressed many of the issues I had with `auto`.  I'll be trying to get in the habit of using it more often.

[cp-elision]: https://en.cppreference.com/w/cpp/language/copy_elision
[rb-for-loop]: https://en.cppreference.com/w/cpp/language/range-for
[AAA]: https://herbsutter.com/2013/08/12/gotw-94-solution-aaa-style-almost-always-auto/
