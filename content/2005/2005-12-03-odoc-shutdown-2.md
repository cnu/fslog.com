---
title: 'ODOC: shutdown'

date: 2005-12-04
url: /2005/12/03/odoc-shutdown-2/
categories:
  - ODOC

---
shutdown &#8212; Bring the system down (Needs Root privilege)

Summary :

shutdown brings the system down in a secure way. All logged-in users are notified that the system is going down, and login is blocked. All processes are first notified that the system is going down by the signal SIGTERM. Runlevel 0 is used to halt the system, runlevel 6 is used to reboot the system. However please take care not to use this command on production systems.

Examples :

> \# shutdown 12:00 &#8212; Shutdown at 12:00
> 
> \# shutdown +10 &#8212; Shutdown after 10min
> 
> \# shutdown now &#8212; Immediate shutdown (now == +0)
> 
> \# shutdown -t 10 &#8212; Wait 10 Sec after warn the user
> 
> \# shutdown -k &#8212; Don&#8217;t really shutdown; only warn
> 
> \# shutdown -r -t 5 &#8212; Reboot after shutdown
> 
> \# shutdown -h -t 5 &#8212; Halt after shutdown
> 
> \# shutdown -f now &#8212; Skip fsck (File System Check) on reboot
> 
> \# shutdown -F now &#8212; Force fsck on reboot
> 
> \# shutdown -c &#8212; Cancel the already waiting shutdown process.

Read : man shutdown

There has been a great deal of flooding in Chennai, India due to the heavy rain yesterday and there was no power in the morning. I have written about the [plight of people due to the floods][1] in [my personal blog][2].

<div>
  Tech Tags: <a rel="tag" href="http://technorati.com/tag/odoc">odoc</a> linux <a rel="tag" href="http://technorati.com/tag/gnu/linux">gnu/linux</a> <a rel="tag" href="http://technorati.com/tag/shutdown">shutdown</a> <a rel="tag" href="http://technorati.com/tag/reboot">reboot</a> <a rel="tag" href="http://technorati.com/tag/halt">halt</a> <a rel="tag" href="http://technorati.com/tag/" />
</div>

 [1]: http://srinivasan.wordpress.com/2005/12/03/flooding-in-chennai/
 [2]: http://srinivasan.wordpress.com/