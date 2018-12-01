---
title: Bug in Ubuntu Breezy exposes root password

date: 2006-03-14
url: /2006/03/14/bug-in-ubuntu-breezy-exposes-root-password/
categories:
  - Updates

---
In actual there is no user account called root in Ubuntu. A normal user can become root by using the sudo command. But in Breezy, the first [user&#8217;s password is can be easily found][1] by any user reading the file `/var/log/installer/cdebconf/questions.dat`. This [bug is present only in Breezy][2] (5.10) and not in Dapper(6.04) the yet to be released version.
  
There are two packages &#8211; base-config and passwd which needs to be upgraded to prevent this problem. A standard system upgrade will fix this problem.
  
If you are upgrading from 5.10 to 6.04 then you need to upgrade your passwd package to the newest version.
  
<tags>ubuntu, breezy, dapper, root+user</tags>

 [1]: https://launchpad.net/distros/ubuntu/+bug/34606/
 [2]: http://www.ubuntu.com/usn/usn-262-1