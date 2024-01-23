---
title: Installation
date: 2023-12-31 12:00:00
categories: [Tutorial, Setup]
tags: [openwrt, bootloader, terminal]     # TAG names should always be lowercase
pin: true
image:
    path: /pics/Sercomm-Openwrt-Login.jpg
    lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
    alt: After successful installation, you can log in via browser and configure the NA502(s) gateway.
---

>This project is  under active development.
{: .prompt-warning }

## Precondition check list

You need to check.

## TFTP installation instructions

You need to attach a serial console to the unpopulated 4-pin header near the LEDs. With the front of the device facing towards you, the pinout is: GND - TXD - ? - RXD. The settings are 57600 8N1 and you should see a bunch of messages immediately after start.

- Using the terminal, select option `1. Load system code to SDRAM via TFTP.``
- Put the `initramfs`` OpenWrt image on your TFTP server and boot it.
- You can then use `SSH`` to connect to the OpenWrt running from RAM.
- Transfer the OpenWrt `squashfs`` image to the device (for instance to /tmp/openwrt.bin)
- Run `sysupgrade -n /tmp/openwrt.bin`` to install the image to your device.
