---
title: 'ODOC: eject'

date: 2006-04-18
url: /2006/04/18/odoc-eject/
categories:
  - ODOC

---
eject &#8212; Eject the removable media

Summary:

Eject allows removable media (like CD-ROM, Floppy, Tape, JAZ, ZIP) to be ejected under software control. The command can also control some multi-disc CD-ROM changers, the auto-eject feature supported by some devices, and close the disc tray of some CD-ROM drives.

Examples:

> $ eject &#8212; Eject the default device, mostly CD.
> 
> $ eject -v &#8212; Same as above and show more info.
> 
> $ eject /dev/cdrom &#8212; Eject CD using device file name.
> 
> $ eject -t &#8212; Close the drive tray.
> 
> $ eject -vt &#8212; Same as above and show more info.

Read: man eject
  
<tags> eject, linux, odoc, gnu/linux</tags>