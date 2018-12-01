---
title: 'ODOC: groupdel'

date: 2006-02-11
url: /2006/02/12/odoc-groupdel-2/
categories:
  - ODOC

---
groupdel &#8212; Delete a group

Summary :

The groupdel command modifies the system account files, deleting all entries that refer to group.

Example:

> \# groupdel mygrp &#8212; Remove all entries about the mygrp.

Note:

  * The named group must exist.
  * You may not remove the primary group of any existing user. You must remove the user before you remove the group.

Read: man groupdel
  
<tags>odoc, groupdel, linux, gnu/linux</tags>