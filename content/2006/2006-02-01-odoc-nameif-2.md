---
title: 'ODOC: nameif'

date: 2006-02-01
url: /2006/02/01/odoc-nameif-2/
categories:
  - ODOC

---
nameif &#8212; NAME network InterFaces based on MAC addresses.

Summary :

nameif is used to rename the network interfaces based on MAC addresses. It is useful, when you have more then one network interfaces/cards & you want to specify the name (eth0, .. ) for each interfaces.

Example:

> \# nameif &#8212; Read the config info from /etc/mactab file.
> 
> \# nameif -s &#8212; Same as above. But error messages goto the syslog.
> 
> \# nameif -s eth0 00:0D:87:77:74:5C &#8212; Name the card with specified MAC as eth0 and error goto syslog.

Note:

  1. Nameif should be run before the interface is up, otherwise it&#8217;ll fail.
  2. Format of the /etc/mactab file:
  
    \# Comments
  
    eth0 00:0D:87:77:74:5B
  
    eth1 00:0D:87:78:7D:6B

Read: man nameif

<tags>nameif, odoc, linux, gnu/linux,network</tags>