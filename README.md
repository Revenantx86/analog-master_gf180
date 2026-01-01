# analog-master_gf180
Analog design library for gf180nm technology



# GF180MCU Analog Building Blocks

**Author:** [Refik Yalcin]  
**Technology:** GlobalFoundries 180nm MCU (gf180mcuC)  
**Tools:** Xschem, Ngspice, Magic, KLayout, OpenLane/OpenROAD (optional)

## 📖 Overview
This repository contains a personal library of reusable analog IP cells designed for the GF180MCU open-source PDK. The goal is to build a "standard cell" library for analog design, allowing for rapid prototyping of complex mixed-signal systems by instantiating pre-verified primitives (mirrors, diff-pairs, opamps).

## 📂 Repository Structure

```text
.
├── doc/                 # Global documentation (pdk specs, characterization plots)
├── lib/                 # The Core Library (Reusable Cells)
│   ├── amplifiers/      # OpAmps, OTAs, Diff-pairs
│   ├── bias/            # Current mirrors, Bandgaps, Bias distributors
│   └── logic/           # 3.3V Logic gates for mixed-signal control
├── sim/                 # Top-level integration testbenches
├── scripts/             # Python/Shell scripts for batch simulation/measurement
├── xschemrc             # Xschem startup configuration
└── magicrc              # Magic startup configuration