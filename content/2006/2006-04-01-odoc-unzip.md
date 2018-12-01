---
title: 'ODOC: unzip'

date: 2006-03-31
url: /2006/04/01/odoc-unzip/
categories:
  - ODOC

---
unzip &#8212; List, Test & Extract compressed ZIP files.

Summary:

unzip will list, test, or extract files from a ZIP archive. The default behavior (with no options) is to extract into the current directory (and subdirectories below it) all files from the specified ZIP archive.

Example:

> $ unzip myfile.zip &#8212; Unzip the myfile.zip
> 
> $ unzip -t myfile.zip &#8212; Test correctness of the file.
> 
> $ unzip myfile \*.txt &#8212; Unzip only \*.txt files
> 
> $ unzip myfile \*.txt \*.sxi \*.tex &#8212; Unzip only \*.txt, \*.sxi and \*.tex files
> 
> $ unzip myfile -d /tmp &#8212; Unzip the files in /tmp Dir.
> 
> $ unzip -f myfile &#8212; Unzip files which are newer then current Dir files.
> 
> $ unzip -o myfile &#8212; Unzip and overwrite existing files without prompting.

Read: man unzip (Lot of examples are available)
  
<tags>unzip, zip, odoc, linux, gnu/linux</tags>