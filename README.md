

# Multi-Output Power Supply PCB (12V → 5V → 3.3V)

## 📌 Overview

This project presents the design and PCB implementation of a multi-stage DC power supply.
The system converts a 12V DC input into regulated 5V and 3.3V outputs using a switching regulator followed by a low-dropout regulator.

---

## ⚡ Architecture

12V → Buck Converter (LM2596) → 5V → LDO (TLV755) → 3.3V

---

## 🔧 Features

* 12V to 5V step-down using LM2596 switching regulator
* 5V to 3.3V regulation using TLV755 LDO
* EMI-aware PCB layout design
* Optimized high-current switching loops
* Controlled SW node for reduced noise
* Clean feedback routing for stable regulation
* 2-layer PCB with dedicated ground plane

---

## 🧠 Design Highlights

### 🔁 Switching Loop Optimization

The high-current switching loop (VIN → IC → diode → GND) is minimized to reduce EMI and switching noise.

### 🎯 Feedback Routing

The feedback trace is routed away from noisy regions such as the inductor and switching node to ensure stable output regulation.

### 🌍 Grounding Strategy

A solid ground plane is implemented on the bottom layer to provide low-impedance return paths and improve noise performance.

### 🔌 Power Integrity

A combination of bulk electrolytic capacitors and ceramic capacitors is used to ensure effective filtering across low and high frequencies.

---

## 📷 PCB Design

### Schematic
![Schematic](Dual-Stage%20Step-Down%20Power%20Supply%20(12V%20to%205V)%20-%20Copy/images/3d3.png)


### Layout

![Layout](Dual-Stage%20Step-Down%20Power%20Supply%20(12V%20to%205V)%20-%20Copy/images/3d.png)

### 3D View 1

![3D view](Dual-Stage%20Step-Down%20Power%20Supply%20(12V%20to%205V)%20-%20Copy/images/3d1.png)

### 3D View 2

![3D view](Dual-Stage%20Step-Down%20Power%20Supply%20(12V%20to%205V)%20-%20Copy/images/3d2.png)

---

## ⚠️ Project Status

⚠️ This project is currently **design-complete but not hardware-tested**.

The focus of this work is on:

* Circuit design
* Component selection
* PCB layout optimization

---

## 🔬 Planned Validation

* Output voltage verification (5V and 3.3V)
* Ripple measurement using an oscilloscope
* Thermal performance analysis
* Load regulation testing
* Efficiency measurement

---

## 🛠 Tools Used

* KiCad (Schematic & PCB Design)

---

## 📚 Future Improvements

* Replace LDO with a high-efficiency buck converter for 3.3V
* Add protection circuits (TVS, fuse, reverse polarity protection)
* Improve thermal performance for higher load currents
* Further compact layout optimization

---

## 📄 License

This project is open-source and intended for educational and learning purposes.

---
