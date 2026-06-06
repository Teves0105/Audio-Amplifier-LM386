# Audio Amplifier PCB Design (LM386) 🔈

A professional-grade Printed Circuit Board (PCB) design for a mono Audio Amplifier based on the **LM386** operational amplifier. This project was developed as a laboratory assignment for **ELEC2010: Introduction to Circuits for Electrical Engineers** at **VinUniversity**.

The project covers the end-to-end hardware design lifecycle, including schematic capture, component footprint definition, PCB layout design with clearance constraints, and the generation of manufacturing files.

## 📋 Features & Specifications

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

## 📂 Project Structure

```text
.
├── Altium_Source/           # Original Altium Designer project files
│   ├── Audio_Amplifier.PrjPcb   # Project file
│   ├── Audio_Amplifier.SchDoc   # Schematic document
│   └── Audio_Amplifier.PcbDoc   # PCB Layout document
├── Gerber_Files/            # Manufacturing files
│   ├── Audio_Amplifier.TXT      # NC Drill file
│   ├── Audio_Amplifier.GBL      # Gerber Bottom Layer
│   ├── Audio_Amplifier.GTL      # Gerber Top Layer
│   ├── Audio_Amplifier.DRR      # Drill Report
│   └── ...                      # Additional manufacturing layers
└── README.md
🛠️ Bill of Materials (BOM)ComponentSpecificationsMountingICLM386 (DIP8)THTCapacitors2x 220uF, 1x 10uFTHTResistors1kΩ, 10ΩTHTTrimPot10kΩTHTAudio Jack3.5mm (4-pin)SMTSpeaker3W, 4Ω, 40mmTHT🏭 ManufacturingThe files located in the Gerber_Files/ directory are fully compliant with industry standards. They can be zipped and sent to any PCB fabrication facility (such as JLCPCB, PCBWay, or local vendors) for physical production.💡 NotesDesign Considerations: The layout was designed with a minimum track width of 1mm to ensure robust power delivery and audio signal integrity.Board Shape: Designed for compact sizing using Altium’s Board Planning Mode.Software: Designed and validated using Altium Designer.👨‍💻 AuthorNguyễn Huy LongElectrical Engineering Student at VinUniversity
