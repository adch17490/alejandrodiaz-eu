---
title: "Mi servidor doméstico con Raspberry Pi 4, OMV y microservicios"
date: 2025-10-01
disableShare: true
ShowSocialIcons: false
tags: ["raspberry pi", "omv", "plex", "mealie", "kavita", "frigate", "microservicios"]
---

Desde hace un tiempo tengo montado un servidor casero sobre una **Raspberry Pi 4**, que me sirve como **nodo de almacenamiento, centro multimedia y plataforma de servicios personales**. Es una solución ligera, silenciosa, eficiente y... divertida de mantener 😄.

---

## 🧱 Base del sistema: Raspberry Pi 4 + OpenMediaVault

Uso una **Raspberry Pi 4 con 4GB de RAM**, a la que conecto un **disco duro externo USB de 1TB** como almacenamiento principal.

Sobre ella tengo instalado **[OpenMediaVault (OMV)](https://www.openmediavault.org/)**, una distro ligera y perfecta para NAS personales. Me permite:

- Gestionar fácilmente el almacenamiento
- Configurar carpetas compartidas vía Samba
- Controlar permisos
- Y lanzar contenedores Docker sin complicarme

Todo accesible por web, estable y con consumo energético mínimo.

---

## 🧩 Microservicios desplegados

Gracias a Docker y Portainer, tengo corriendo varios contenedores útiles:

### 🎬 Plex Media Server

Mi centro multimedia principal. Reproduce sin problemas contenido local desde el disco duro y lo sirvo en red a mi Fire Stick, móvil, y portátil. No tengo transcodificación activa (limita mucho en Pi), pero funciona perfectamente con archivos compatibles.

### 🍽️ Mealie

Una app genial para **gestionar recetas**, listas de la compra y planificaciones de comidas. La uso para organizar mis comidas semanales y compartir el menú en casa desde el móvil.

### 📚 Kavita

Una herramienta ligera para **leer cómics, libros y mangas** desde red local. Su interfaz es limpia, rápida, y me permite tener mi biblioteca bien organizada y accesible desde cualquier dispositivo.

---

## 📷 ¿Y Frigate?

Intenté montar **Frigate**, una solución potente para **detección de movimiento y objetos con cámaras IP**, que funciona con inteligencia artificial y procesamiento por TensorFlow.

El problema: la **Raspberry Pi 4 no tiene GPU ni potencia suficiente** para manejarlo en condiciones. Frigate requiere aceleración por hardware (tipo Coral USB, GPU externa o Jetson), y ahí mi setup se queda corto.

---

## 🚧 Limitaciones y próximos pasos

- **No puedo hacer transcodificación en Plex**, pero sí reproducción directa.
- Frigate lo he desactivado por ahora hasta tener hardware específico para visión por IA.
- Todo corre con cuidado de no saturar la RAM o temperatura. La Pi está en una carcasa con ventilador activo.

---

## 💡 Conclusión

Este servidor doméstico me da todo lo que necesito en mi día a día digital: multimedia, organización, lectura, y almacenamiento. Es modular, silencioso, y económico.

Si estás pensando en montarte uno parecido, la Pi 4 con OMV y Docker sigue siendo una opción excelente.

---

📩 ¿Usas algo similar? ¿Tienes una Coral USB para Frigate que te funcione bien?  
Cuéntamelo en [LinkedIn](https://www.linkedin.com/in/alejandro-dch/) o escríbeme por [email](mailto:alexdiaz17490@gmail.com).
