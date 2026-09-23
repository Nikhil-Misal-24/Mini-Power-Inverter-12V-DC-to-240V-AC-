# ⚡ Mini Power Inverter

### `12V DC → 240V AC`

<p align="center">
  <img src="https://img.shields.io/badge/Power%20Electronics-Inverter-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Input-12V%20DC-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Output-240V%20AC-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/PCB-Custom-orange?style=for-the-badge">
</p>

<p align="center">
  <b>A compact switching-based DC–AC power inverter developed as a practical power-electronics and PCB design project.</b>
</p>

---

## 🚀 Project at a Glance

> **A compact 12V DC → 240V AC inverter built around an IR2153 switching/driver stage, IRLZ24 MOSFET power switches, and a transformer-based voltage conversion stage.**

The project focuses on turning a theoretical inverter topology into a **real, compact hardware implementation**, covering the complete development cycle from circuit design to PCB fabrication, assembly, soldering, testing, and troubleshooting.

### 🔋 Input

**12V DC**

### ⚡ Conversion

**High-frequency switching + transformer**

### 🔌 Output

**240V AC nominal**

### 🧩 Controller

**IR2153**

### 🔧 Power Switch

**IRLZ24 MOSFET**

### 📐 PCB

**~65 × 35 mm**

---

# 🧠 How It Works

```text
                 ┌──────────────────┐
                 │   12V DC INPUT   │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │     IR2153       │
                 │ Oscillator /     │
                 │ Gate Driver      │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │   IRLZ24         │
                 │ MOSFET Switching │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │   TRANSFORMER    │
                 │   Step-Up Stage  │
                 └────────┬─────────┘
                          │
                          ▼
                 ┌──────────────────┐
                 │   240V AC OUT    │
                 └──────────────────┘
```

### 🔄 Conversion Process

**01 — DC Input**

A 12V DC source supplies energy to the inverter.

**02 — Oscillation**

The IR2153 generates the switching signal required to control the power MOSFET stage.

**03 — Power Switching**

IRLZ24 MOSFETs rapidly switch the DC supply through the transformer primary.

**04 — Voltage Transformation**

The transformer steps up the switched waveform to a high-voltage AC output.

**05 — AC Output**

The secondary side provides a nominal 240V AC output under the designed operating conditions.

---

# ⚙️ Technical Specifications

| Parameter      | Value                          |
| -------------- | ------------------------------ |
| 🔋 Input       | **12V DC**                     |
| ⚡ Output       | **240V AC nominal**            |
| 🔄 Conversion  | **DC → AC**                    |
| 🎛️ Driver     | **IR2153**                     |
| 🔧 MOSFET      | **IRLZ24**                     |
| 🧲 Transformer | **Step-Up Transformer**        |
| 📐 PCB Size    | **~65 × 35 mm**                |
| 🛠️ PCB        | **Custom Designed**            |
| 🎯 Application | **Educational / Experimental** |

> Actual output voltage, waveform, efficiency and power capability depend on the transformer, component values, input supply, switching configuration and load.

---

# 🧩 Hardware Architecture

### Control & Switching Stage

The **IR2153** forms the oscillator/driver section responsible for generating the switching signals.

### Power Stage

The **IRLZ24 MOSFETs** handle the high-current switching required to transfer energy from the 12V DC source into the transformer.

### Voltage Conversion Stage

The transformer performs the required voltage step-up from the low-voltage switching stage to the high-voltage AC output.

---

# 🛠️ Design Journey

```text
Concept
   ↓
Circuit Design
   ↓
Component Selection
   ↓
Schematic Development
   ↓
PCB Layout
   ↓
PCB Fabrication
   ↓
Component Assembly
   ↓
Soldering
   ↓
Testing
   ↓
Debugging
   ↓
Final Hardware
```

This project was developed with a focus on **practical hardware implementation**, not just simulation.

---

# 🖥️ PCB Design

The inverter was implemented on a compact custom PCB.

### PCB Design Goals

* Compact footprint
* Practical component placement
* Reduced high-current path length
* Organized power-stage routing
* Easy component identification
* Reliable soldering and assembly
* Hardware-oriented layout

**Approximate PCB Dimensions**

```text
65 mm × 35 mm × 19 mm
```

---

# 📸 Project Gallery

> Replace the paths below with your actual repository images.

### 🔧 Final PCB

<p align="center">
  <img src="Screenshot 2026-03-02 201450.png" width="800">
</p>

### 🖥️ PCB Layout

