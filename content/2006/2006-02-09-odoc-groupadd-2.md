---
title: 'ODOC: groupadd'

date: 2006-02-09
url: /2006/02/09/odoc-groupadd-2/
categories:
  - ODOC

---
groupadd &#8212; Create a new group

Summary :

The groupadd command creates a new group account using the values
  
specified on the command line and the default values from the system.

Example:

> \# groupadd newgrp &#8212; Create a new group
> 
> \# groupadd -g 600 newgrp &#8212; Create newgrp with specified Group ID.
> 
> \# groupadd -f newgrp &#8212; Force flag. Don&#8217;t show error message.

Read: man groupadd

<tags>odoc, linux, gnu/linux</tags>