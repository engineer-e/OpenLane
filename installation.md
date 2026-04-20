Here is the proper GitHub `README.md` documentation for your OpenLane Installation Guide video.

---


# OpenLane Tutorial: From RTL to Silicon - Complete Installation Guide

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![OpenLane](https://img.shields.io/badge/OpenLane-1.0.2-green)](https://github.com/The-OpenROAD-Project/OpenLane)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Mac-lightgrey)](https://github.com/The-OpenROAD-Project/OpenLane)
[![YouTube](https://img.shields.io/badge/YouTube-Subscribe-red)](https://youtube.com/playlist?list=PLkvtzcMGVO88SVBMTKp0brqD1bdHWzBUP&si=eb-BRW7-K4NInlUO)


---

## 📌 Table of Contents

- [What is OpenLane?](#-what-is-openlane)
- [What You Will Learn](#-what-you-will-learn)
- [Tools Covered in This Series](#-tools-covered-in-this-series)
- [System Requirements](#-system-requirements)
- [Installation Steps](#-installation-steps)
- [Verifying Installation](#-verifying-installation)
- [Directory Structure](#-directory-structure)
- [Common Issues and Solutions](#-common-issues-and-solutions)
- [Quick Commands](#-quick-commands)
- [Resources](#-resources)
- [Next Steps](#-next-steps)
- [Support](#-support)

---

## 🔬 What is OpenLane?

OpenLane is an automated **RTL-to-GDSII** ASIC implementation flow based on:

| Tool | Purpose |
|------|---------|
| **OpenROAD** | Floorplanning, placement, CTS, routing |
| **Yosys** | RTL synthesis and technology mapping |
| **Magic** | GDSII streaming and layout editing |
| **Netgen** | Layout vs. Schematic (LVS) verification |
| **KLayout** | GDSII viewing and DRC |

It transforms your Register Transfer Level (RTL) design into a final GDSII file ready for fabrication at a foundry like SkyWater.

---

## 🎯 What You Will Learn

- ✅ Install WSL2 on Windows 10 or 11
- ✅ Set up Docker Desktop with WSL2 integration
- ✅ Install OpenLane from GitHub
- ✅ Run the test design to verify installation
- ✅ Understand the OpenLane directory structure

---

## 🛠️ Tools Covered in This Series

| Tool | Purpose |
|:-----|:--------|
| **OpenLane** | Main RTL-to-GDSII flow controller |
| **Yosys** | RTL synthesis and technology mapping |
| **OpenROAD** | Floorplanning, placement, CTS, routing |
| **Magic** | GDSII streaming and layout editing |
| **Ngspice** | Transistor-level simulation |
| **KLayout** | GDSII viewing and DRC |
| **Netgen** | LVS verification |
| **Icarus Verilog** | Digital simulation |
| **GTKWave** | Waveform viewing |

---

## 💻 System Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **OS** | Windows 10 (version 2004+) | Windows 11 |
| **RAM** | 8 GB | 16 GB |
| **Disk Space** | 50 GB | 100 GB |
| **CPU** | Dual core | Quad core or more |
| **Admin Access** | Required | Required |

---

## 📥 Installation Steps

### Step 1: Install WSL2

Open **PowerShell as Administrator** and run:

```powershell
wsl --install -d Ubuntu
```

Restart your computer when prompted.

### Step 2: Launch Ubuntu

After restart, launch **Ubuntu** from the Start Menu. Create a username and password when prompted.

### Step 3: Update Ubuntu

Run these commands in the Ubuntu terminal:

```bash
sudo apt update
sudo apt upgrade -y
```

### Step 4: Install Docker Desktop

1. Download Docker Desktop from [docker.com](https://www.docker.com/products/docker-desktop/)
2. Install with default settings
3. Launch Docker Desktop

### Step 5: Enable WSL Integration

In Docker Desktop:

1. Go to **Settings** → **General**
2. Check **Use WSL 2 based engine**
3. Go to **Resources** → **WSL Integration**
4. Enable integration for your Ubuntu distribution
5. Click **Apply & Restart**

### Step 6: Install OpenLane

In the Ubuntu terminal:

```bash
cd ~
git clone --depth 1 https://github.com/The-OpenROAD-Project/OpenLane.git
cd OpenLane
make
```

The `make` command will download the Docker image and set up the environment.

---

## ✅ Verifying Installation

Run the test design to verify everything works:

```bash
make test
```

**Expected output:**

```
Basic test passed
```

This confirms OpenLane is correctly installed and the Sky130 PDK is ready.

---

## 📁 Directory Structure

After installation, your OpenLane directory looks like this:

```
OpenLane/
├── designs/          # Your design folders
├── docker/           # Docker configuration
├── docs/             # Documentation
├── scripts/          # Helper scripts
├── Makefile          # Build and run commands
└── README.md         # Documentation
```

---

## ⚠️ Common Issues and Solutions

| Issue | Solution |
|-------|----------|
| `docker: command not found` | Enable WSL integration in Docker Desktop settings |
| Permission denied | Restart your computer after Docker installation |
| Slow performance | Work in `~/OpenLane`, not `/mnt/d/` |
| `python3-venv not found` | Run `sudo apt install python3-venv` |
| `make: command not found` | Run `sudo apt install make` |
| Docker Desktop shows "Stopped" | Launch Docker Desktop from Windows Start Menu |

---

## 🔧 Quick Commands

| Action | Command |
|--------|---------|
| Enter OpenLane | `cd ~/OpenLane && make mount` |
| Run test | `make test` |
| Clean installation | `make clean` |
| Update OpenLane | `git pull && make` |

---

## 🔗 Resources

| Resource | Link |
|----------|------|
| **OpenLane GitHub** | [github.com/The-OpenROAD-Project/OpenLane](https://github.com/The-OpenROAD-Project/OpenLane) |
| **Docker Desktop** | [docker.com/products/docker-desktop](https://www.docker.com/products/docker-desktop/) |
| **OpenLane Docs** | [openlane.readthedocs.io](https://openlane.readthedocs.io) |
| **Sky130 PDK** | [github.com/google/skywater-pdk](https://github.com/google/skywater-pdk) |
| **OpenROAD** | [theopenroadproject.org](https://theopenroadproject.org) |

---

## 📢 Next Video

**Title:** AND Gate - Verilog to GDSII Complete Flow

**Topics:**
- Design AND gate in Verilog
- Simulate with Icarus Verilog
- View waveforms in GTKWave
- Run through full OpenLane flow
- Generate GDSII file

---

## 🏷️ Tags

`OpenLane`, `RTL to GDSII`, `Chip Design`, `ASIC`, `OpenROAD`, `Sky130`, `VLSI`, `Open Source EDA`, `Digital Design`, `IC Design`, `WSL2`, `Docker`, `Yosys`, `Magic VLSI`, `KLayout`, `Netgen`

---

## ❓ Support

- **Questions?** Leave a comment on the YouTube video
- **Issues?** Check the [OpenLane GitHub Issues](https://github.com/The-OpenROAD-Project/OpenLane/issues)
- **Source Code:** [github.com/engineer-e/OpenLane](https://github.com/engineer-e/OpenLane)

---

## 🔔 Stay Connected

- **Subscribe** for weekly chip design tutorials
- **Hit the bell** to never miss a video

---

<div align="center">

**Made with ❤️ for the open-source chip design community**

[⬆ Back to Top](#openlane-tutorial-from-rtl-to-silicon---complete-installation-guide)

</div>


