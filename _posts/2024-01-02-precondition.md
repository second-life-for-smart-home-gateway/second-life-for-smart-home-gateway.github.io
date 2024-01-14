---
title: Prerequisites
date: 2024-01-02 12:00:00
categories: [Tutorial, Preparation]
tags: [getting started]     # TAG names should always be lowercase
pin: true
---

## Everything you need for implementation

- computer device with an Ethernet and serial TTL connection
- `TFTP server` and `Console Client` running on your computer
- Sercomm NA502(s) gateway with the cover/housing removed
- 3-pin serial connection to the unpopulated `4-pin solder pads` near the LEDs
  - with the front of the device facing you, the pinout is as follows: `GND - TXD - n.a. - RXD`
  - the serial interface settings are `57600 8N1`
- direct LAN cable connection between computer and gateway
  - It is the safest to
    - manually assign your computer an IP address in the `192.168.1.x` range, eg. `192.168.1.100`
    - enter `192.168.1.1` for the router and
    - use `255.255.255.0` as the network mask

## Illustrations of the hardware tools used

![solder-pads](/pics/Sercomm-NA502-Connector.jpg){: .shadow }
_The Solder Pads of the NA502(s)_
![ttl-adapter](/pics/Sercomm-TTL-Adapter.jpg){: .shadow }
_The TTL Adapter_
![ttl-connection](/pics/Sercomm-NA502-Connection-Error.jpg){: .shadow }
_The wired connection_

>
- If the TTL connection is established when switching power on and `NO MESSAGES` are visible on the console, disconnect the TTL connection and restart the gateway without a TTL connection.
- When the gateway has completed the boot process, establish the TTL connection and then press the reset button.
- The gateway should now restart and a series of messages should now be visible.
{: .prompt-info }
