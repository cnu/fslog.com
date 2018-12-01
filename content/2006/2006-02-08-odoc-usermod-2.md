---
title: 'ODOC: usermod'

date: 2006-02-08
url: /2006/02/08/odoc-usermod-2/
categories:
  - ODOC

---
usermod &#8212; Modify a user account

Summary :

The usermod command modifies the system account files to reflect the changes that are specified, like Home dir, password, etc. on the command line

Example:

> \# usermod -d /home2/usr1 usr1 &#8212; Create the new home Dir for usr1 in /home2 & Move old Dir contents to this Dir.
> 
> \# usermod -e 2005-04-30 usr1 &#8212; From 30/4/2005 the usr1 acc will be disabled.
> 
> \# usermod -f 6 usr1 &#8212; After passwd expires, system will allow the user to login for 6 days with a warning to change his passwd.
> 
> \# usermod -g prof usr1 &#8212; Set usr1&#8217;s initial group as prof.
> 
> \# usermod -p $1$d8 usr1 &#8212; Set the new passwd for the usr1
> 
> \# usermod -s /bin/bash usr1 &#8212; Set Bash as the default login shell for the usr1.
> 
> \# usermod -L usr1 &#8212; Lock a user&#8217;s password.
> 
> \# usermod -U usr1 &#8212; Unlock a user&#8217;s password.

Read: man usermod

<tags>usermod, odoc, linux, gnu/linux</tags>