---
title: Deluge Bittorrent client for Linux

date: 2006-12-02
url: /2006/12/02/deluge-bittorrent-client-for-linux/
categories:
  - Software

---
<img align="left" alt="deluge logo" id="image308" src="http://www.fslog.com/wp-content/uploads/2006/12/deluge192.png" />In windows I used to have uTorrent for downloading my torrents. Under Linux I searched for a nice software which doesn&#8217;t take too much system resources. Atlast I found [Deluge][1] which is written in Python and has a very easy to use interface just like uTorrent.

It shows detailed statistics about the torrent you are downloading, multiple torrents download using the same interface, even a built-in search engine.

If you are using debian/ubuntu, Deluge can be apt-getted easily. Just add the followind lines to your sources.list file. There are two repositories, you can add either one of them.

<pre>deb http://deluge.mynimalistic.net/apt dapper main</pre>

<pre>deb http://espergreen.com/apt dapper main</pre>

After adding it, run `sudo apt-get install deluge`

It requires python-libtorrent_0.4.0 but all the dependencies will be handled by apt-get automatically (why else do you use apt-get).

There are packages for Gentoo and Arch Linux. You can also [download][2] the package by visiting the trac page. Ubuntu Forums host a [support forum][3] for Deluge. You can ask for help there.

This new version 0.4 supports plugins and various plugins are available for monitoring the network, showing the graphs, monitoring CPU usage.

 [1]: http://deluge-torrent.org/
 [2]: http://deluge-torrent.org/trac/wiki/Downloads
 [3]: http://ubuntuforums.org/forumdisplay.php?f=172