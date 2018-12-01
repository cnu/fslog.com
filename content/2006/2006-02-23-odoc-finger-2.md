---
title: 'ODOC: finger'

date: 2006-02-23
url: /2006/02/23/odoc-finger-2/
categories:
  - ODOC

---
finger &#8212; User information lookup program.

Summary:

finger will lookup and show information about users in the local or remote system.

Example:

> $ finger &#8212; Show currently logged on user&#8217;s info.
> 
> $ finger user1 &#8212; Show info about the user1.
> 
> $ finger -s &#8212; Show more info about the currently logged on users.
> 
> $ finger -l &#8212; Show all info about the users in multi-lines.
> 
> $ finger @host2 &#8212; Show all current logged on users info.
> 
> $ finger user2@host2 &#8212; Show info about user2 on host2.

Note:

  * User can add his/her plans in ~/.plan and projects details in ~/.project file. Finger will show this in output.
  * Remote host should run fingerd to support remote fingering.

Read: man finger

<tags>finger,odoc, linux,gnu/linux</tags>