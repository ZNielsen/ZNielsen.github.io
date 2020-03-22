## A Success Story for UnitTests (yes, in _CAL_!!)

I am currently putting the C++ cals through the ringer as much as I am able.  During this process, I needed to make some tweaks to trim tail cal to integrate it with the python cals that run later.  As a part of this change, I modified the return type of a function.  All was good and it would have worked perfectly for my intended purpose.  I didn't think the change would affect the cal.  However, when attempting to compile, the unit test caught a corner case that happens as the cal is wrapping up.  My type change had inadvertently truncated a value so the cal would loose precision!  Because this doesn't happen during the main part of the cal loop (and because it has been a bit since I've messed with Trim Tail Cal), I had completely missed it during my visual inspection.  The Unit Test saved me.  I was easily able to rework my new change to fix the issue, but it would have taken who-knows-how-long to track down the issue if the cal had started failing.  

Unit Tests.  They help.  Even Cal.


