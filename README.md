# Three-Phase 3-Level T-Type Isolated Bidirectional AC-DC Converter for EV Charging

---

## 📌 Project Overview
This project presents the **design, modeling, and simulation** of a **Three-Phase 3-Level T-Type Isolated Bidirectional AC–DC Converter** intended for **high-power EV charging applications**.

The proposed converter supports **bidirectional power flow**, enabling both **grid-to-vehicle (G2V)** and **vehicle-to-grid (V2G)** operation with **high efficiency, power factor correction, and galvanic isolation**.

---

## 🚗 Application
- On-board and off-board **EV fast chargers**
- Bidirectional **V2G / G2V** systems
- Medium-voltage **AC–DC conversion**
- High-frequency isolated power converters

---

## 🎯 Objectives
- Design a **6.6 kW bidirectional EV charger**
- Implement **3-Level T-Type topology** for reduced switching losses
- Achieve **high power density** using high-frequency operation
- Design **control loops for current and DC-link voltage**
- Validate design using **MATLAB/Simulink and LTspice**

---

## ⚙️ System Specifications

| Parameter | Value |
|--------|------|
| Peak Power | 6.6 kW |
| AC Input Voltage | 300–415 V, 50 Hz |
| DC Link Voltage | 900–1100 V |
| Battery Voltage | 600–800 V |
| Switching Frequency | 120 kHz |
| Topology | 3-Level T-Type Isolated |
| Power Flow | Bidirectional |

---

## 🔧 Key Design Parameters
- **HF Transformer Turns Ratio**: 55:80  
- **Resonant Inductance**: 78.8 µH  
- **Resonant Capacitance**: 32.145 nF  
- **Split DC-Link Capacitance**: 660 µF  
- **Output DC Capacitance**: 440 µF  

---

## 🧠 Control Strategy
- d–q current control
- DC-link voltage regulation
- Output current control
- Closed-loop operation for bidirectional power flow

**Controllers Used**
- d-axis current controller: `5 + 1000/s`
- q-axis current controller: `5 + 1000/s`
- DC-link voltage controller: `0.1 + 10/s`

---

## 🧪 Tools & Software
- MATLAB / Simulink  
- LTspice  
- KiCad  
- Code Composer Studio (CCS)  

---

## 🔌 Power Electronics Design Highlights
- **SiC MOSFET-based switching**
- **ACPL-W346 isolated gate driver**
- **MGJ2D051505BSC isolated gate power supply**
- Optimized **snubber, DC-link, and resonant components**
- EMI-aware **gate loop and PCB layout**

---

## 📊 Switch Selection Summary
The SiC MOSFET **G3R40MT12K (GeneSiC)** was selected based on minimum total loss:

| Switch | Total Loss |
|------|-----------|
| G3R40MT12K | **12.04 W** |
| IMZA120R040M1H | 15.83 W |
| SCT4036KRHR | 17.23 W |

---

## 🌡️ Thermal Design
- 3 switches per heat sink
- Total loss per heat sink: **36.1 W**
- Selected heat sink: **CR-201-75E**
- Thermal resistance: **2.6 K/W**

---

## 📁 Repository Structure
- `MATLAB_Simulink/` → Converter & control models  
- `LTspice/` → Gate driver & sensor simulations  
- `Hardware/` → PCB schematics & footprints  
- `Firmware/` → CCS-based control code  
- `Documentation/` → Detailed design report  

---

## 🚀 Key Outcomes
- High-efficiency **6.6 kW isolated EV charger design**
- Reduced switching and conduction losses
- Stable closed-loop control
- EMI-aware hardware design approach

---

## 🔭 Future Scope
- Hardware prototype development
- Experimental V2G validation
- EMI compliance testing
- Extension to **11 kW / 22 kW chargers**

---

## 📜 License
This project is intended for **academic and research purposes only**.
