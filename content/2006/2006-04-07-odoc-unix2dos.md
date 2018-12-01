---
title: 'ODOC: unix2dos'

date: 2006-04-06
url: /2006/04/07/odoc-unix2dos/
categories:
  - ODOC

---
unix2dos &#8212; UNIX to DOS text file format converter.

Summary:

Each OS will indicate the line end using Line Feed (LF,10) or Carriage Return (CR,13). Unix uses LF as line end, Windows/DOS uses CR/LF and MacOS uses CR.

So when transferring a file from Linux to DOS, you have to convert the Line end to DOS format. unix2dos will convert the Unix text file to DOS format.

Examples:

> $ unix2dos gnu.txt &#8212; Convert and replace gnu.txt.
> 
> $ unix2dos -n gnu.txt dos.txt &#8212; Convert gnu.txt and write into dos.txt
> 
> $ unix2dos -k gnu.txt &#8212; Convert and replace gnu.txt, while keeping original date stamp.

Read: man unix2dos
  
<tags>unix2dos, dos, unix, mac, linux, odoc, gnu/linux</tags>