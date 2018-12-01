---
title: 'ODOC: showkey'

date: 2006-01-30
url: /2006/01/30/odoc-showkey-2/
categories:
  - ODOC

---
showkey &#8212; Examine the codes sent by the keyboard

Summary :

**showkey** prints to standard output either the scan codes or the keycode or the \`ascii&#8217; code of each key pressed. It can be used to check the keyboard driver and key mappings.

Example:

> $ showkey &#8212; Show the interpreted keycode.
> 
> $ showkey -k &#8212; Same as above (Default Option).
> 
> $ showkey -s &#8212; Show the raw scan-codes of the keys.
> 
> $ showkey -a &#8212; Show the Decimal/Octal/Hex values of the keys.

Note:
  
If Showkey is in keycode/scancode mode, then you have to wait 10 second to exit. In ASCII mode, Press Ctrl+D to exit.

Read: man showkey

<tags>showkey, odoc, linux, gnu/linux</tags>