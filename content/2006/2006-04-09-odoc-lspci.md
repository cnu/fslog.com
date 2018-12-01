---
title: 'ODOC: lspci'

date: 2006-04-09
url: /2006/04/09/odoc-lspci/
categories:
  - ODOC

---
lspci &#8212; List all PCI device information.

Summary:

lspci is a utility for displaying information about all PCI buses in the system and all devices connected to them.

Examples:

> $ lspci &#8212; List all PCI device details in short form.
> 
> $ lspci -v &#8212; List all PCI device details in long form.
> 
> $ lspci -vv &#8212; List all PCI device details in very verbose form.
> 
> $ lspci -vb &#8212; Show PCI device connection in Tree form.
> 
> $ lspci -n &#8212; Show details in raw form like vendor & device code.
> 
> $ lscpi -d 8086: &#8212; Show only Intel&#8217;s PCI devices.
> 
> $ lspci -m &#8212; Show the details in more readable form.
> 
> $ lspci -x &#8212; Show initial PCI configuration details in HEX.
> 
> \# lspci -xxx &#8212; Show whole PCI configuration details in HEX.

Read: man lspci
  
<tags>lspci, pci,linux, odoc, gnu/linux</tags>