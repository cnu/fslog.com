---
title: Smartlink Modem in Ubuntu Dapper

date: 2006-07-08
url: /2006/07/08/smartlink-modem-in-ubuntu-dapper/
categories:
  - Distribution
  - Hardware
  - Software

---
This week I had installed [Ubuntu Dapper 6.06][1] and tried really hard at making my SmartLink Internal Modem to work in it. It hadn&#8217;t worked in any other distro other than Debian Sarge. I started with a 64 bit version of Ubuntu, but it didn&#8217;t help. I followed the instructions in Launchpad and configured the modem. So here are the steps that I followed to make my SmartLink modem work in Ubuntu 6.06.

  1. First we need to have a few packages which need to be installed before installing the driver. You need to have build-essential, linux-headers-ARCH (where ARCH is your kernel version and can be found with uname -r in the terminal), fakeroot, module-assistant and debhelper. All these can be installed (with the dependancies) using apt-get.
  2. Then you need to install ungrab-winmodem from the [linmodem website][2]. Just extract it and make; make install to install it.
  3. Download slmodem-2.9.11-20051101.tar.gz from <http://phep2.technion.ac.il/linmodems/packages/smartlink/>
  4. Download sl-modem-daemon\_2.9.10+2.9.9d+e-pre2-5build1\_i386.deb, but don&#8217;t install it yet.
  5. Extract the tar.gz file and type make and then sudo make install in the folder where you extracted it.
  6. Type sudo modprobe slamr
  7. Then install the sl-modem-daemon using `dpkg -i sl-modem-daemon_2.9.10+2.9.9d+e-pre2-5build1_i386.deb` command.
  8. Type `sudo /etc/init.d/sl-modem-daemon restart` to restart the daemon. 
      * This ends the installation part of the modem. Now you can setup your internet connection. 
      * I used wvdial and unusually, the modem redialled every time the ISP showed the Login prompt. So, I put in the Stupid Mode = 1 in the `/etc/wvdial.conf` file.</ol>

 [1]: http://www.fslog.com/2006/06/01/ubuntu-606-lts-released/
 [2]: http://phep2.technion.ac.il/linmodems/packages/smartlink/