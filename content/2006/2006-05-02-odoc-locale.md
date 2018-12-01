---
title: 'ODOC: locale'

date: 2006-05-01
url: /2006/05/02/odoc-locale/
categories:
  - ODOC

---
locale &#8212; Get and show the locale-specific information.

Summary:

The locale program writes information about the current locale environment, or all locales, to screen. Locale is a set of local environment settings, which is used to describe the Language Encoding Standard, Date/Time format, Number format, Telephone Number format, Paper format, etc &#8230;

Examples:

> $ locale &#8212; Show the current locale settings.
> 
> $ locale -a &#8212; List currently available locale settings.
> 
> $ locale -m &#8212; List currently available character encodings.
> 
> $ locale -c LC\_TIME &#8212; Show values of the LC\_TIME.
> 
> $ locale -k LC\_TIME &#8212; Show the Name and Value of the LC\_TIME.

Read: man locale
  
<tags>locale, odoc, linux, gnu/linux</tags>