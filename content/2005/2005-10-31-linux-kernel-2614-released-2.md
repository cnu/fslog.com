---
title: Linux Kernel 2.6.14 released

date: 2005-10-31
url: /2005/10/31/linux-kernel-2614-released-2/
categories:
  - Software
  - Updates

---
[Linux kernel][1] 2.6.14 was released after two months of development.
  
Here are some new features added to the new kernel.

  * HostAP &#8211; HostAP is one the most popular 802.11 device drivers for linux. It works with cards utilizing the Prism 2/2.5/3 chipset and support Host AP mode, which allows a wireless card to perform all the functions of an access point.
  * FUSE &#8211; Filesystem in USEr space provides a simple interface for userspace programs to export a virtual filesystem to the linux kernel. FUSE also aims to provide a secure method for non privileged users to create and mount their own filesystem implementations.
  * Linux port of the Plan9&#8217;s 9P protocol &#8211; 9P, or the Plan 9 Filesystem Protocol, is a network protocol developed for the Plan 9 distributed operating system as the means of connecting the components of a Plan 9 system (site).
  * Relayfs &#8211; Basically relayfs is just a bunch of per-cpu kernel buffers that can be efficiently written into from kernel code. These buffers are represented as files which can be map&#8217;ed and directly read from in user space. The purpose of this setup is to provide the simplest possible mechanism allowing potentially large amounts of data to be logged in the kernel and &#8216;relayed&#8217; to user space.

There are many more [added features to the new kernel][2].

<div>
  Tech Tags: linux <a rel="tag" href="http://technorati.com/tag/gnu/linux">gnu/linux</a> kernel <a rel="tag" href="http://technorati.com/tag/linux+kernel">linux+kernel</a> <a rel="tag" href="http://technorati.com/tag/kernel+2.6.14">kernel+2.6.14</a> <a rel="tag" href="http://technorati.com/tag/FUSE">FUSE</a> <a rel="tag" href="http://technorati.com/tag/Relayfs">Relayfs</a> <a rel="tag" href="http://technorati.com/tag/Plan9">Plan9</a> <a rel="tag" href="http://technorati.com/tag/9p">9p</a> <a rel="tag" href="http://technorati.com/tag/HostAP">HostAP</a>
</div>

 [1]: http://www.kernel.org/
 [2]: http://wiki.kernelnewbies.org/LinuxChanges