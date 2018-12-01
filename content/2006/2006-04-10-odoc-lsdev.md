---
title: 'ODOC: lsdev'

date: 2006-04-10
url: /2006/04/10/odoc-lsdev/
categories:
  - ODOC

---
lsdev &#8211; Display information about installed hardware

Summary:

lsdev gathers information about your computer&#8217;s installed hardware from the interrupts, ioports and dma files in the /proc directory, thus giving you a quick overview of which hardware uses what I/O addresses and what IRQ and DMA channels.
  
This program only shows the kernel&#8217;s idea of what hardware is present, not what&#8217;s actually physically available.

Examples:

> $ lsdev

Read: man lsdev
  
<tags>lsdev, odoc, linux, gnu/linux,kernel</tags>