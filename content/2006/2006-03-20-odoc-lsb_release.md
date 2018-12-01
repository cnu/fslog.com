---
title: 'ODOC: lsb_release'

date: 2006-03-19
url: /2006/03/20/odoc-lsb_release/
categories:
  - ODOC

---
lsb_release &#8212; Show Linux Standard Base and Distribution info.

Summary:

If the installation is LSB compliant, the `/etc/lsb-release` file should contain the LSB\_VERSION field and other optional fields like DISTRIB\_ID, DISTRIB\_RELEASE, DISTRIB\_CODENAME, DISTRIB_DESCRIPTION.

lsb_release will read the above config file and show the details in different format. It is useful command to find your distribution informations.

Example:

> $ lsb_release &#8212; Show the LSB version number.
> 
> $ lsb_release -i &#8212; Display the distributor ID or Name.
> 
> $ lsb_release -d &#8212; Display the single line text description of the distribution.
> 
> $ lsb_release -r &#8212; Display the release number of the distribution.
> 
> $ lsb_release -c &#8212; Display the distribution code-name.
> 
> $ lsb_release -a &#8212; Display all of the above information.
> 
> $ lsb_release -s &#8212; Show only field values, not the filed name.
> 
> $ lsb_release -ds &#8212; Show only field values, not the filed name.
> 
> $ lsb_release -as &#8212; Show in short format.

Read: man lsb_release
  
<tags>lsb_release, distribution, distro, linux+distro, linux, gnu/linux</tags>