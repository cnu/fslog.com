---
title: 'ODOC: passwd'

date: 2006-02-24
url: /2006/02/24/odoc-passwd-2/
categories:
  - ODOC

---
passwd &#8212; Update a user&#8217;s authentication details.

Summary:

Passwd is used to update a user&#8217;s authentication tokens, like password, lifetime, etc.. Passwd is configured to work through the Linux-PAM API.

Example:

> $ passwd &#8212; Ask new passwd for your account.
> 
> \# passwd user1 &#8212; Ask new passwd for user1&#8217;s account.
> 
> \# passwd -l user1 &#8212; Lock user1 account.
> 
> \# passwd -u user1 &#8212; Unlock user1 account.
> 
> \# passwd -d user1 &#8212; Remove password for user1.
> 
> \# passwd -S user1 &#8212; Show short info about user1&#8217;s password.
> 
> \# passwd -n 30 user1 &#8212; Set 30days as the min lifetime of the user1&#8217;s password.

Note:
  
All new users should read the following topic in the man page
  
A) Protect your password & B) Choose a hard-to-guess password.

Read: man passwd, pam

<tags>passwd, pam, odoc, linux, gnu/linux</tags>