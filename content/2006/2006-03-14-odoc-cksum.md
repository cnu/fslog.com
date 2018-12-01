---
title: 'ODOC: cksum'

date: 2006-03-14
url: /2006/03/14/odoc-cksum/
categories:
  - ODOC

---
cksum &#8212; Computes a CRC (Cyclic Redundancy Check) checksum.

Summary:

**cksum** prints the CRC checksum for each file along with the number of bytes in the file. The CRC algorithm is specified by the POSIX Std. It is not compatible with the BSD or System V \`sum&#8217; algorithms.

Example:

> $ cksum file &#8212; Prints the Checksum, No of Bytes and filename.
> 
> $ cksum file1 file2 &#8212; Prints the Checksum, No of Bytes and filename for each file.

Read: man cksum
  
<tags>cksum, crc, linux, gnu/linux, odoc</tags>