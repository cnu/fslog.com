---
title: 'ODOC: ifconfig'

date: 2006-01-28
url: /2006/01/28/odoc-ifconfig-2/
categories:
  - ODOC

---
ifconfig &#8211; CONFIGure a \`network&#8217; InterFace

Summary :

**ifconfig** is used to display/configure the kernel-resident network interfaces. It is used at boot time to set up interfaces.

Example:

> $ ifconfig &#8212; Show info abt the active network interfaces like IP Address, MAC address, Subnet mask, and status.
> 
> $ ifconfig -a &#8212; Show the status of active and inactive interfaces.
> 
> \# ifconfig eth0 down &#8212; Deactivate/Shutdown the eth0 interface.
> 
> \# ifconfig eth0 up &#8212; Activate the eth0 interface.
> 
> \# ifconfig eth0 192.168.1.100 netmask 255.255.255.0 up &#8212; Activate an interface with specific IP address.
> 
> \# ifconfig eth0:0 192.168.1.101 netmask 255.255.255.0 broadcast 192.168.1.255
> 
> \# ifconfig eth0:1 192.168.1.102 netmask 255.255.255.0 &#8212; Creating alias for eth0, ie Assign more than one IP address to eth0.
> 
> \# ifconfig eth0 arp &#8212; Enable the use of the ARP protocol on eth0.
> 
> \# ifconfig eth0 -arp &#8212; Disable the use of the ARP protocol on eth0.
> 
> \# ifconfig eth0 promisc &#8212; Enable the promiscuous mode on eth0.
> 
> \# ifconfig eth0 hw ether 09:08:07:06:05:04 &#8212; Change eth0 MAC address.
> 
> \# ifconfig eth0 mtu 1412 &#8212; Change Max Transfer Unit of eth0.

NOTE:

  * Deactivate the interface before changing the IP/MAC.
  * Note down the original MAC, Otherwise Reboot needed to get the original MAC Address.
  * Some command sequence needs super user permission.

Read : man ifconfig

<tags>ifconfig, network, odoc, linux, gnu/linux</tags>