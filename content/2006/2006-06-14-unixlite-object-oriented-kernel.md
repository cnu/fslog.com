---
title: 'UnixLite: Object Oriented Kernel'

date: 2006-06-14
url: /2006/06/14/unixlite-object-oriented-kernel/
categories:
  - Distribution
  - Software

---
<img align="right" id="image261" alt="Unix Lite" src="/uploads/2006/06/unixlite.png" />[UnixLite][1] is a lightweight unix/linux compatible operating system written in C++. Just like Linux, it is just a kernel &#8211; written from scratch and most of the part is written in C++. However the library used by UnixLite comes from [uClibc][2] and applications running comes from the [GNU][3] project. UnixLite kernel implements some <a target="_blank" href="http://www.unixlite.org/status.html">frequently used system calls of linux</a>, furthermore, it is binary compatible with linux, and some GNU software have been ported to unixlite.

Due to the small size(the kernel is made up of about 20000 lines of code) and the object oriented programming using the c++, the kernel becomes more modular and easy to understand.

Technical Features:

  * Support paging and flat memory model, nearly same as linux
  * Implements about 80 posix compliant system call
  * Binary compatible with linux
  * Able to run bash/gcc, and some other common UNIX tools
  * Very rudimentary TCP/IP support, able to run a simple http server
  * Very small, about 20000 lines of code
  * Written in c++, highly modular and extensible
  * Minix&#8217;s 32-bit file system

 [1]: http://www.unixlite.org/
 [2]: http://www.uclibc.org/
 [3]: http://www.gnu.org/