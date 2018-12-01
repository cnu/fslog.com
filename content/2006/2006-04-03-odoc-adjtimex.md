---
title: 'ODOC: adjtimex'

date: 2006-04-03
url: /2006/04/03/odoc-adjtimex/
categories:
  - ODOC

---
adjtimex &#8211; Display/Set the kernel time variables.

Summary:

This program gives you raw access to the kernel time variables, like clock tick, frequency, offset, PPL Time constant, etc.

Examples:

> $ adjtimex -p &#8212; Print current kernel time values.
> 
> \# adjtimex -w &#8212; Provide time details and ask the user to approximate the accuracy.
> 
> \# adjtimex -c &#8212; Periodically (10Sec) compare the system clock with the CMOS clock values and give suggestions.
> 
> \# adjtimex -t 100001 &#8212; Set the no of mSec that should be added to the system time for each kernel tick interrupt.
> 
> \# adjtimex -f -408033 &#8212; Set the system clock frequency offset.

Read: man adjtimex
  
<tags>adjtimex, linux, gnu/linux, odoc</tags>