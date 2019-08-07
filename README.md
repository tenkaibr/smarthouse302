# Smarthouse302
My Home Assistant Configuration (@Smarthouse302)

<p align="center"><img width="246" height="246" src="/images/logo.png"></p>

This is my Home Assistant configuration for a small appartment with 7 rooms (living room, kitchen, bedroom, suite, balcony and two bathrooms). It is my currently active set of configuration files for my Home Assistant running on Raspberry Pi.

Be sure to ⭐️ my configuration repo so you can keep up to date on any daily progress! Don't forget to check out [my blog](https://smarthouse302.blogspot.com/) and [my instagram account](https://www.instagram.com/smarthouse302/)

Use the menu links bellow to jump between sections.

# Menu

Hardware | Hubs | Lighting | Climate| Switches | Locks | Security | Voice Assistant | Media | Sensors | Cameras | Vacuum | Network | Other Hardware | Software | Screenshots |

# General Overview
This configuration controls a couple of significant features in my smart home.

<p align="center"><img width="500" height="450" src="/images/esquema.png"></p>

### Main Hardware

I am running Home Assistant within Hass.io on an Raspberry Pi B+.

1. [TP-Link ArcherC5400 v2.0](https://www.tp-link.com/us/home-networking/wifi-router/archer-c5400/) (Firmware 1.2.2 Build 20170912 rel.56240).
2. [Raspberry Pi 3 Model B+](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/) running Home Assistant 0.96.5.

### Add-ons running on my Home Assistant (Hass.io) instance

1. [DuckDNS](https://www.home-assistant.io/addons/duckdns/) - For keeping my SSL certificate validated through Let's Encrypt.
2. [Mosquitto Broker](https://www.home-assistant.io/addons/mosquitto/) - For managing my Sonoff devices and any future MQTT devices.
3. [Samba](https://www.home-assistant.io/addons/samba/) - For exploring the config files from a Windows computer.
4. [Spotify Connect](https://community.home-assistant.io/t/community-hass-io-add-on-spotify-connect/61210/1) (to do) - Play Spotify music on your Home Assistant device..

### My Custom cards on Home Assistant

1. [Markdown Mod](https://github.com/thomasloven/lovelace-markdown-mod) - Makes the built-in markdown card better.
2. [Atomic Calendar](https://github.com/atomic7777/atomic_calendar) - Advanced calendar card for Home Assistant with Lovelace.
3. [Card-tools](https://github.com/thomasloven/lovelace-card-tools) - Collection of tools to simplify creating custom cards 
4. [Button-card](https://github.com/custom-cards/button-card) - Lovelace Button card for your entities.
5. [Popup-card](https://github.com/thomasloven/lovelace-popup-card) - Replace the more-info dialog of one entity with a custom lovelace card
6. [Radial Menu](https://github.com/custom-cards/radial-menu) - Provides a radial menu on click for quick/space saving access to commands. 
7. [Layout-card](https://github.com/thomasloven/lovelace-layout-card) - Gives more control over the placement of lovelace cards

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

### Screenshots

![Screenshots 01](/images/screenshots-01.jpg =250x)
![Screenshots 02](/images/screenshots-02.jpg =250x)
![Screenshots 03](/images/screenshots-03.jpg =250x)

~~~~
Dark:

 dark-primary-color: "#a1a19a"
 disabled-text-color: "#545454"
 divider-color: "rgba(255, 255, 255, 0.12)"
 light-primary-color: "#524a4a"
 paper-card-background-color: "#202020"
 paper-grey-200: "#191919"
 paper-listbox-background-color: "#202020"
 primary-background-color: "#303030"
 primary-color: "#3d3d3d"
 primary-text-color: "#cfcfcf"
 secondary-background-color: "#131313"
 sidebar-text_-_background: "#62717b"
 sidebar-icon-color: "#3d3d3d"
 paper-icon-button: "#3d3d3d"
 paper-item-icon_-_color: "#D3D3D3"
 paper-item-icon-color: "#D3D3D3"
 accent-color: "#fa3e3e"
 --accent-color: "#fa3e3e"
 --lumo-base-color: "#4c4c4c"
 --lumo-contrast-90pct: "#a1a19a"
 lumo-base-color: "#4c4c4c"
 lumo-primary-color: "#a1a19a"
 lumo-primary-text-color: "#a1a19a"
 lumo-contrast-90pct: "#a1a19a"
 lumo-primary-color-50pct: "#000000"
 lumo-body-text-color: "#000000"
 lumo-header-text-color: "#000000"
 lumo-tertiary-text-color: "#000000"
 lumo-shade-5pct: "#646464"
 --lumo-shade-5pct: "#000000"
 table-row-alternative-background-color: "#232323"
 paper-card-header-color: "var(--paper-item-icon-color)"
 paper-item-icon-active-color: "var(--primary-color)"
 paper-listbox-color: "var(--primary-text-color)"
 paper-grey-50: "var(--primary-text-color)"
 paper-slider-active-color: "var(--primary-color)"
 paper-slider-knob-color: "var(--primary-color)"
 paper-slider-knob-start-color: "var(--primary-color)"
 paper-slider-pin-color: "var(--primary-color)"
 paper-slider-secondary-color: "var(--light-primary-color)"
 paper-toggle-button-checked-ink-color: "var(--dark-primary-color)"
 paper-toggle-button-checked-button-color: "var(--primary-color)"
 paper-toggle-button-checked-bar-color: "var(--light-primary-color)"
 paper-toggle-button-unchecked-bar-color: "var(--primary-text-color)"
 secondary-text-color: "var(--primary-color)"
 table-row-background-color: "var(--paper-card-background-color)"
~~~~

# Devices
Hubs

# Lighting

## Sensors


# To Do List


