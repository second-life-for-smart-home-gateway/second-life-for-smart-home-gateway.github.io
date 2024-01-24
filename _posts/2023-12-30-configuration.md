---
title: Configuration
date: 2023-12-30 12:00:00
categories: [Tutorial, Setup]
tags: [openwrt, webui]     # TAG names should always be lowercase
pin: true
image:
    path: /pics/Sercomm-ser2net-overview.jpg
    lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
    alt: We use ser2net to enable a connection to the internal serial interfaces of the Zwave and ZigBee controllers via TCP. 
---

## Making a "dump" wifi access point

For an easy start, the NA502(s) gateway operated with OpenWrt can be set up as a wireless access point (AP). This assumes that the Sercomm Gateway does not need to provide any routing, DHCP or DNS services.

A detailed description can be found at: [**Wireless Access Point (aka "Dumb" Access Point**)](https://openwrt.org/docs/guide-user/network/wifi/dumbap#wireless_access_point_aka_dumb_access_point){:target="_blank"}

>The **easiest** way is really to configure the **wireless AP** to get its address from the main router via **DHCP**, even though the guide focuses on how to do it with a static IP address.
{: .prompt-tip}

## Loading additional OpenWrt packages

### ser2net: Telnet/tcp connections to serial interfaces

### LuCI - Web interface support for ser2net
