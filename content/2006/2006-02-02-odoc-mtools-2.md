---
title: 'ODOC: mtools'

date: 2006-02-02
url: /2006/02/02/odoc-mtools-2/
categories:
  - ODOC

---
mtools &#8211; Utilities to access DOS disks in Unix

Summary :

Mtools is a public domain collection of tools to allow Unix systems to manipulate DOS files: Read, Write, Delete & Move around files on an DOS file system (Default floppy). Each program attempts to emulate the MS-DOS equivalent command. No need to mount the DOS file system.

Example:

> $ mdir &#8212; List files from the floppy.
> 
> $ minfo &#8212; Get DOS FS info.
> 
> $ mdu dir1 &#8212; Space usage report of dir1.
> 
> $ mcopy myfile a: &#8212; Copy DOS files to/from Linux.
> 
> $ mcd dir1 &#8212; Change the current dir to a:/dir1.
> 
> $ mmove file1 file2 &#8212; Move/Rename an DOS file/subdir.
> 
> $ mdel file &#8212; Del a DOS file from floppy.
> 
> $ mdeltree dir &#8212; Del a DOS dirtree from floppy.
> 
> $ mformat &#8212; Create a DOS FS in a formatted floppy.
> 
> $ mlabel &#8212; Make DOS volume label.

Note:

  * More tools are available in MTool Set.
  * Behavior of MTools will change depending upon the config `/etc/mtools.conf`.

Read: man mtools

<tags>odoc, mtools, dos, linux, gnu/linux</tags>