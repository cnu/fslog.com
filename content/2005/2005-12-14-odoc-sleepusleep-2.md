---
title: 'ODOC: sleep/usleep'

date: 2005-12-14
url: /2005/12/14/odoc-sleepusleep-2/
categories:
  - ODOC

---
Sorry I was busy for the two days and couldn&#8217;t post here. And my rescheduled exams start from 16th Dec till 27th Dec.

sleep/usleep &#8212; Sleep for a specified amount of time

Summary :

Sleep will introduce a delay for a specified seconds (Seconds may be an arbitrary floating point number). usleep sleeps some no of micro-seconds (default is 1).

Examples :

> $ sleep 6 &#8212; Sleep for 6 Seconds.
> 
> $ sleep 6s &#8212; Sleep for 6 Seconds (Default).
> 
> $ sleep 6m &#8212; Sleep for 6 Minutes.
> 
> $ sleep 6h &#8212; Sleep for 6 Hours.
> 
> $ sleep 6d &#8212; Sleep for 6 Days.
> 
> $ sleep 10.5 &#8212; sleep for 10.5 Seconds.
> 
> $ usleep 200 &#8212; Sleep for 200 micro Seconds.

Sleep may NOT give a very accurate result on many machines.
  
Read : man sleep, usleep

<div>
  Tech Tags: <a href="http://technorati.com/tag/odoc" rel="tag">odoc</a> linux <a href="http://technorati.com/tag/gnu/linux" rel="tag">gnu/linux</a> <a href="http://technorati.com/tag/sleep" rel="tag">sleep</a> <a href="http://technorati.com/tag/usleep" rel="tag">usleep</a>
</div>