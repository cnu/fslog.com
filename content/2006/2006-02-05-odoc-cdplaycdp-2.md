---
title: 'ODOC: cdplay,cdp'

date: 2006-02-05
url: /2006/02/05/odoc-cdplaycdp-2/
categories:
  - ODOC

---
cdplay, cdp &#8212; Program to Control & Play Audio CDs.

Summary :

**cdplay** is a text-mode program for controlling and playing audio CDs. **cdp** is same as cdplay. But it is an interactive program. It uses the NUM keypad as a control panel to allow you to move track to track, play, pause, stop, and resume playing of audio CDs.

Example:

> $ cdp &#8212; Start in interactive mode with text based user interface.
> 
> $ cdplay &#8212; Start playing the Audio CD in the CD Drive.
> 
> $ cdplay play 6 &#8212; Play the track number 6.
> 
> $ cdplay stop &#8212; Stop it.
> 
> $ cdplay -l &#8212; Slow start (Give some time for CD Drive to init).
> 
> $ cdplay table &#8212; Show CD Contents.

Note:

  * Most of the command line options are same for cdplay and cdp.
  * If the Audio-Out of the CD Drive is not connected to sound card then, you have use the head-phone out of the CD Drive to hear the music.

Read: man cdp/cdplay

<tags>cdp, cdplay, odoc, linux, gnu/linux, audio+cds</tags>