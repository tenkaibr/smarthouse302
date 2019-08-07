# Smarthouse302
My Home Assistant Configuration ([@Smarthouse302](https://www.instagram.com/smarthouse302/))

<p align="center"><img width="246" height="246" src="/images/logo.png"></p>

This is my Home Assistant configuration for a small appartment with 7 rooms (living room, kitchen, bedroom, suite, balcony and two bathrooms). It is my currently active set of configuration files for my Home Assistant running on Raspberry Pi.

Be sure to ⭐️ my configuration repo so you can keep up to date on any daily progress! Don't forget to check out [my blog](https://smarthouse302.blogspot.com/) and [my instagram account](https://www.instagram.com/smarthouse302/)

# General Overview
This configuration controls a couple of significant features in my smart home.

<p align="center"><img width="500" height="450" src="/images/esquema.png"></p>

1. Lighting control and monitoring;
2. Monitoring and opening of doors and windows.
3. Programming of lighting scenarios.
4. Air conditioning control.
5. Full integration with TVs.
6. Automated aspiration.
7. Handling of curtains and blinds.
8. Ambient sound.
9. Voice control.
10. Pet urinal hygiene.

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

### Screenshots

<p align="center">
 <img width="250" src="/images/screenshots-01.jpg">
 <img width="250" src="/images/screenshots-02.jpg">
 <img width="250" src="/images/screenshots-03.jpg">
</p>


### Home Assistant Integrations

1. [Google Assistant](https://www.home-assistant.io/components/google_assistant/) - The google_assistant integration allows you to control things via Google Assistant (on your mobile or tablet) or a Google Home device.
2. [Google Calendar Event](https://www.home-assistant.io/components/calendar.google/) - The google calendar platform allows you to connect to your Google Calendars and generate binary sensors.
3. [Push Notifications](https://www.home-assistant.io/components/html5/) - The html5 notification platform enables you to receive push notifications to Chrome or Firefox, no matter where you are in the world.
4. [Xiaomi Gateway (Aqara)](https://www.home-assistant.io/components/xiaomi_aqara/) - The xiaomi_aqara integration allows you to integrate Xiaomi Aqara-compatible devices into Home Assistant.
5. [Broadlink](https://www.home-assistant.io/components/broadlink/) - There is currently support for the following device types within Home Assistant:
6. [Dark Sky](https://www.home-assistant.io/components/weather.darksky/) - The darksky platform uses the Dark Sky web service as a source for meteorological data for your location.
7. [MQTT](https://www.home-assistant.io/components/mqtt/) - MQTT (aka MQ Telemetry Transport) is a machine-to-machine or “Internet of Things” connectivity protocol on top of TCP/IP. It allows extremely lightweight publish/subscribe messaging transport.
8. [Xiaomi Mi Robot Vacuum](https://www.home-assistant.io/components/vacuum.xiaomi_miio/) - The xiaomi_miio vacuum platform allows you to control the state of your Xiaomi Mi Robot Vacuum. <span style="color:red">TO DO</span>.

### Automations

1. Send notification if new Home Assistant release through HTLM5 and creates a persistent notification.

# Theme

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

### Hubs

| [Xiaomi Mijia Gateway](https://www.gearbest.com/living-appliances/pp_344667.html?wid=1433363) | [Broadlink RM PRO](https://www.gearbest.com/smart-home-controls/pp_255607.html) |
|:-------------:|:-------------:|
| <p align="center"><img width="200" src="/images/xiaomi-gateway.jpg"></p> | <p align="center"><img width="200" src="/images/broadlink.jpg"></p> |
| U$27.99 | U$38.78 |

### Switches

| [TP-Link HS200](https://www.tp-link.com/la/home-networking/smart-switch/hs200/) | [Sonoff Mini](https://www.itead.cc/sonoff-mini.html) | [Sonoff Pow R2](https://www.itead.cc/sonoff-pow-r2.html) | [Sonoff Pow R2](https://www.itead.cc/sonoff-pow-r2.html) |
|:-------------:|:-------------:|:-------------:|:-------------:|
| <p align="center"><img width="200" src="/images/HS200.jpg"></p> | <p align="center"><img width="200" src="/images/sonoff.jpg"></p> | <p align="center"><img width="200" src="/images/sonoff-pow.jpg"></p> | <p align="center"><img width="200" src="/images/sonoff-pow.jpg"></p> |
| U$22.99 | U$8.49 | U$14.00 | U$14.00 |


sonoff-basic.jpg

### Sensors

|[Aqara Motion Sensor](https://www.gearbest.com/alarm-systems/pp_659226.html?wid=1433363)| [Xiaomi Door Sensor](https://www.gearbest.com/smart-light-bulb/pp_257677.html?wid=1433363) | [Aqara Temperature Sensor](https://www.gearbest.com/access-control/pp_626702.html?wid=1433363) |
|:-------------:|:-------------:|:-------------:|
| <p align="center"><img width="200" src="/images/motion-sensor.jpg"></p> | <p align="center"><img width="200" src="/images/window-sensor.jpg"></p> | <p align="center"><img width="200" src="/images/temperature-sensor.jpg"></p> |
| U$14.99 | U$10.87 | U$13.99 |


# To Do List


