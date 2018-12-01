---
title: 'ODOC: lpstat'

date: 2006-03-05
url: /2006/03/05/odoc-lpstat-2/
categories:
  - ODOC

---
lpstat &#8212; Print CUPS status information

Summary:

lpstat displays status information about the current jobs, and
  
printers. When run with no arguments, lpstat will list jobs
  
queued by the user.

Example:

> $ lpstat &#8212; List jobs queued by the user.
> 
> $ lpstat -a &#8212; Shows the accepting state of all printer queues.
> 
> $ lpstat -d &#8212; Show default printer queue.
> 
> $ lpstat -p &#8212; Shows the printers status.
> 
> $ lpstat -r &#8212; Shows whether or not the CUPS server is running.
> 
> $ lpstat -s &#8212; Shows a status summary
> 
> $ lpstat -t &#8212; Show a detailed status
> 
> $ lpstat -u user1 &#8212; Shows the print jobs queued by user1.
> 
> $ lpstat -v prn1 &#8212; Shows printers & what device they are attached to.

Read: man lpstat

Sorry for not posting for a long time. Actually I was busy this week as we had our culturals in our college. Also my mouse was not working. I guess I will buy a new computer. So, have any of you have any suggestions for my new system? Please comment here.

<tags>odoc, linux, gnu/linux, lpstat, printer</tags>