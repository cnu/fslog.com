---
title: 'ODOC: procinfo'

date: 2006-02-26
url: /2006/02/26/odoc-procinfo-2/
categories:
  - ODOC

---
procinfo &#8212; Display system status gathered from `/proc` folder

Summary:

procinfo gathers system data from the /proc directory and prints it nicely formatted on the standard output device.

Example:

> $ procinfo &#8212; Show MEM,CPU Usage and IRQ details.
> 
> $ procinfo -f &#8212; Run in Full screen mode and update will happen for every 5 Sec.
> 
> $ procinfo -n.1 &#8212; Run in Full screen mode and update for every .1 sec (Run with highest-priority).
> 
> $ procinfo -m &#8212; Show info about modules and device drivers.
> 
> $ procinfo -d &#8212; For memory, CPU times, paging, swapping, disk, context and IRQ status.
> 
> $ procinfo -F /dev/tty9 &#8212; Redirect output to tty9.

Read: man procinfo
  
<tags>procinfo, odoc, linux, gnu/linux</tags>