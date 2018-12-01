---
title: 'ODOC: dos2unix'

date: 2006-04-05
url: /2006/04/06/odoc-dos2unix/
categories:
  - ODOC

---
dos2unix &#8212; DOS/MAC to UNIX text file format converter.

Summary:

Each OS will indicate the line end using Line Feed (LF,10) or Carriage Return (CR,13). So when transferring a file from DOS to Linux, you have to convert the Line end from DOS format to Linux format.
  
dos2unix will convert the DOS/MAC Text file to Unix format. Unix uses LF as line end, Windows/DOS uses CR/LF and MacOS uses CR.

Examples:

> $ dos2unix dos.txt &#8212; Convert and replace dos.txt.
> 
> $ dos2unix -n dos.txt gnu.txt &#8212; Convert dos.txt and write into gnu.txt
> 
> $ dos2unix -k dos.txt &#8212; Convert and replace a.txt while keeping original date stamp.

Read: man dos2unix
  
<tags>dos2unix, linux, odoc, gnu/linux, mac, dos, unix</tags>