---
title: FrostWire – Free Gnutella client

date: 2006-12-17
url: /2006/12/17/frostwire-free-gnutella-client/
categories:
  - Software

---
<img align="left" alt="FrostWire" id="image320" src="http://www.fslog.com/wp-content/uploads/2006/12/64x64frostsphere.png" />FrostWire is a fork of the very popular [LimeWire][1] [Gnutella][2] client. Gnutella is a popular file sharing network. It is a huge network hosting approximately 2.2 million users. It has numerous files ranging from mp3s, movies, ebooks, applications, etc.

FrostWire is a free and open source software without all the nasty nags. It also has a built-in bittorrent client. Here the steps to install FrostWire on your Ubuntu Edgy.First you have to install J2SE Runtime Environment (JRE).

<pre>sudo apt-get install sun-java5-jre sun-java5-plugin</pre>

Then download the frostwire deb file and install it using dpkg.

<pre>wget -c <a rel="nofollow" title="http://www.users.on.net/~stubby/FrostWire-4.10.9-2.i586.deb" class="external free" href="http://www.users.on.net/%7Estubby/FrostWire-4.10.9-2.i586.deb">http://www.users.on.net/~stubby/FrostWire-4.10.9-2.i586.deb</a>
sudo dpkg -i FrostWire-4.10.9-2.i586.deb</pre>

That was so simple. You can run FrostWire by running Applications -> Internet -> FrostWire

 [1]: http://www.limewire.com/
 [2]: http://en.wikipedia.org/wiki/Gnutella