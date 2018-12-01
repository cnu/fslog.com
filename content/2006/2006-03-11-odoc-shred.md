---
title: 'ODOC: shred'

date: 2006-03-11
url: /2006/03/11/odoc-shred/
categories:
  - ODOC

---
shred &#8212; Overwrite/Delete a file securely.

Summary:

Overwrite the specified file repeatedly and remove, in order to make it harder for even very expensive hardware probing to recover the data.

Example:

> $ shred file &#8212; Repeatedly overwrite the file content with random data.
> 
> $ shred -v file &#8212; Show progress info.
> 
> $ shred -n 5 file &#8212; Overwrite 5 times instead of the default is 25.
> 
> $ shred -x file &#8212; Use exact file size. Don&#8217;t round off.
> 
> $ shred -z file &#8212; At the end of shred, overwrite the file with zeros.
> 
> $ shred -u file &#8212; Overwrite, Truncate and Remove the file.

Read: man shred

<tags>shred, odoc, linux, gnu/linux</tags>