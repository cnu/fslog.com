---
title: Boot Linux faster with Open BIOS

date: 2006-09-06
url: /2006/09/06/boot-linux-faster-with-open-bios/
categories:
  - Hardware
  - Software

---
If you want faster boot/reset times on your Linux box, you should consider switching over to [OpenBIOS][1]. OpenBIOS can save the time wasted by proprietary BIOS legacy support for MS-DOS and other unnecessary functions.
  
The proprietary BIOSes typically found in off-the-shelf PCs and boards often account for more than half of total boot time. And, much of this time is spent loading drivers and compiling information useful to legacy OSes such as DOS, but largely useless and redundant when using a modern OS such as Linux, which tends to do its own hardware probing, and load its own hardware drivers.

This problem can be avoided by replacing the proprietary BIOS by OpenBIOS. Open implementations can be configured to perform only the required initialisation tasks before booting the OS.

Another approach is to use linux itself to initialise its hardware. The [LinuxBIOS][2] loads a small kernel directly on the ROM. This can be easily attained as current hardware has 1-2MB of flash ROM onboard.

 [1]: http://www.openfirmware.org/
 [2]: http://www.linuxbios.org/