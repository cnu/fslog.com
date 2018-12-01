---
title: 'ODOC: groupmod'

date: 2006-02-10
url: /2006/02/11/odoc-groupmod-2/
categories:
  - ODOC

---
groupmod &#8212; Modify a group

Summary :

The groupmod command modifies the system account files to reflect the
  
changes that are specified on the command line.

Example:

> \# groupmod -g 600 mygrp &#8212; Change the mygrp Group ID to 600.
> 
> \# groupmod -n mygrp1 mygrp &#8212; Change the mygrp name to mygrp1.

Group informations are stored in /etc/group files.

Read: man groupmod
  
<tags>odoc, groupadd, linux, gnu/linux</tags>