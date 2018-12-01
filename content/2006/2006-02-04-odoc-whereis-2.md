---
title: 'ODOC: whereis'

date: 2006-02-04
url: /2006/02/04/odoc-whereis-2/
categories:
  - ODOC

---
whereis &#8212; Locate the bin, src & man page for a file.

Summary :

**whereis** locates source/binary and manuals sections for specified files. _whereis_ will attempts to locate the desired program in a list of standard Linux places.

Example:

> $ whereis ls &#8212; Display the bin, src(if avail) and man page locations.
> 
> $ whereis -b ls &#8212; Show only bin file location.
> 
> $ whereis -m ls &#8212; Show only man page location.
> 
> $ whereis -s ls &#8212; Show only source file location.
> 
> $ whereis -u -M /usr/share/man/man1 -f route &#8212; Find the bin file location and search for man page in only man1 dir.
> 
> $ whereis -u -M /usr/man/man1 -S /usr/src -f * &#8212; Find all files in /usr/bin which are not documented in /usr/man/man1 with source in /usr/src.

Read: man whereis

<tags>whereis,man, odoc, linux, gnu/linux</tags>