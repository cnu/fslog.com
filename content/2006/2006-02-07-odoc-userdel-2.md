---
title: 'ODOC: userdel'

date: 2006-02-07
url: /2006/02/07/odoc-userdel-2/
categories:
  - ODOC

---
userdel &#8211; Delete a user account and related files

Summary :

The userdel command modifies the system account files, deleting all entries that refer to login. userdel will not allow you to remove an account if the user is currently logged in. You must kill any running processes which belong to an account that you are deleting.

Example:

> \# userdel usr1 &#8212; Remove the usr1 account entry details. Home Dir will not be removed.
> 
> \# userdel -r usr1 &#8212; Remove the account entries, Home Dir and Mail Spool of the usr1.

Read: man userdel

<tags>odoc, userdel, linux, gnu/linux</tags>