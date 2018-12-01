---
title: 'ODOC: mii-tool'

date: 2006-04-08
url: /2006/04/08/odoc-mii-tool/
categories:
  - ODOC

---
mii-tool &#8212; Show/Check/Set the MII status.

Summary:

MII (Media Independent Interface) is a standard bus which connects network interface controllers to physical media interfaces (PHYs). PHYs are usually located on a network interface card itself, but there are cards available which have external MII connectors for attaching external PHYs.

mii-tool display/checks/sets the status of a network interface&#8217;s MII unit. Most fast Ethernet adapters use an MII to autonegotiate link speed and duplex setting.

Examples:

> \# mii-tool &#8212; Show shot status info about the network card.
> 
> \# mii-tool -v &#8212; Show detailed status.
> 
> \# mii-tool -R &#8212; Reset the MII unit to default value.
> 
> \# mii-tool -r &#8212; Restart the Auto Negotiation.
> 
> \# mii-tool -w &#8212; Watch the network interface and show if there is any change in the status.(Run it and remove & reconnect the cable).
> 
> \# mii-tool -F 10baseT-HD &#8212; Forcibly set the capability to 10Mpbs and Half Duplex mode.
> 
> \# mii-tool -A 10baseT-HD, 10baseT-FD &#8212; Enable and restart Auto Negotiation, and advertise only the specified capabilities.

Read: man mii-tool
  
<tags>mii-tool,odoc, linux,gnu/linux,network</tags>