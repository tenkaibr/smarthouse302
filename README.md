# Smarthouse302
My Home Assistant Configuration (@Smarthouse302)

<p align="center">
  <img width="246" height="246" src="/images/logo.png">
</p>

This is my Home Assistant configuration for a small appartment with 7 rooms (living room, kitchen, bedroom, suite, balcony and two bathrooms). It is my currently active set of configuration files for my Home Assistant running on Raspberry Pi.

Be sure to ⭐️ my configuration repo so you can keep up to date on any daily progress! Don't forget to check out [my blog](https://smarthouse302.blogspot.com/) and [my instagram account](https://www.instagram.com/smarthouse302/)

Use the menu links bellow to jump between sections.

# Menu

Hardware | Hubs | Lighting | Climate| Switches | Locks | Security | Voice Assistant | Media | Sensors | Cameras | Vacuum | Network | Other Hardware | Software | Screenshots |






# General Overview
This configuration controls a couple of significant features in my smart home.

### Hardware

I am running Home Assistant within Hass.io on an Raspberry Pi B+.

1. [TP-Link ArcherC5400 v2.0](https://www.tp-link.com/us/home-networking/wifi-router/archer-c5400/) (Firmware 1.2.2 Build 20170912 rel.56240).
2. [Raspberry Pi 3 Model B+](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/) running Home Assistant 0.96.5.

### Add-ons running on my Home Assistant (Hass.io) instance

1. DuckDNS - For keeping my SSL certificate validated through Let's Encrypt.
2. Mosquitto Broker - For managing my Sonoff devices and any future MQTT devices.
3. Samba Share - For exploring the config files from a Windows computer.
4. Spotify Connect (to do).

### Automation Overview
Typical Automations in use include

Turn on / off outside lights at sunset
Turn on / off pantry light when door opens / closes
Turn off lights after no activity / motion
Grouping of lights for use with Alexa for commands
Perform actions based on people leaving home / arriving home
Update location for user based on geolocation zones (Work, School, Church, Home)
Enable holiday color lights on outside lights via scenes
Turn on lights based on motion / ring front door and return to previous theme after
Send notification and flash lights if water detected in basement
Send notification and flash lights if water detected by washing machine / Kitchen Sink
Cut power to washing machine if water detected by washing machine
Send notification and flash lights if CO / Smoke detectors go off
Send alert if Eth miner hashrate drops
Send alert if power is lost at the house
Enhance security system through extra sensors and motion reading
Send alert if auxiliary / emergency heat is activated
Send long term data to InfluxDB for Grafana configuration


Alarm Clock using my bedroom lights and TV
Turning the outside lights on at night (to do)
Arming the alarm system when nobody is home
Security lighting when motion is detected at my front door

Note: Private information is stored in secrets.yaml (not uploaded)

2. Controle e monitoramento da iluminação;
3. Monitoramento e abertura de porta e janelas.
4. Programação de cenários de iluminação.
5. Controle do ar-condicionado.
6. Integração total com as TVs.
7. Aspiração automatizada.
8. Manipulação de cortinas e persianas.
9. Sonorização ambiente.
10. Controle por voz.
11. Higienização do mictório do pet.


# Devices
Hubs

# Lighting

## Sensors


# To Do List


