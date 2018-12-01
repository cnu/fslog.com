---
title: Install Opera on Ubuntu

date: 2006-12-03
url: /2006/12/03/install-opera-on-ubuntu/
categories:
  - Software

---
<img align="left" alt="Opera Logo" id="image310" src="http://www.fslog.com/wp-content/uploads/2006/12/operalogo.jpg" />Though many users prefer Mozilla Firefox, there are people who like Opera for the speed. It has many features that are yet to be seen in Internet Explorer.

The latest version of Opera is 9 and has many unique features that is not yet found in other browsers.

It has a built in Bittorrent downloader, Content blocker(to block images and ads), Widgets &#8211; small web applications, download manager, email client, IRC and many such cool features.

Linux users can also download a client for their distribution. Ubuntu users can get a deb file and install it.

Before it you should install libqt3-mt package. Then download the .deb file and install it. All these three can be done by these commands.

<pre>sudo apt-get install libqt3-mt
wget <a rel="nofollow" title="http://ftp.wayne.edu/opera/linux/902/final/en/i386/shared/opera 9.02-20060919.6-shared-qt en i386.deb" class="external free" href="http://ftp.wayne.edu/opera/linux/902/final/en/i386/shared/opera_9.02-20060919.6-shared-qt_en_i386.deb">http://ftp.wayne.edu/opera/linux/902/final/en/i386/shared/opera_9.02-20060919.6-shared-qt_en_i386.deb</a>
sudo dpkg -i opera_9.02-20060919.6-shared-qt_en_i386.deb</pre>

To get java working go to Tools->Preferences->Advanced->Content-> Check &#8220;Enable Java&#8221;. Click the &#8220;Enable Java&#8230;&#8221; button and enter &#8220;_/usr/lib/jvm/java-1.5.0-sun/jre/lib/i386_&#8221; (for Sun Java) in the new dialog and then click the &#8220;Validate Java Path&#8221; button.