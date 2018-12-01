---
title: Install Flash Player 9 Beta on Ubuntu Edgy

date: 2006-11-28
url: /2006/11/28/install-flash-player-9-beta-on-ubuntu-edgy/
categories:
  - Software

---
<img align="right" id="image297" alt="flash logo" src="http://www.fslog.com/wp-content/uploads/2006/11/flash-logo.thumbnail.jpg" />Flash player 9 beta is the latest version that you can get for your linux box. This is very essential for my life because I miss all the youtube videos. So, I decided to install the flash player 9 beta on by Ubuntu Edgy Eft 6.10.

First you have to install the flash player 7. Remember to enable all the repositories.

<pre>sudo apt-get install flashplugin-nonfree
sudo update-flashplugin
sudo apt-get install libflash-mozplugin</pre>

After flash player 7 is installed, you can carry on your installation for the new release. These three command will download the player, extract it and also install it.

<pre>wget <a class="external free" title="http://download.macromedia.com/pub/labs/flashplayer9 update/FP9 plugin beta 112006.tar.gz" rel="nofollow" href="http://download.macromedia.com/pub/labs/flashplayer9_update/FP9_plugin_beta_112006.tar.gz">http://download.macromedia.com/pub/labs/flashplayer9_update/FP9_plugin_beta_112006.tar.gz</a>
tar xvzf FP9_plugin_beta_112006.tar.gz
sudo cp flash-player-plugin-9.0.21.78/libflashplayer.so /usr/lib/flashplugin-nonfree/</pre>

This is an easy method for installing flash player for linux and now I can enjoy my videos.