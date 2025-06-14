# Creality Ender 7 - Smart Orbiter 3 + Klipper Build

## 🛠️ Descripción (Español)

Este proyecto documenta la modificación de una impresora **Creality Ender 7** con el extrusor directo **Smart Orbiter 3**, junto con la implementación de firmware **Klipper**. El objetivo fue mejorar la calidad de impresión, la precisión en extrusión y la capacidad de trabajar con filamentos flexibles.

Incluye:
- Archivos STL impresos personalizados
- Configuración de firmware Klipper
- Perfiles de laminado (Cura / PrusaSlicer)
- Esquema de conexiones electrónicas
- Fotografías del montaje

---

## 🛠️ Description (English)

This project documents the modification of a **Creality Ender 7** 3D printer using a **Smart Orbiter 3** direct-drive extruder and **Klipper** firmware. The goal is to enhance print quality, extrusion accuracy, and compatibility with flexible filaments.

Includes:
- Custom printable STL parts
- Klipper firmware configuration
- Slicer profiles (Cura / PrusaSlicer)
- Wiring diagrams
- Assembly photos

---

## 📂 Contenido del repositorio / Repository structure

- `stl/`: Archivos imprimibles personalizados / Printable STL files
- `klipper/`: Archivos de configuración del firmware / Klipper configuration files
- `slicer/`: Perfiles para Cura y/o PrusaSlicer / Slicer profiles
- `images/`: Fotografías del proceso / Assembly photos
- `wiring/`: Esquema de conexiones eléctricas / Wiring diagrams

---

## 🧰 Requisitos / Requirements

- Creality Ender 7
- Smart Orbiter 3 (con stepper de 10:1 o 20:1)
- Raspberry Pi o similar con Klipper
- Fuente de alimentación estable
- Impresora 3D adicional para imprimir soportes

---

## 🔧 Instalación / Installation

1. Imprime los STL en la carpeta `stl/`
2. Sigue el esquema de conexiones en `wiring/`
3. Carga los archivos de Klipper en tu Raspberry Pi
4. Ajusta PID, offsets y calibraciones según tu impresora
5. Importa los perfiles en tu laminador

---

## 📸 Créditos / Credits

Modificación realizada por **@designnc**  
Basado en el diseño original de Smart Orbiter 3 por **LDO / MihaiDesign**  
Con aportes de la comunidad Klipper y usuarios de Ender 7

---

## 📜 Licencia / License

MIT o CC-BY-4.0, dependiendo del contenido.
