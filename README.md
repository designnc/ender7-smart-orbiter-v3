# Creality Ender 7 - Smart Orbiter 3 + Klipper Build

![Overview Image](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/images/Ender%207%20X%20S03%20v3.3-1.png)

## Table of Contents / Tabla de Contenidos

- [Project Description / Descripción del Proyecto](#project-description--descripción-del-proyecto)
- [Important Warnings / Advertencias](#important-warnings--advertencias)
- [Repository Structure / Estructura del Repositorio](#repository-structure--estructura-del-repositorio)
- [Klipper Configuration / Configuración de Klipper](#klipper-configuration--configuración-de-klipper)
- [Mount Files / Archivos de Montaje](#mount-files--archivos-de-montaje)
  - [Assembly Notes / Notas de Ensamblaje](#assembly-notes--notas-de-ensamblaje)
- [EzMount Mod / Mod EzMount](#ezmount-mod--mod-ezmount)
- [Known Issues / Problemas Conocidos](#known-issues--problemas-conocidos)
- [Installation / Instalación](#installation--instalación)
- [Credits / Créditos](#credits--créditos)
- [License / Licencia](#license--licencia)

---

## Project Description / Descripción del Proyecto

This project documents the modification of a **Creality Ender 7** 3D printer using a **Smart Orbiter 3** direct-drive extruder, combined with **Klipper** firmware. The goal is to improve print quality, extrusion accuracy, and compatibility with flexible filaments.

Este proyecto documenta la modificación de una **Creality Ender 7** con un extrusor directo **Smart Orbiter 3**, utilizando firmware **Klipper**, con el fin de mejorar la calidad de impresión y la compatibilidad con filamentos flexibles.

🔗 Learn more / Más información: [https://www.orbiterprojects.com/so3/](https://www.orbiterprojects.com/so3/)

---

## Important Warnings / Advertencias

1. **Reduced print volume / Área de impresión reducida**:  
   From / De **250x250x300 mm** → To / A **240x240x295 mm**

2. **belt modification / Modificación de correas**:  
   You'll need to trim the belts / Se deben recortar ligeramente las correas.

3. **Y endstop relocation / Reubicación del endstop del eje Y**:  
   Must be moved forward / Debe moverse hacia adelante.  
   ✅ Adapter included / Adaptador incluido

---

## Repository Structure / Estructura del Repositorio

- `mount/3mf/`: Printable `.3mf` files / Archivos `.3mf` listos para imprimir  
- `mount/editable/`: Editable `.step` files / Archivos `.step` editables  
- `mount/Ender 7 X SO3 v.3.3/`: Main mount  
- `klipper/`: Klipper config / Configuración Klipper  
- `slicer/OrcaSlicer/`: OrcaSlicer profiles  
- `images/`: Assembly photos / Fotos del ensamblaje  
- `wiring/`: Wiring diagrams / Diagramas de conexiones  
- `SO3/SO3_EzMount_v1/`: Fan + probe mount mod

---

## Klipper Configuration / Configuración de Klipper

- `printer.cfg`: Main config  
- `SO3.cfg`: Smart Orbiter 3 config  
- `crtouch.cfg` / `microprobe.cfg`: Probes  
- `drivers_tmc2209.cfg` / `tmc5160.cfg`: Stepper drivers  
- `macros.cfg`: Useful macros

Modular configuration using `include`.

---

## Mount Files / Archivos de Montaje

Parts to mount the Smart Orbiter 3 on the Ender 7:

- `3mf/`: Ready-to-print  
- `editable/`: Editable `.step` for customization  
- Main mount: `mount/Ender 7 X SO3 v.3.3/`

### Assembly Notes / Notas de Ensamblaje

The main mount located in `mount/Ender 7 X SO3 v.3.3/` includes all components required to attach the Smart Orbiter 3 to the Ender 7.

- Uses **M3 screws** and **heat-set threaded brass inserts**
- Includes motor mount, hotend support, fan duct, and belt holder
- Exact screw lengths and quantities to be confirmed

---

El montaje principal ubicado en `mount/Ender 7 X SO3 v.3.3/` incluye todas las piezas necesarias para instalar el Smart Orbiter 3 en la Ender 7.

- Utiliza **tornillos M3** y **insertos metálicos tipo termofijado**
- Incluye soporte de motor, soporte de hotend, ducto de ventilación y tensor de correa
- Las longitudes y cantidades exactas de tornillos serán confirmadas

---

## EzMount Mod / Mod EzMount

Custom mount for the fan and probe directly on SO3:

- Located in `SO3/SO3_EzMount_v1/`
- `.3mf` files
- Previews:

![S03 EzMount P1](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P1.png)  
![S03 EzMount P2](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P2.png)  
![S03 EzMount P3](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P3.png)

> This mod simplifies wiring and reduces the number of printed parts.

---

## Known Issues / Problemas Conocidos

These issues may vary depending on print speed, slicer settings, and printer condition.

---

Estos problemas pueden variar según la velocidad de impresión, el laminador y el estado de la impresora.

### 🌀 Vibrations / Vibraciones

- Some noticeable **vibrations** during fast movements or high-speed printing  
- Using the original **plastic cover** over the head may worsen this — removal is recommended

---

Durante movimientos rápidos o impresiones a alta velocidad, se pueden notar **vibraciones**.  
El uso de la **tapa protectora plástica original** puede aumentar estas vibraciones — se recomienda retirarla.

### 🔊 Fan Noise / Ruido del Ventilador

- The small **cooling fan on the SO3** can produce a **high-pitched noise** ("mosquito-like") due to its speed and size

---

El pequeño **ventilador de enfriamiento del SO3** puede generar un **ruido agudo tipo mosquito** debido a su alta velocidad y tamaño reducido.

---

## Installation / Instalación

1. Print parts from `mount/3mf/` or `SO3_EzMount_v1/`  
2. Trim Y belts and relocate endstop (adapter included)  
3. Load Klipper config files from `klipper/`  
4. Tune PID, axis offsets and travel limits  
5. Import OrcaSlicer profile from `slicer/OrcaSlicer/` *(coming soon)*

---

## Credits / Créditos

Based on: **Smart Orbiter 3** by **Dr. Róbert Lőrincz**, manufactured in collaboration with **LDO Motors**  
Mod design and adaptation for Ender 7 by **@designnc**  
Thanks to / Gracias a: Klipper + Ender 7 community

---

## License / Licencia

This project is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

You are free to remix, adapt, and build upon this work **non-commercially**, as long as you **credit the original author** (@designnc) and **license your new creations under identical terms**.

More info: [https://creativecommons.org/licenses/by-nc-sa/4.0/](https://creativecommons.org/licenses/by-nc-sa/4.0/)

---

Este proyecto está licenciado bajo **Creative Commons Atribución-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)**.

Puedes modificar, adaptar y crear versiones derivadas **solo para uso no comercial**, siempre que **des crédito al autor original** (@designnc) y **compartas tus nuevas versiones bajo la misma licencia**.

Más información: [https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.es)