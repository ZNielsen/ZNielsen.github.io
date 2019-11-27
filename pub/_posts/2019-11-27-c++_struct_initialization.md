---
title: "C++ Named Initialization: My Bugbear"
layout: post
tags: [c++]
---

I often lament the lack of named initialization in C++.  It changes how
I design code - if two arguments can be swapped without the compiler
complaining about it, then it's possible to have a runtime bug that can be
difficult to track down.  I love Python's named initialization, but it
appears that C++ is constrained to the not-exactly-foolproof method of
["Just throw some comments on the end of the lines, it will be fine!"][1].
I'm not a fan.

Thankfully, [C++ 20 will come to the rescue][2], bringing
functionality available to C since 1999!  Only 20+ years behind.
Better late than never though, looking forward to having this available.


[1]: https://stackoverflow.com/questions/11516657/c-structure-initialization
[2]: https://en.cppreference.com/w/cpp/language/aggregate_initialization
