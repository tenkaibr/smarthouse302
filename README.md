# Smarthouse302
My Home Assistant Configuration (@Smarthouse302)

## Hardware
I am running Home Assistant within Hass.io on an Ubuntu virtual machine which is running within VMware ESXi on an Intel NUC. For the most part, I have attempted to abstract as much hardware from the equation as possible.

## General Information
This configuration controls a couple of significant features in my smart home.

Alarm Clock using my bedroom lights and TV
Turning the outside lights on at night
Arming the alarm system when nobody is home
Security lighting when motion is detected at my front door
Note: Private information is stored in secrets.yaml (not uploaded)

## Automation Overview
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



# Devices
Hubs

# Lighting

## Sensors


# To Do List
