---
title: 'ODOC: strings'

date: 2006-03-05
url: /2006/03/06/odoc-strings-2/
categories:
  - ODOC

---
strings &#8211; Print the strings of printable characters in files.

Summary:

For each file given, strings prints the printable character sequences that are at least 4 characters long & are followed by an unprintable character. Strings is mainly useful for determining the contents of
  
non-text files.

Example:

> $ strings /bin/ls &#8212; Prints the strings from initialized & loaded sections.
> 
> $ strings -a file &#8212; Scan the whole file for the strings.
> 
> $ strings -f /bin/* | grep Free &#8212; Print Filename before each string.
> 
> $ strings -t o file &#8212; Print the offset within the file before each string [o = octal, x = hex, d = decimal].
> 
> $ strings -n 10 file &#8212; Print sequences of characters that are at least 10 characters long (Default 4).

NOTE: Write one &#8220;Hello World&#8221; Program in C and try this command on the binary file(a.out) of that program.

Read: man strings
  
strings, odoc, linux, gnu/linux