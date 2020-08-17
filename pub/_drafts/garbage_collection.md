---
title: Why I Don't Like Garbage Collection
layout: post
tags:
---

Why GC is good, as I understand it

- Non-deterministic
- Joel Spolskey's Law of leaky abstractions.

Garbage collection helps you bootstrap quickly. You incur a bit of technical debt (not managing your own memory) to save some time in programming and early debugging (in the beginning) so you can get the product out faster. If you don't scale or need best in class performance, you will probably never need to worry about GC. It becomes exactly as promised -- something that works magic in the background. However as soon as you have to think about garbage collection, that technical debt has come due.

Some links to big problemes where GC was the main culprate
- Dropbox and Go
- Instagram and Python
- Discord moving to Rust??

