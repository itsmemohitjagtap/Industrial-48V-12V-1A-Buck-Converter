# LMR38020 Buck Converter PCB Design

📌 **Project Overview**

This project is a **PCB design and power electronics practice project** for a wide-input **DC-DC Buck Converter** based on the **Texas Instruments LMR38020**.

The converter is designed to step down a **14V–48V input supply** to a regulated **12V output at 1A**, operating at **400kHz switching frequency**.

This project focuses on professional schematic capture, component selection, switching regulator calculations, and PCB layout best practices using **Altium Designer 25.2.1**. It emphasizes correct power loop routing, thermal considerations, and EMI-aware layout techniques.

Fabrication and hardware validation are not included in this version. The objective is to strengthen practical knowledge in industrial-grade power supply PCB design.

---

## 🎯 Features

- Wide input voltage range (14V – 48V)
- Regulated 12V output @ 1A
- 400kHz switching frequency configuration
- Synchronous buck topology
- Adjustable output via feedback network
- Properly designed power loop layout
- Thermal pad grounding with via stitching
- Industrial-style PCB layout discipline

---

## 🧠 Learning Outcomes

- Understanding synchronous buck converter operation  
- Calculating switching frequency (RT resistor selection)  
- Inductor and capacitor selection based on ripple requirements  
- Designing feedback divider network  
- Power loop minimization in PCB layout  
- SW node copper control for EMI reduction  
- Thermal pad design and heat dissipation strategy  
- Practical application of datasheet-driven design  

---

## 🗂️ Files Included

| File | Description |
|------|-------------|
| `lmr38020_schematic.pdf` | Complete schematic diagram |
| `pcb_layout.png` | 2D PCB layout image |
| `pcb_3d_view.png` | 3D PCB visualization |
| `design_calculations.md` | Design equations and component selection details |
| `bom.xlsx` | Bill of Materials |

---

## 🔩 Key Components Used

- LMR38020SDDAR (HSOIC-8 with PowerPAD)
- Shielded Power Inductor (~68µH)
- X7R Ceramic Input and Output Capacitors
- Bootstrap Capacitor (100nF)
- RT Resistor (~66kΩ for 400kHz)
- Feedback Resistors for 12V Output

---

## 🖥️ Software Used

- **Altium Designer 25.2.1**

---

## 🔧 How It Works

- The LMR38020 operates as a synchronous step-down (buck) converter.
- The high-side MOSFET switches at 400kHz.
- Energy is transferred through the inductor to the output capacitor.
- The feedback network regulates the output voltage to 12V.
- The RT resistor sets the switching frequency.
- Proper PCB layout minimizes switching noise and improves thermal performance.

---

## ⚡ Design Considerations

- High-current switching loop kept minimal
- Dedicated ground strategy
- Exposed PowerPAD connected to ground with thermal vias
- Controlled SW node copper area to reduce EMI
- Wide traces used for VIN, SW, VOUT, and PGND
- Feedback trace routed away from switching node

---

## 🧑‍💻 Designed By

**Mohit Jagtap**  
Electronics & Telecommunication Engineering  
Dr. D. Y. Patil Institute of Engineering Management and Research  
Akurdi, Pune  

---
