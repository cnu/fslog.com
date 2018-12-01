---
title: Ubuntu Linux Installation Guide

date: 2005-10-24
url: /2005/10/23/ubuntu-linux-installation-guide-2/
categories:
  - Distribution
  - Software
  - Tutorial

---
After reading the [live CD article][1], I think you must be interested in Linux. Live CDs are useful to try out linux, but as it runs from the CD, it isn&#8217;t as fast as a installed version. Also you can&#8217;t save any files to your harddisk.
  
So you think it is time to switch over to installed version of your favourite GNU/Linux. Here is a guide to do how&#8230;

I am going to write this guide with [Ubuntu][2] 5.10 (breezy) in mind and so you need to [download the CD][3] or [order for free][4].

**First stage**

  * Put the CD in your CDROM drive and boot off it (change your BIOS configuration)
  * After the installer starts, press enter to start.
  * Choose your language, country and keyboard layout. The installer detects some hardware.
  * Now configure your network, if you are on one.

**Partitioning the harddisk**
  
This is the most important step and be careful as you can lose your data. Please take a backup of important data.
  
You have got two choices here

  * Automatically partition an entire disk &#8211; will erase the harddisk and install only Ubuntu.
  * Manually partition the disk. Resize your disk so that you get atleast 4GB for your root (/) partition and 256MB for your swap.
  * After finishing with the partition, save it and the installer formats your disk.
  * Then the base system is configured and then the packages are copied to the disk

**Installing the boot loader**
  
The bootloader is used to boot into many different operating systems by means of a menu. The installer automatically detects your OS and installs the GRUB loader.
  
After this, remove your disk and reboot.

**Second stage**

  * After rebooting, you need to configure your timezone.
  * Enter your full name, username and password. There is no root account in Ubuntu and there is a nice explanation for it.
  * If you have not setup your network, then you can setup your PPP to have a dial-up account for internet.
  * All the set of packages required for a basic desktop installation will be setup.
  * Now you can login to the system with your username/password.

I have written this guide using the [Installation guide from the Ubuntu wiki][5]. Hope it was useful for newbies. You can also try this book [Beginning Ubuntu Linux][6] by Keir Thomas to know more about Ubuntu Linux.
  
If at all you encounter any problems, please feel free to post here. Also tell me how good I am at writing such articles?

<div>
  Tech Tags: ubuntu linux <a rel="tag" href="http://technorati.com/tag/gnu/linux">gnu/linux</a> <a rel="tag" href="http://technorati.com/tag/installation">installation</a> <a rel="tag" href="http://technorati.com/tag/install">install</a> <a rel="tag" href="http://technorati.com/tag/i386">i386</a> <a rel="tag" href="http://technorati.com/tag/linux+install">linux+install</a> <a rel="tag" href="http://technorati.com/tag/partition">partition</a> <a rel="tag" href="http://technorati.com/tag/" />
</div>

 [1]: http://www.fslog.com/2005/10/20/gnulinux-live-cd/
 [2]: http://www.ubuntu.com
 [3]: http://download.ubuntu.com "Download Ubuntu"
 [4]: http://shipit.ubuntu.com "Order Ubuntu for free"
 [5]: https://wiki.ubuntu.com/Installation/I386 "Ubuntu Installation"
 [6]: http://www.amazon.com/exec/obidos/ASIN/1590596277/freesoftwareb-20?creative=327641&camp=14573&link_code=as1 "Begining Ubuntu Linux"