---
title: Firefox 1.5 in Ubuntu Breezy

date: 2006-01-30
url: /2006/01/30/firefox-15-in-ubuntu-breezy-2/
categories:
  - Software
  - Tutorial

---
Ubuntu Breezy 5.10 users search for installing Firefox 1.5 on their boxes. So, I thought of writing a tutorial. I am writing this using the information in the [Ubuntu Wiki][1]. There are a few points to note before installing Firefox 1.5.

  * Don&#8217;t remove the Ubuntu version of Firefox, otherwise, you will break a few packages
  * You will no longer get automatic updates through repositories, but the auto-updater built in firefox is enough
  * The Totem video plugin doesn&#8217;t work. I don&#8217;t use this particular plugin. Anyway you can install the package **mozilla-mplayer**.
  * You need package **libstdc++5** installed. 
    <pre>sudo apt-get install libstdc++5</pre>

  * There is a [bug in Firefox][2] which causes an error dialog to be displayed, each time FF starts up saying _Firefox could not install this item because of a failure in Chrome Registration_. Do this for a work around: 
    <pre>sudo mkdir -p /opt/firefox/extensions/talkback@mozilla.org
sudo touch /opt/firefox/extensions/talkback@mozilla.org/chrome.manifest</pre>

**Installing
  
** 

  * I would suggest you backup your bookmarks and settings by 
    <pre>cd ~/.mozilla/firefox/*.default
mkdir ~/Desktop/ffsettingscp bookmarks.html cert8.db cookies.txt formhistory.dat 
key3.db signons.txt history.dat  mimeTypes.rdf ~/Desktop/ffsettings</pre>

  * Download [firefox-1.5.tar.gz][3] and change to the directory you downloaded.
  * Extract it to `/opt/firefox` 
    <pre>sudo tar -C /opt -xvzf firefox-1.5.tar.gz</pre>

  * Link to your plugins and remove totem-mozilla as it doesn&#8217;t work with FF 1.5 
    <pre>cd /opt/firefox/plugins/sudo ln -s /usr/lib/mozilla-firefox/plugins/*
sudo rm libtotem_mozilla.*</pre>

  * Change to your home directory and rename your old profile(just as backup) 
    <pre>cd ~mv .mozilla .mozilla.ubuntu</pre>

  * To ensure it is used as the default version, modify the symbolic link in /usr/bin 
    <pre>sudo dpkg-divert --divert /usr/bin/firefox.ubuntu --rename /usr/bin/firefoxsudo
ln -s /opt/firefox/firefox /usr/bin/firefox</pre>
    
    The `dpkg-divert` command will move the original system-wide `/usr/bin/firefox` to a new name. The `ln` command will place a symbolic link to the newly installed firefox in `/usr/bin`.</li> 
    
      * Try the new firefox by typing `firefox`
      * Restore your old data 
        <pre>cd ~/Desktop/ffsettingsmv * ~/.mozilla/firefox/*.default</pre>
    
      * Restore your search plugins 
        <pre>sudo cp -i --reply=no /usr/lib/mozilla-firefox/searchplugins/* /opt/firefox/searchplugins/
sudo cp -i --reply=no ~/.mozilla/firefox/*.default/search/* /opt/firefox/searchplugins/</pre>
    
      * To ensure that other programs use the 1.5 version and not the older 1.0.7 version, goto Preferences>Preferred Applications in the System Menu. Under the Web Browser tab, choose custom and enter `firefox %s`</ul> 
    
    I hope this tutorial would really help many in installing Firefox and thereby enabling them to view the web in a totally different view. If anyone got any problem in installing Firefox or has got a better way, please discuss here.
    
    Technorati Tags: <a rel="tag" href="http://technorati.com/tag/firefox">firefox</a>, ubuntu, ubuntu linux, <a rel="tag" href="http://technorati.com/tag/firefox%201.5">firefox 1.5</a>, linux

 [1]: https://wiki.ubuntu.com/FirefoxNewVersion
 [2]: https://bugzilla.mozilla.org/show_bug.cgi?id=311480
 [3]: http://ftp.mozilla.org/pub/mozilla.org/firefox/releases/1.5/linux-i686/en-US/firefox-1.5.tar.gz