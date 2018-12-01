---
title: 'ODOC: colrm'

date: 2006-04-16
url: /2006/04/16/odoc-colrm/
categories:
  - ODOC

---
colrm &#8212; Remove columns from a file.

Summary:

colrm removes selected columns from the input. Input is taken from STDIN and Output is sent to STDOUT. Column numbering starts with 1.

Examples:

> $ ls -l | colrm 35 &#8212; Remove all columns after the 34th column.
> 
> $ ls -l | colrm 1 14 &#8212; Remove columns from 1 to 14.

Read: man colrm
  
<tags>colrm, linux, odoc, gnu/linux<tags>