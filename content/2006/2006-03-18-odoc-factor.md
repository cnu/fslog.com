---
title: 'ODOC: factor'

date: 2006-03-18
url: /2006/03/18/odoc-factor/
categories:
  - ODOC

---
factor &#8212; Print prime factors

Summary:

Print the prime factors of each number.The algorithm it uses is not very sophisticated, so for some inputs \`factor&#8217; runs for a long time.

Example:

> $ factor 25 &#8212; Print prime factors
> 
> $ factor 125 200 &#8212; Print prime factors for each number.
> 
> $ factor \`echo &#8216;2^64-1&#8217;|bc\` &#8212; Factors the largest 64-bit number.
> 
> $ factor \`echo &#8216;4294967279 * 4294967291&#8217;|bc\` &#8212; Factors the largest 32-bit prime numbers. (Warning: It take more time)

Read: man factor
  
<tags>odoc, factor, linux, gnu/linux</tags>