---
title: 'ODOC: lsusb'

date: 2006-04-14
url: /2006/04/15/odoc-lsusb/
categories:
  - ODOC

---
lsusb &#8212; List all USB devices

Summary:

lsusb is a utility for displaying information about all USB buses in the system and all devices connected to them.

Examples:

> $ lsusb &#8212; List all USB device details in short form.
> 
> $ lsusb -v &#8212; List all USB device details in long form.
> 
> $ lsusb -vv &#8212; List all USB device details in very verbose form.
> 
> $ lsusb -t &#8212; Show USB device hierarchy as a tree.

Note:

  * lsusb will collect all USB device info from `/proc/bus/usb`
  * List of all known USB IDs are available in `/usr/share/hwdata/usb.ids`

Read: man lsusb
  
<tags>usb,lsusb, linux, odoc, gnu/linux</tags>