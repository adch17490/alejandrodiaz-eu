---
title: "My Home Server with Raspberry Pi 4, OMV and Microservices"
date: 2025-10-01
disableShare: true
ShowSocialIcons: false
tags: ["raspberry pi", "omv", "plex", "mealie", "kavita", "frigate", "microservices"]
---

For some time now, I've been running a small home server based on a **Raspberry Pi 4**, which serves as **storage hub, media center, and self-hosted services platform**. It's a lightweight, silent, energy-efficient setup — and a fun one to manage 😄.

---

## 🧱 System base: Raspberry Pi 4 + OpenMediaVault

I use a **Raspberry Pi 4 with 4GB RAM**, connected to a **1TB external USB hard drive** as the main storage.

I run **[OpenMediaVault (OMV)](https://www.openmediavault.org/)**, a lightweight Linux distro designed for personal NAS setups. It allows me to:

- Manage shared folders via Samba
- Control user permissions
- Monitor system health
- Run Docker containers easily

The web interface is clean and intuitive — perfect for this kind of project.

---

## 🧩 Deployed microservices

Thanks to Docker and Portainer, I run several useful services:

### 🎬 Plex Media Server

This is my go-to media server. It serves local content to my Fire Stick, laptop, and mobile devices without issues. I don't use transcoding (too demanding for the Pi), but direct play works flawlessly with compatible files.

### 🍽️ Mealie

A fantastic app to manage **recipes, meal planning, and grocery lists**. I use it weekly to organize meals and share the plan at home.

### 📚 Kavita

A lightweight reader for **comics, books and manga** over the local network. Fast, clean interface and ideal to manage my personal digital library.

---

## 📷 What about Frigate?

I tested **Frigate**, a powerful NVR system with **real-time object detection for security cameras**, powered by TensorFlow.

The downside: the **Raspberry Pi 4 lacks the computing power** (and GPU) needed to handle Frigate properly. It's designed for setups with hardware acceleration (like Coral USB or a dedicated GPU).

---

## 🚧 Limitations and future upgrades

- **No transcoding on Plex** due to hardware limitations, but direct play works.
- Frigate is paused for now until I get proper hardware (Coral, NVIDIA Jetson...).
- Everything runs with careful monitoring to avoid memory spikes or overheating (I use an active-cooled Pi case).

---

## 💡 Conclusion

This home server gives me everything I need on a daily basis: media, organization, reading, and reliable storage. It's modular, quiet, low-power, and still very capable.

If you're considering a similar setup, the Raspberry Pi 4 with OMV and Docker remains an excellent starting point.

---

📩 Do you run something like this? Have you tried Frigate with a Coral USB?  
Let’s chat on [LinkedIn](https://www.linkedin.com/in/alejandro-dch/) or feel free to [email me](mailto:alexdiaz17490@gmail.com).
