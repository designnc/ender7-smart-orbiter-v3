# Creality Ender 7 - Smart Orbiter 3 + Klipper Build

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

---

## 🧰 Requisitos / Requirements

- Creality Ender 7  
- Smart Orbiter 3 (con stepper de 10:1 o 20:1)  
- Raspberry Pi o similar con Klipper  
- Fuente de alimentación estable  
- Impresora 3D adicional para imprimir soportes  

---

## 🔧 Instalación / Installation

1. Imprime los archivos `.3mf` desde `mount/3mf/`  
2. Revisa el diagrama de conexiones en `wiring/`  
3. Carga los archivos de Klipper desde `klipper/` en tu Raspberry Pi  
4. Ajusta PID, offsets y calibraciones según tu impresora  
5. Importa el perfil `.json` desde `slicer/OrcaSlicer/` en OrcaSlicer  

---

## 🧱 Archivos de Montaje / Mount Files

La carpeta `mount/` contiene todos los archivos necesarios para adaptar el extrusor **Smart Orbiter 3** a la **Creality Ender 7**:

- `3mf/`: Archivos orientados y preparados para impresión
- `editable/`: Archivos `.step` para personalización CAD

Incluye soportes, espaciadores, adaptadores y ductos diseñados específicamente para este montaje.

---

## 📸 Créditos / Credits

Modificación realizada por **@designnc**  
Basado en el diseño original de Smart Orbiter 3 por **LDO / MihaiDesign**  
Con aportes de la comunidad Klipper y usuarios de Ender 7  

---

## 📜 Licencia / License

MIT o CC-BY-4.0, dependiendo del contenido incluido. Revisa archivos individuales para más detalles.
