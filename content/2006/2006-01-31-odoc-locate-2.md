---
title: 'ODOC: locate'

date: 2006-01-31
url: /2006/01/31/odoc-locate-2/
categories:
  - ODOC

---
locate &#8212; Quick search for files

Summary :

Locate provides a secure way to index and quickly search for files on your system. The index database to make searching faster and file permissions and ownership info will give the security.

Example:

> $ locate myfile &#8212; Locate myfile in the DB and Print the path.
> 
> $ locate -i MyFile &#8212; Same as above. But Case insensitive.
> 
> $ locate -q myfile &#8212; Run in Quiet Mode.
> 
> $ locate -n 10 myfile &#8212; Limit the no. of results shown to 10.
> 
> \# locate -U mydir -o myDB &#8212; Create index DB starting at path mydir and store the index file in myDB.

Read: man locate

<tags>locate, odoc, linux, gnu/linux</tags>