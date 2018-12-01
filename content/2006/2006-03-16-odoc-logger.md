---
title: 'ODOC: logger'

date: 2006-03-15
url: /2006/03/16/odoc-logger/
categories:
  - ODOC

---
logger &#8212; Makes entries in the system log file.

Summary:

**Logger** is a shell command interface to the syslog system log module. It can be used to makes entries in the system log from the shell scripts. By default, messages will be logged in `/var/log/messages`.

Example:

> $ logger MyLog1 &#8212; Log the message in syslog.
> 
> $ logger -i MyLog2 &#8212; Log the message with PID.
> 
> $ logger -s MyLog3 &#8212; Log the message in stderr and syslog.
> 
> $ logger -t MYTAG MyLog4 &#8212; Log the message with specified Tag.
> 
> $ logger -p user.panic MyLog5 &#8212; Log the message with priority.

Read the man page for more priority Facility and Level details.

Read: man logger
  
<tags>logger, log, odoc, linux, gnu/linux</tags>