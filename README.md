# Creality Ender 7 - Smart Orbiter 3 + Klipper Build

![Overview Image](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/images/Ender%207%20X%20S03%20v3.3-1.png)

## 📑 Table of Contents / Tabla de Contenidos

- [🛠️ Project Description / Descripción del Proyecto](#project-description--descripción-del-proyecto)
- [⚠️ Important Warnings / Advertencias](#important-warnings-before-installing-this-mod--advertencias-importantes-antes-de-instalar-el-mod)
- [📂 Repository Structure / Estructura del Repositorio](#repository-structure--estructura-del-repositorio)
- [⚙️ Klipper Configuration / Configuración de Klipper](#klipper-configuration--configuración-de-klipper)
- [🧱 Mount Files / Archivos de Montaje](#mount-files--archivos-de-montaje)
- [🧩 EzMount Mod / Mod EzMount](#ezmount-mod--mod-ezmount)
- [🔧 Installation / Instalación](#installation--instalación)
- [📸 Credits / Créditos](#credits--créditos)
- [📜 License / Licencia](#license--licencia)

---

## 🛠️ Project Description / Descripción del Proyecto

This project documents the modification of a **Creality Ender 7** 3D printer using a **Smart Orbiter 3** direct-drive extruder, combined with **Klipper** firmware. The goal is to improve print quality, extrusion accuracy, and compatibility with flexible filaments.

Este proyecto documenta la modificación de una **Creality Ender 7** con un extrusor directo **Smart Orbiter 3**, utilizando firmware **Klipper**, con el fin de mejorar la calidad de impresión y la compatibilidad con filamentos flexibles.

🔗 Learn more / Más información: [https://www.orbiterprojects.com/so3/](https://www.orbiterprojects.com/so3/)

---

## ⚠️ Important Warnings Before Installing This Mod / Advertencias importantes antes de instalar el mod

1. 📐 **Reduced print volume / Área de impresión reducida**:  
   From / De **250x250x300 mm** → To / A **240x240x295 mm**

2. ✂️ **Y-axis belt modification / Modificación de correas Y**:  
   You'll need to trim the Y belts / Se deben recortar ligeramente las correas del eje Y.

3. 🛑 **Y endstop relocation / Reubicación del endstop del eje Y**:  
   Must be moved forward / Debe moverse hacia adelante.  
   ✅ Adapter included / Adaptador incluido

---

## 📂 Repository Structure / Estructura del Repositorio

- `mount/3mf/`: Printable `.3mf` files / Archivos `.3mf` listos para imprimir  
- `mount/editable/`: Editable `.step` files / Archivos `.step` editables  
- `klipper/`: Klipper config / Configuración Klipper  
- `slicer/OrcaSlicer/`: OrcaSlicer profiles  
- `images/`: Assembly photos / Fotos del ensamblaje  
- `wiring/`: Wiring diagrams / Diagramas de conexiones  
- `SO3/SO3_EzMount_v1/`: Fan + probe mount mod

---

## ⚙️ Klipper Configuration / Configuración de Klipper

- `printer.cfg`: Main config  
- `SO3.cfg`: Smart Orbiter 3 config  
- `crtouch.cfg` / `microprobe.cfg`: Probes  
- `drivers_tmc2209.cfg` / `tmc5160.cfg`: Stepper drivers  
- `macros.cfg`: Useful macros

Modular configuration using `include`.

---

## 🧱 Mount Files / Archivos de Montaje

Parts to mount the Smart Orbiter 3 on the Ender 7:

- `3mf/`: Ready-to-print  
- `editable/`: Editable `.step` for customization

---

## 🧩 EzMount Mod / Mod EzMount

Custom mount for the fan and probe directly on SO3:

- Located in `SO3/SO3_EzMount_v1/`
- `.3mf` files
- Previews:

![S03 EzMount P1](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P1.png)
![S03 EzMount P2](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P2.png)
![S03 EzMount P3](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P3.png)

---

## 🔧 Installation / Instalación

1. Print from `mount/3mf/` or `SO3_EzMount_v1/`  
2. Trim belts & move endstop  
3. Setup Klipper with `klipper/`  
4. Tune PID, offsets  
5. Import OrcaSlicer profile

---

## 📸 Credits / Créditos

Designed by / Diseño: **@designnc**  
Based on: Smart Orbiter 3 by **LDO / MihaiDesign**  
Thanks to / Gracias a: Klipper + Ender 7 community

---

## 📜 License / Licencia

MIT or CC-BY-4.0 depending on file / según el archivo.
