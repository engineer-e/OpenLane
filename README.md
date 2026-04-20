# OpenLane
Support Digital Electronic

Here is the complete GitHub `README.md` document with emojis, proper formatting, and a professional documentation style.

---


# 🚀 Learn Chip Design with OpenLane - Complete RTL-to-GDSII Series

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![OpenLane](https://img.shields.io/badge/OpenLane-1.0.2-green)](https://github.com/The-OpenROAD-Project/OpenLane)
[![Sky130](https://img.shields.io/badge/Sky130-PDK-orange)](https://github.com/google/skywater-pdk)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-red)](https://youtube.com)

A comprehensive 25-part video series teaching chip design from basics to complete SoC using open-source EDA tools.

---

## 📌 Table of Contents

- [What You Will Learn](#-what-you-will-learn)
- [Tools Covered](#-tools-covered)
- [Complete Series (25 Videos)](#-complete-series-25-videos)
- [Design Complexity Guide](#-design-complexity-guide)
- [Quick Commands](#-quick-commands)
- [System Requirements](#-system-requirements)
- [Resources](#-resources)
- [Tags](#-tags)
- [Credits](#-credits)

---

## 🎯 What You Will Learn

| Category | Topics |
|----------|--------|
| **Digital Design** | Verilog, RTL-to-GDSII, FSMs, Processors |
| **Analog Design** | Op-Amps, PLLs, Comparators, ADCs, DACs |
| **Mixed-Signal** | Sensors, Digital Readout, Bandgap References |
| **Tools** | OpenLane, Yosys, OpenROAD, Magic, Ngspice, KLayout |

---

## 🛠️ Tools Covered

| Tool | Purpose |
|------|---------|
| **OpenLane** | Complete RTL-to-GDSII flow |
| **Yosys** | Logic synthesis |
| **OpenROAD** | Floorplanning, placement, routing |
| **Magic** | Layout editing, DRC, GDSII streaming |
| **Ngspice** | Analog circuit simulation |
| **KLayout** | GDSII viewing and verification |
| **Xschem** | Schematic capture |
| **Icarus Verilog** | Digital simulation |
| **GTKWave** | Waveform viewing |
| **ALIGN** | Analog layout generation |

---

## 📚 Complete Series (25 Videos)

### 🟢 Beginner Level (Videos 1-5)

| # | Title | Topic |
|---|-------|-------|
| 1 | OpenLane Installation on Windows | WSL2 + Docker setup |
| 2 | AND Gate - Verilog to GDSII Complete Flow | RTL-to-GDSII |
| 3 | AND Gate at Transistor Level | CMOS + Ngspice |
| 4 | Simulating Verilog with Icarus & GTKWave | Digital simulation |
| 5 | Basic Logic Gates | OR, XOR, NOT, NAND, NOR |

### 🔵 Intermediate Level (Videos 6-12)

| # | Title | Topic |
|---|-------|-------|
| 6 | Sequential Logic - D Flip-Flop & Counter | Flip-flops, counters |
| 7 | 4-bit Adder/Subtractor in OpenLane | Arithmetic circuits |
| 8 | Multiplexers & Decoders - Complete Flow | Data selectors |
| 9 | Finite State Machine (FSM) Design | State machines |
| 10 | UART Transmitter/Receiver Implementation | Serial communication |
| 11 | Analog Design with Xschem + Ngspice | Analog simulation |
| 12 | CMOS Inverter Characterization & Layout | Inverter design |

### 🟠 Advanced Digital (Videos 13-18)

| # | Title | Topic |
|---|-------|-------|
| 13 | ALU (Arithmetic Logic Unit) Design | Arithmetic |
| 14 | Memory Controller with OpenRAM Integration | Memory |
| 15 | SPI/I2C Communication Interfaces | Protocols |
| 16 | FIR Filter Implementation | DSP |
| 17 | RISC-V Processor (Ibex/PicoRV32) | Processor design |
| 18 | AES Encryption Core Design | Cryptography |

### 🟣 Analog & Mixed-Signal (Videos 19-25)

| # | Title | Topic |
|---|-------|-------|
| 19 | Two-Stage Operational Amplifier Design | Op-Amp |
| 20 | Ring Oscillator & PLL Basics | Oscillators |
| 21 | Comparator & ADC Design | Converters |
| 22 | Digital-to-Analog Converter (DAC) | Converters |
| 23 | Bandgap Voltage Reference | Voltage reference |
| 24 | Temperature Sensor with Digital Readout | Sensors |
| 25 | Complete SoC - RISC-V + Analog Peripherals | System-on-Chip |

---

## 📊 Design Complexity Guide

| Design Type | Examples | Videos |
|-------------|----------|--------|
| **Basic Logic** | AND/OR/XOR, adders, muxes | 2, 5, 7, 8 |
| **Sequential** | Flip-flops, counters, FSMs | 6, 9 |
| **Arithmetic** | ALUs, multipliers, FPU | 13 |
| **Processors** | RISC-V cores, 8051 | 17 |
| **Memory** | SRAM, ROM, FIFO controllers | 14 |
| **Communication** | UART, SPI, I2C | 10, 15 |
| **DSP Blocks** | FIR filters, FFT | 16 |
| **Security** | AES, SHA, RSA | 18 |
| **Analog** | Op-Amps, PLLs, Comparators | 11, 12, 19, 20 |
| **Data Converters** | ADCs, DACs | 21, 22 |
| **Mixed-Signal** | Sensors, PMICs | 23, 24, 25 |

---

## 🔧 Quick Commands

### Enter OpenLane Environment
```bash
cd ~/OpenLane && make mount
```

### Run a Design
```bash
./flow.tcl -design DESIGN_NAME
```

### View Layout (KLayout)
```bash
klayout runs/*/results/final/gds/DESIGN_NAME.gds
```

### Simulate Verilog (Icarus + GTKWave)
```bash
iverilog -o sim tb.v DESIGN.v
vvp sim
gtkwave dump.vcd
```

### Analog Simulation (Ngspice)
```bash
ngspice circuit.cir
```

### View Layout (Magic)
```bash
magic -T sky130A.tech DESIGN_NAME.mag
```

---

## 💻 System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10/11, Ubuntu 20.04+, macOS | Windows 11 / Ubuntu 22.04 |
| **RAM** | 8 GB | 16 GB |
| **Disk Space** | 50 GB | 100 GB |
| **CPU** | Dual core | Quad core or more |
| **Docker** | Docker Desktop | Docker Desktop + WSL2 |

---

## 🔗 Resources

| Resource | Link |
|----------|------|
| **OpenLane** | [github.com/The-OpenROAD-Project/OpenLane](https://github.com/The-OpenROAD-Project/OpenLane) |
| **Sky130 PDK** | [github.com/google/skywater-pdk](https://github.com/google/skywater-pdk) |
| **Ngspice** | [ngspice.sourceforge.io](http://ngspice.sourceforge.io) |
| **Xschem** | [xschem.sourceforge.io](http://xschem.sourceforge.io) |
| **KLayout** | [www.klayout.de](https://www.klayout.de) |
| **OpenCores** | [opencores.org](https://opencores.org) |
| **OpenROAD** | [theopenroadproject.org](https://theopenroadproject.org) |

---

## 🏷️ Tags

`OpenLane`, `Chip Design`, `RTL to GDSII`, `VLSI`, `ASIC`, `OpenROAD`, `Sky130`, `Digital Design`, `Analog Design`, `Mixed Signal`, `IC Design`, `Semiconductor`, `RISC-V`, `Processor Design`, `CMOS`, `Ngspice`, `Verilog`, `Yosys`, `Magic VLSI`, `KLayout`, `GTKWave`, `Icarus Verilog`, `Xschem`, `Open Source EDA`

---

## 📅 Series Stats

| Metric | Value |
|--------|-------|
| **Total Videos** | 25 |
| **Total Duration** | ~15 hours |
| **Difficulty** | Beginner to Advanced |
| **Open Source Tools** | 10+ |
| **Target Technology** | Sky130 (130nm) |

---

## 🙏 Credits

| Organization | Contribution |
|--------------|--------------|
| **Efabless** | OpenLane framework |
| **Google** | Sky130 PDK |
| **OpenROAD Project** | Physical design tools |
| **Open Source EDA Community** | Yosys, Magic, Ngspice, KLayout, GTKWave, Icarus Verilog |

---

## 🔔 Stay Connected

- **Subscribe on YouTube** for weekly chip design tutorials
- **Leave comments** - I reply to every question
- **Source code** available at: [GitHub Repository Link](https://github.com/engineer-e/OpenLane/)

---



<div align="center">

**Made with ❤️ for the open-source chip design community**

[⬆ Back to Top](#-learn-chip-design-with-openlane---complete-rtl-to-gdsii-series)

</div>


---
