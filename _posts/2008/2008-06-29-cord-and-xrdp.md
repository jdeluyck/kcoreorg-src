---
id: 255
title: CoRD and xrdp
date: 2008-06-29T17:07:47+02:00
author: Jan
layout: single
guid: http://sadevil.org/blog/?p=255
permalink: /2008/06/29/cord-and-xrdp/
categories:
  - Apple / Mac OS
  - Linux / Unix
tags:
  - beta
  - cord
  - Mac OS
  - rdp
  - xrdp
---
I was trying to get <a href="http://xrdp.sourceforge.net/" target="_blank">xrdp</a> running on my Linux box, so I could takeover the screen from the outside world. The <a href="http://en.wikipedia.org/wiki/Remote_Desktop_Protocol" target="_blank">rdp protocol</a> is a (huge) bit more performant than <a href="http://en.wikipedia.org/wiki/Vnc" target="_blank">VNC</a>, which is why I wanted to use it.

Today I was trying for the 3rd time to get it to work, using <a href="http://cord.sourceforge.net/" target="_blank">CoRD</a> as an RDP client, but I never got any image back &#8211; the client started, I saw the connection being built up, but I never got any image over. Starting <a href="http://www.rdesktop.org/" target="_blank">rdesktop</a> locally gave me the output I expected.

This gave me the idea of using <a href="http://connect.microsoft.com/macrdc" target="_blank">Microsoft Remote Desktop Connection Client for Mac 2 Public Beta</a>, to see if it might be a problem with the client&#8230; and yup, it is.

Seems CoRD 0.4.3 (the current stable) is unable to handle the output of xrdp. I now installed the <a href="http://sourceforge.net/forum/forum.php?forum_id=790899" target="_blank">0.5 beta 1</a> which works without any problems.