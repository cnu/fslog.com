---
title: Ubuntu Popularity Contest

date: 2006-07-30
url: /2006/07/30/ubuntu-popularity-contest/
categories:
  - Distribution
  - Software

---
Ubuntu has a package called [Popularity Contest][1] (popcon), where you can vote on your popular, most-used application every week. It is fully automated and once configured, it takes care of the rest. This information will help the developers to make decisions over which packages should be promoted and which should be in standard installs.

To set it using the command:

`$sudo dpkg-reconfigure popularity-contest`

You can send the information through HTTP or via EMail. I have set it up through HTTP. The results is updated in [popcon.ubuntu.com][2].

 [1]: http://packages.ubuntu.com/popularity-contest
 [2]: http://popcon.ubuntu.com/