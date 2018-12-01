---
title: 'ODOC: useradd'

date: 2006-02-06
url: /2006/02/06/odoc-useradd-2/
categories:
  - ODOC

---
useradd &#8212; Create a new user.

Summary :

useradd creates a new user with specified options like username, home dir, group details, password, etc &#8230;

Example:

> \# useradd usr1 &#8212; Add new user usr1 with default settings.
> 
> \# useradd usr1 -d /home2/usr1 &#8212; Create the new user&#8217;s home dir in /home2
> 
> \# useradd usr1 -e 2005-04-30 &#8212; From 30/4/2005 the user acc will be disabled.
> 
> \# useradd usr1 -f 6 &#8212; After passwd expires, system will allow the user to login for 6 days with a warning to change his passwd.
> 
> \# useradd usr1 -g staff -G student,lect, prof &#8212; Set his initial group as staff and sublimentry group as office, lect, prof.
> 
> \# useradd usr1 -p $1$d8 &#8212; Create the usr1 with the given encrypted password. For No passwd, acc disabled.
> 
> \# useradd usr1 -s /bin/csh &#8212; Set C Shell as the default login shell for the usr1.

Read: man useradd

<tags>odoc, useradd, linux, gnu/linux</tags>