<p align="center">
  <img src="images/pcb-layout.png" width="800">
</p>

### 📐 Schematic

<p align="center">
  <img src="images/schematic.png" width="800">
</p>

---

# 🔬 Engineering Focus

This project explores several important electronics concepts:

| Area                | Implementation           |
| ------------------- | ------------------------ |
| Power Electronics   | DC–AC conversion         |
| Switching           | MOSFET-based switching   |
| Gate Driving        | IR2153                   |
| Power Semiconductor | IRLZ24                   |
| Magnetic Components | Transformer              |
| PCB Engineering     | Custom PCB               |
| Hardware            | Through-hole components  |
| Testing             | Hardware debugging       |
| Manufacturing       | PCB assembly & soldering |

---

# 💡 What I Learned

Through this project, I gained practical experience with:

* Switching inverter architectures
* MOSFET power switching
* Gate-driver circuits
* Transformer-based voltage conversion
* Power PCB layout
* High-current PCB routing
* Component selection
* Hardware assembly
* Soldering
* Circuit debugging
* Practical testing
* Power-electronics safety considerations

---

# 🔮 Future Development

The next version could include:

* [ ] Output voltage feedback
* [ ] Closed-loop voltage regulation
* [ ] Over-current protection
* [ ] Short-circuit protection
* [ ] Thermal protection
* [ ] Battery low-voltage cutoff
* [ ] Output voltage monitoring
* [ ] Frequency monitoring
* [ ] Improved waveform quality
* [ ] Higher conversion efficiency
* [ ] Better thermal management
* [ ] Protective enclosure

---

# 📊 Project Status

<p align="center">

| Development Stage   | Status                  |
| ------------------- | ----------------------- |
| Circuit Concept     | ✅ Completed             |
| Component Selection | ✅ Completed             |
| Schematic           | ✅ Completed             |
| PCB Design          | ✅ Completed             |
| PCB Fabrication     | ✅ Completed             |
| Assembly            | ✅ Completed             |
| Hardware Testing    | 🔧 In Progress / Update |
| Optimization        | 🚀 Future               |

</p>

---

# ⚠️ HIGH-VOLTAGE SAFETY

<div align="center">

### ⚠️ WARNING — 240V AC IS DANGEROUS

</div>

This project produces potentially **lethal high voltage**.

Do not touch exposed output terminals or conductors while the inverter is powered.

Always:

* Use proper insulation.
* Maintain adequate PCB clearance and creepage.
* Disconnect the DC supply before making modifications.
* Use appropriate measurement equipment.
* Avoid working alone around high voltage.
* Enclose the final hardware appropriately.

**This project is intended for educational and experimental purposes.**

---

# 📁 Repository Structure

```text
Mini-Power-Inverter-12V-DC-to-240V-AC/
│
├── 📁 Images/
│   ├── final-pcb.jpg
│   ├── pcb-layout.png
│   └── schematic.png
│
├── 📁 PCB/
│   ├── schematic/
│   └── layout/
│
├── 📁 Documentation/
│
├── 📄 README.md
└── 📄 LICENSE
```

---

# 🎯 Project Objectives

### Primary Objective

Develop a compact practical inverter capable of converting a **12V DC source into a nominal 240V AC output** using a switching-based power stage.

### Secondary Objectives

* Understand inverter topology.
* Gain practical MOSFET switching experience.
* Design a compact PCB.
* Understand transformer-based voltage conversion.
* Develop hardware debugging skills.
* Build practical power-electronics experience.

---

# 👨‍💻 Developer

## Nikhil Misal

**Electronics & Communication Engineering Student**

**Focus Areas**

`Embedded Systems` · `PCB Design` · `Electronics Hardware` · `Power Electronics` · `IoT` · `Microcontrollers`

---

# 🌟 Why This Project?

This project represents a complete **hardware development workflow**:

```text
Idea
 ↓
Engineering
 ↓
Design
 ↓
PCB
 ↓
Assembly
 ↓
Testing
 ↓
Optimization
```

Rather than treating electronics as only theoretical concepts, this project focuses on **building, testing, debugging, and improving real hardware.**

---

<p align="center">

### ⚡ Built with Electronics • Designed with Purpose • Tested in Hardware

</p>

<p align="center">

<b>⭐ If you find this project useful, consider starring the repository.</b>

</p>

---

## 📜 License

This repository is intended for educational and experimental use.

Refer to the repository's `LICENSE` file for the applicable licensing terms.
