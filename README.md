# PCB Printer

An open-source desktop PCB printer designed for rapid and affordable PCB prototyping at home, in workshops, or in makerspaces.  
This project includes hardware designs, schematics, and supporting files for building a compact PCB fabrication machine.

---

## Features

- CoreXY motion system
- Easy-to-assemble design
- Subtractive PCB fabrication method
- Low-power milling for PCB engraving

---

## 📸 Overview

![PCB Printer Image](Images/PCB%20printer%20image.PNG)

---

## ⚙️ System Overview

### Hardware
- Arduino Uno
- CNC Shield with TMC2209 stepper drivers
- 3 × NEMA 17 stepper motors
- Custom frame made from 3D-printed parts and aluminum profiles
- Spindle motor
- 24V power supply
- limit switches
- rasberry pi (optional)
- 

### Software
- GRBL firmware for Arduino
- G-code sender software (Universal G-code Sender)
- PCB design software (KiCad / Eagle)

---

## 🔁 Workflow

1. Design the PCB in KiCad
2. Export the Gerber files
3. Convert the Gerbers to G-code
4. Send the G-code to the Arduino running GRBL
5. Engrave the circuit onto a copper-clad board

---

## 🛠️ Build Instructions

### Bill of Materials (BOM)
See the BOM file included in the project.

### Assembly
- Build the frame using aluminum profiles and 3D-printed connectors
- Mount the stepper motors on the X, Y, and Z axes
- Assemble the CoreXY motion system
- Install and route the belts
- Tension the belts evenly
- Wire the Arduino, CNC Shield, and stepper drivers

### Setup
- Flash GRBL firmware to the Arduino
- Connect the machine to a G-code sender
- Calibrate the steps/mm for each axis

---

## ⚠️ Challenges

- Finding reliable software for PCB toolpath generation and machine control
- Operating the machine without a dedicated host computer
- Reducing and absorbing vibrations during milling

---

## 🚀 Future Improvements

- Add laser cutting or engraving tools
- Upgrade to a more powerful spindle for acrylic milling
- Improve accuracy for denser PCB layouts

---

## 📁 Included Files

- `.f3d` — Editable Fusion 360 design files
- `.step` — Universal CAD files
- `.stl` — 3D-printable parts
- `.pdf` — Schematics and documentation

---

## 📜 License

This project is licensed under the MIT License.

---

## 👤 Author

**Cristiano Nicoletti**  
Mechatronics Engineering Student