---
title: 'ODOC: sha1sum'

date: 2006-03-17
url: /2006/03/17/odoc-sha1sum/
categories:
  - ODOC

---
sha1sum &#8211; Compute & Check Secure Hash Algorithm Std 1 message digest.

Summary:

**sha1sum** computes a 160-bit checksum/fingerprint/message-digest for each specified file. \`sha1sum&#8217; can also determine whether a file & checksum are consistent. The sums are computed as described in [FIPS-180-1][1].

Example:

> $ sha1sum file &#8212; Compute and print the MD5 checksum of that file.
> 
> $ sha1sum -c input.txt &#8212; Read checksum and filename from the file and validate checksums.
> 
> $ sha1sum -w -c input.txt &#8212; Same as above and warn if the checksums format is wrong in the file.
> 
> $ sha1sum &#8211;status -c input.txt &#8212; Indicate the status in exit status code.

Read: man sha1sum

Format of input.txt :

`2bff10a7855964335a86e84efb5f4ce9c40d4cfd` **file1**
  
`e62341664decd9f55896ab3635697de29ed1077f` **file2**
  
`9b088ddc22456233a76` **file3**
  
<tags>odoc, sha1sum, linux, gnu/linux</tags>

 [1]: http://www.itl.nist.gov/fipspubs/fip180-1.htm