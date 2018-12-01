---
title: 'ODOC: hostid'

date: 2006-02-17
url: /2006/02/18/odoc-hostid-2/
categories:
  - ODOC

---
hostid &#8211; Print the numeric id for the host.

Summary:

It will print a 32-bit hexadecimal numerical identifier for the host machine. Certain product registration procedures use this number to brand a particular user license. The 32-bit quantity happens to be closely related to the system&#8217;s IP address, but that isn&#8217;t always the case.

If your IP address is 192.168.14.155 then your hostid is A8C09B0E.

A8 &#8212; 168
  
C0 &#8212; 192
  
9B &#8212; 155
  
0E &#8212; 14

Example:

> $ hostid &#8212; Print the hostid of the current host.

Read: man hostid
  
<tags>hostid, network, odoc, linux, gnu/linux</tags>