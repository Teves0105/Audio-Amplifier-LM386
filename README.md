# Audio Amplifier PCB Design (LM386) 🔈

A professional-grade Printed Circuit Board (PCB) design for a mono Audio Amplifier based on the **LM386** operational amplifier. This project was developed as a laboratory assignment for **ELEC2010: Introduction to Circuits for Electrical Engineers** at **VinUniversity**.

The project covers the end-to-end hardware design lifecycle, including schematic capture, component footprint definition, PCB layout design with clearance constraints, and the generation of manufacturing files.

## 📋 Features & Specifications
<div align="center">
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/8ebad289-2f26-4b2a-997f-5746c209c6de" />
 </div>
* **Core IC:** LM386 (DIP-8 package) for high-efficiency audio amplification.
* **Power Supply:** Wide input range (5V - 15V DC).
* **Connectivity:** 
  * 3.5mm Audio Jack (Surface-Mount Technology - SMT)
  * 2-Pin Header for DC power input
* **User Control:** Integrated 10kΩ Trimming Potentiometer for volume control.
* **Output:** 3W, 4Ω Speaker interface.
* **PCB Layout Constraints:** 
  * Wire width: ≥ 1.0mm (designed for optimal current flow).
  * Compact form factor.
  * Labeled Top Overlay for team identification.
<div align="center">
 <img width="806" height="576" alt="image" src="https://github.com/user-attachments/assets/db039ff5-9964-404c-b6af-17d7af4d4c3f" />

</div>

## 🛠️ Bill of Materials (BOM)

| Component | Specifications | Mounting |
| :--- | :--- | :--- |
| **IC** | LM386 (DIP8) | THT |
| **Capacitors** | 2x 220uF, 1x 10uF | THT |
| **Resistors** | 1kΩ, 10Ω | THT |
| **TrimPot** | 10kΩ | THT |
| **Audio Jack** | 3.5mm (4-pin) | SMT |
| **Speaker** | 3W, 4Ω, 40mm | THT |

## 🏭 Manufacturing

The files located in the `Gerber_Files/` directory are fully compliant with industry standards. They can be zipped and sent to any PCB fabrication facility (such as JLCPCB, PCBWay, or local vendors) for physical production.

## 💡 Notes

* **Design Considerations:** The layout was designed with a minimum track width of 1mm to ensure robust power delivery and audio signal integrity.
* **Board Shape:** Designed for compact sizing using Altium’s Board Planning Mode.
* **Software:** Designed and validated using Altium Designer.

## 👨‍💻 Author

* **Nguyen Huy Long**
* *Electrical Engineering Student at VinUniversity*
* **Vu Hoang Lan**
* *Electrical Engineering Student at VinUniversity*
## 📂 Project Structure

```text
.
├── Audio_Amplifier.PcbDoc   # PCB Layout document
├── Audio_Amplifier.PrjPcb   # Project file
└── Audio_Amplifier.SchDoc   # Schematic document
├── Gerber_Files/            # Manufacturing files (Gerber)
│   ├── Audio_Amplifier-macro.APR_LIB
│   ├── Audio_Amplifier.EXTREP
│   ├── Audio_Amplifier.GBL      # Gerber Bottom Layer
│   ├── Audio_Amplifier.GBO      # Gerber Bottom Overlay
│   ├── Audio_Amplifier.GBP      # Gerber Bottom Paste
│   ├── Audio_Amplifier.GBS      # Gerber Bottom Solder
│   ├── Audio_Amplifier.GM       # Mechanical Layer (Profile)
│   ├── Audio_Amplifier.GM4      # Mechanical Layer (Board)
│   ├── Audio_Amplifier.GTL      # Gerber Top Layer
│   ├── Audio_Amplifier.GTO      # Gerber Top Overlay
│   ├── Audio_Amplifier.GTP      # Gerber Top Paste
│   ├── Audio_Amplifier.GTS      # Gerber Top Solder
│   ├── Audio_Amplifier.REP      # Gerber Report
│   └── Audio_Amplifier.apr      # Aperture file
├── NC_Drill_Files/          # NC Drill data for manufacturing
│   ├── Audio_Amplifier.DRR      # Drill Report
│   └── Audio_Amplifier.LDP      # Drill Layer Pair file
└── README.md
