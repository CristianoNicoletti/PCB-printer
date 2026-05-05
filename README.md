# PCB-printer
Open-source desktop PCB printer project. Includes hardware designs and schematics for rapid, affordable PCB prototyping at home or in a makerspace.


## Features
- Core XY construction
- easy assembly
- subtractive PCB printing method



## 📸 Overview
# insert picture

PCB Printer Build 
Printed PCB Result

---

## ⚙️ System Overview

### Hardware
- Arduino Uno  
- CNC Shield + A4988 Stepper Drivers  
- 3x NEMA 17 Stepper Motors
- Custom frame (3D printed + aluminum profiles)  
- spindle motor 
- 12V Power Supply  

### Software
- GRBL firmware (Arduino)  
- G-code sender (Universal G-code Sender)  
- PCB design tools (KiCad / Eagle)  

---

## 🔁 Workflow

1. Design PCB in KiCad  
2. Export Gerber files  
3. Convert to G-code  
4. Upload G-code to Arduino (GRBL)  
5. Machine engraves circuit onto copper board  

---

## 🧩 Repository Structure

# fix

pcb-printer/ │── README.md │── hardware/ │   ├── CAD/ │   │   ├── pcb_printer.f3d │   │   ├── pcb_printer.step │   │   ├── parts/ │   │       ├── motor_mount.stl │   │       ├── frame_connector.stl │   ├── drawings/ │       ├── assembly.pdf │── software/ │   ├── arduino/ │   ├── gcode_examples/ │── images/ │── docs/

---

## 🛠️ Build Instructions

### Bill of Materials (BOM)

# do

| Component            | Quantity |
|---------------------|--------|
| Arduino Uno         | 1      |
| CNC Shield          | 1      |
| Stepper Motor       | 2      |
| A4988 Drivers       | 2      |
| Power Supply (12V)  | 1      |

---

### Assembly

# do
- Construct frame using 3D printed connectors and profiles  
- Mount stepper motors on X and Y axes  
- Wire Arduino, CNC shield, and drivers  

---

### Setup
- Flash GRBL firmware to Arduino  
- Connect to G-code sender  
- Calibrate steps/mm for both axes  

---

## ⚠️ Challenges

---

## 🚀 Future Improvements

- Add Z-axis for engraving capability  
- Replace pen with engraving spindle  
- Improve precision using linear rails  
- Implement limit switches and homing  

---

## 📁 Files

- .f3d → editable Fusion 360 design  
- .step → universal CAD format  
- .stl → 3D printable parts  
- .pdf → schematics  

---

## 📜 License

MIT License

---

## 👤 Author

Cristiano Nicoletti 
Mechatronics Engineering Student