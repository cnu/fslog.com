---
title: 'ODOC: setfont'

date: 2006-05-02
url: /2006/05/03/odoc-setfont/
categories:
  - ODOC

---
setfont &#8212; Load EGA/VGA console screen font.

Summary:

The setfont command reads a font file and loads it into the EGA/VGA character generator and optionally outputs the previous font. It can also load various mapping tables and output the previous versions. The standard Linux font format is the PSF (PC Screen Format) font.

Examples:

> $ setfont &#8212; Load the default font.
> 
> $ setfont -v &#8212; Load the default font with verbose output.
> 
> $ setfont iso01.14 &#8212; Load the iso01 font (size=8&#215;14).

`/lib/kbd/consolefonts` &#8211; Default Dir for console fonts.
  
`/lib/kbd/unimaps` &#8211; Default Dir for Unicode maps.
  
`/lib/kbd/consoletrans` &#8211; Default Dir for screen mappings.

Read the ReadMe files available in the above locations to get more information about the font and maps.

TIP: Set your default console font in `/etc/sysconfig/i18n` file.

Read: man setfont
  
<tags>setfont, linux, odoc, gnu/linux</tags>