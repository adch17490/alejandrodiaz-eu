---
title: "How I control my home with Home Assistant"
date: 2025-03-25
disableShare: true
ShowSocialIcons: false
tags: ["home automation", "home assistant", "zigbee", "knx"]
featured_image: /img/hass3d.png
---

For some time now, I've been using Home Assistant as the brain of my smart home. It's an open-source platform that centralizes all my devices: lights, sensors, blinds, heating, security, etc.

![Home Assistant main panel](/img/hass3d.png)

One of its strong points is its flexibility: I have it running on a Raspberry Pi 4, with Zigbee, MQTT, and KNX integration.

It allows me to automate things like:

- Lower the blinds if I open the window and it's cold
- Stop the blinds from moving for safety when I open the windows
- Increase the speed of the heat exchanger if I detect a rapid rise in humidity in the bathrooms (shower)
- Turn on the lights based on movement and brightness
- Control the underfloor heating according to rooms and schedules

Additionally, the control panel is fully customizable, and I'm starting to experiment with SCADA-style dashboards to view everything in real time.

In future posts, I'll explain how I have organized the sensor structure and some interesting automations that I use on a daily basis.
