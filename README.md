# Creality Ender 7 - Smart Orbiter 3 + Klipper Build

![Vista general del montaje](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/images/Ender%207%20X%20S03%20v3.3-1.png)

## 🛠️ Descripción (Español)

Este proyecto documenta la modificación de una impresora **Creality Ender 7** con el extrusor directo **Smart Orbiter 3**, junto con la implementación de firmware **Klipper**. El objetivo fue mejorar la calidad de impresión, la precisión en extrusión y la capacidad de trabajar con filamentos flexibles.

Incluye:
- Archivos de montaje en formato `.3mf`
- Configuración de firmware Klipper
- Perfiles de laminado (OrcaSlicer)
- Esquema de conexiones electrónicas
- Fotografías del montaje
- Archivos editables `.step` para personalización

🔗 Más información sobre el extrusor Smart Orbiter 3 en el sitio oficial:  
[https://www.orbiterprojects.com/so3/](https://www.orbiterprojects.com/so3/)

---

## 🛠️ Description (English)

This project documents the modification of a **Creality Ender 7** 3D printer using a **Smart Orbiter 3** direct-drive extruder and **Klipper** firmware. The goal is to enhance print quality, extrusion accuracy, and compatibility with flexible filaments.

Includes:
- Mount parts in `.3mf` format
- Klipper firmware configuration
- Slicer profiles (OrcaSlicer)
- Wiring diagrams
- Assembly photos
- Editable `.step` files for customization

🔗 Learn more about the Smart Orbiter 3 extruder at the official site:  
[https://www.orbiterprojects.com/so3/](https://www.orbiterprojects.com/so3/)

---

## 📂 Contenido del repositorio / Repository structure

- `mount/3mf/`: Archivos 3D `.3mf` listos para imprimir / Printable parts  
- `mount/editable/`: Archivos `.step` editables / Editable CAD files  
- `klipper/`: Archivos de configuración para Klipper / Klipper firmware config  
- `slicer/OrcaSlicer/`: Perfiles exportados desde OrcaSlicer / Slicer profiles  
- `images/`: Fotografías del montaje / Assembly photos  
- `wiring/`: Diagramas de conexiones / Wiring diagrams  
- `SO3/SO3_EzMount_v1/`: Mod para montar fan y probe directamente sobre el extrusor

---

## ⚙️ Configuración Klipper personalizada / Custom Klipper Configuration

La carpeta `klipper/` contiene todos los archivos personalizados utilizados en este mod para Klipper. Está organizada para facilitar la integración modular.

Incluye:
- `printer.cfg`: archivo principal de configuración.
- `SO3.cfg`: configuración del extrusor Smart Orbiter 3.
- `crtouch.cfg` y `microprobe.cfg`: soporte para sensores de autonivelación.
- `drivers_tmc2209.cfg` y `drivers_tmc5160.cfg`: según el tipo de driver que uses.
- `macros.cfg`: comandos útiles para calibración y pruebas.

> Puedes importar estos archivos directamente o integrarlos con `include`.

---

## 🧱 Archivos de Montaje / Mount Files

La carpeta `mount/` contiene todos los archivos necesarios para adaptar el extrusor **Smart Orbiter 3** a la **Creality Ender 7**:

- `3mf/`: Archivos orientados y preparados para impresión
- `editable/`: Archivos `.step` para personalización CAD

Incluye soportes, espaciadores, adaptadores y ductos diseñados específicamente para este montaje.

---

## 🧩 Modificación EzMount para SO3

Esta carpeta contiene una versión modificada del soporte del **Smart Orbiter 3** llamada **EzMount**, diseñada para simplificar el montaje del ventilador de capa y el sensor de nivelación (probe) directamente sobre el cuerpo del extrusor.

Ubicación: `SO3/SO3_EzMount_v1/`

Incluye:
- Archivos `.3mf` para:
  - Soporte para ventilador
  - Soporte para sensor (CR-Touch / Microprobe)
  - Ensamble principal
- Imágenes de referencia del modelo ensamblado

Imágenes de vista previa:
![S03 EzMount P1](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P1.png)
![S03 EzMount P2](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P2.png)
![S03 EzMount P3](https://github.com/designnc/ender7-smart-orbiter-v3/raw/main/SO3/SO3_EzMount_v1/S03%20EzMount%20V1.0%20P3.png)

> Esta mejora permite reducir la cantidad de piezas y cables, ofreciendo un diseño más compacto y funcional.

---

## 🔧 Instalación / Installation

1. Imprime los archivos `.3mf` desde `mount/3mf/` o `SO3_EzMount_v1/`  
2. Revisa el diagrama de conexiones en `wiring/`  
3. Carga los archivos de Klipper desde `klipper/` en tu Raspberry Pi  
4. Ajusta PID, offsets y calibraciones según tu impresora  
5. Importa el perfil `.json` desde `slicer/OrcaSlicer/` en OrcaSlicer  

---

## 📸 Créditos / Credits

Modificación realizada por **@designnc**  
Basado en el diseño original de Smart Orbiter 3 por **LDO / MihaiDesign**  
Con aportes de la comunidad Klipper y usuarios de Ender 7  

---

## 📜 Licencia / License

MIT o CC-BY-4.0, dependiendo del contenido incluido. Revisa archivos individuales para más detalles.
