---
title: 'ODOC: ulimit'

date: 2005-11-14
url: /2005/11/14/odoc-ulimit-2/
categories:
  - ODOC

---
ulimit &#8211; Control the resources available to processes

Summary :

ulimit, Bash Built-in Command, provides control over the
  
resources (Virtual Mem, Max no .of process, Core file
  
size, &#8230;) available to processes started by the shell.

If Max no. of user process is set to 5, then the particular
  
user can&#8217;t run more then 5 process.

Examples :

> $ ulimit -a &#8212; Show All current limits.
> 
> $ ulimit -c &#8212; Show core file size (If Core file size is 0, Core file will not be created during the SEG fault).
> 
> $ ulimit -c 1000 &#8212; Set new core file size.
> 
> $ ulimit -u 3 &#8212; Set max no .of user processes
> 
> $ ulimit -n &#8212; Show max open files.

Read : info bash (or) help ulimit

<div>
  Tech Tags: <a rel="tag" href="http://technorati.com/tag/odoc">odoc</a> linux <a rel="tag" href="http://technorati.com/tag/gnu/linux">gnu/linux</a> <a rel="tag" href="http://technorati.com/tag/ulimit">ulimit</a>
</div>