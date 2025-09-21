# 🖥️ RISC-V Reference SoC Tapeout Program VSD.

Welcome to my journey through the **SoC Tapeout Program VSD**!

This repository documents my **week-by-week progress** with tasks inside each week.

<div align="center">

> *"This program guides participants through designing a complete System-on-Chip (SoC), from fundamental RTL design to GDSII layout, using open-source tools. As part of India’s largest collaborative RISC-V tapeout project, it enables over 3,500 contributors to create silicon and contribute to the growth of the national semiconductor ecosystem."*

</div>

<div align="center">

```
📝 RTL Design → 🔄 Synthesis → 🏗️ Physical Design → 🎯 Tapeout Ready
```

</div>

---
## 📅 Week 0 

---

### 1. 💡 Chip Modelling

→ Begin with chip-level functional modeling.

→ Develop a C model to represent the intended functionality.

---

### 2. 🛠 GCC Compilation

→ Compile the C model specifications using GCC.

---

### 3. 📄 C Model Specifications

→ Define the chip specifications in C.

→ Serves as input for:

i) 🧪 Testbench Development (C Language): Validates the functional correctness of the chip.

ii) 🔧 RTL Hardware Design (Verilog).

---

### 4. 🔧 RTL Design

→ Describe hardware at the Register Transfer Level (RTL) using Verilog.

→Key components:

i) ⚙️ Processor → Converted into a Gate-Level Netlist (Synth PI).

ii) 🖧 Peripherals/IPs → Packaged as Macros (Synth RTL).

iii) 🎛 Analog IPs → Modeled at Functional RTL Level.

---

### 5. 🧩 SoC Integration (GPIOs)

→ Combine processor, peripherals, macros, and analog IPs into a complete System-on-Chip (SoC).

---

### 6. 🏗 Physical Implementation

→ Conduct floorplanning, placement, and routing for the integrated SoC.

---

### 7. 🧩 Macro & Analog IP Integration

→ Integrate hard and soft macros along with analog IP blocks into the design.

---

### 8. 📐 GDSII Output 

→ Export the design into GDSII format, the standard format for IC layout data.

---

### 9. ✅Design Verification

→ DRC (Design Rule Check):**Confirms the layout meets fabrication rules.

→ LVS (Layout vs. Schematic):** Verifies the layout corresponds to the schematic design.

---

### 10. 🏭 Tapeout → Chip Fabrication

→ Send the finalized design to a semiconductor foundry (tapeout).

→ Begin the physical fabrication of the chip.

---
## Flow Chart 

<img width="1024" height="1024" alt="Gemini_Generated_Image_jcgdf2jcgdf2jcgd" src="https://github.com/user-attachments/assets/ed6804d6-fbc2-4b64-9397-1c46e826d02e" />

---

## 📌 Key Workflow Overview
The VLSI design flow can be summarized as:

1)💡 High-level C modeling

2)🛠 Compilation and functional specification

3)🔧 RTL hardware implementation

4)🧩 SoC integration and synthesis

5)🏗 Physical design and verification

6)📐 GDSII generation and 🏭 tapeout for manufacturing

---
## 🙏 **Acknowledgment**

<div align="center">

### 🏆 **Program Leadership & Support**

I am thankful to [**Kunal Ghosh**](https://github.com/kunalg123) and Team **[VLSI System Design (VSD)](https://vsdiat.vlsisystemdesign.com/)** for the opportunity to participate in the ongoing **RISC-V SoC Tapeout Program**.

