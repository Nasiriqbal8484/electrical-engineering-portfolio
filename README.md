# Electrical Engineering Portfolio

A growing collection of practical electrical-engineering tools and learning projects focused on **power systems, solar PV, battery energy storage systems (BESS), and EV charging infrastructure**.

## About this repository

This repository documents hands-on engineering practice through small, understandable Python projects. Each project begins with transparent assumptions and fundamental engineering equations, then can be expanded into a more complete analysis or design tool.

> **Engineering note:** These tools are for learning, preliminary calculations, and portfolio demonstration. Final engineering designs must be checked against applicable standards, equipment datasheets, project requirements, and qualified engineering review.

## Projects

### 1. Three-Phase Power Calculator
**Folder:** `power-systems/`

Calculates balanced three-phase line current and apparent power from active power, line-to-line voltage, and power factor.

**Topics:**
- Three-phase power relationships
- Line-to-line voltage
- Power factor
- kW, kVA, and current

### 2. Solar PV String Sizing Tool
**Folder:** `solar-pv/`

Performs a basic PV string voltage check using module Voc/Vmp, module count, inverter limits, and a cold-temperature Voc correction.

**Topics:**
- PV module voltage
- Series string sizing
- Inverter DC limits
- MPPT operating window
- Temperature coefficient of Voc

### 3. BESS Sizing Calculator
**Folder:** `bess/`

Estimates required nominal battery energy from a target delivered energy while accounting for usable depth of discharge, system efficiency, and design margin.

**Topics:**
- MW and MWh
- Storage duration
- Depth of discharge
- Efficiency
- Nominal vs. delivered energy

### 4. EV Charger Energy Calculator
**Folder:** `ev-charging/`

Estimates AC energy drawn, approximate energy delivered to a vehicle, charging duration, and charger utilization.

**Topics:**
- Charger power
- Charging-session energy
- Charging duration
- Efficiency
- Utilization

## Repository structure

```text
electrical-engineering-portfolio/
├── README.md
├── power-systems/
│   ├── README.md
│   └── three_phase_calculator.py
├── solar-pv/
│   ├── README.md
│   └── pv_string_sizing.py
├── bess/
│   ├── README.md
│   └── bess_sizing.py
├── ev-charging/
│   ├── README.md
│   └── charger_energy_calculator.py
└── docs/
    └── project-roadmap.md
```

## Running the calculators

These starter scripts require only Python 3 and the standard library.

Example:

```bash
python power-systems/three_phase_calculator.py --power-kw 22 --voltage-v 400 --power-factor 0.95
```

Each script includes default example values, so it can also be run without arguments.

## Development roadmap

Planned additions include:

- Cable sizing and voltage-drop calculations
- Short-circuit and protection-study examples
- Expanded PV string sizing using equipment-specific limits
- Solar DC/AC ratio analysis
- BESS augmentation and degradation scenarios
- EV charging utilization and energy-cost analysis
- CSV/Excel input and engineering reports
- Automated validation tests

See [`docs/project-roadmap.md`](docs/project-roadmap.md) for the staged development plan.

## Skills demonstrated

- Electrical engineering calculations
- Python automation
- Engineering assumptions and documentation
- Git and GitHub workflow
- Renewable-energy and EV infrastructure concepts

## Responsible use

Do not use these scripts as the sole basis for equipment selection, protection settings, construction design, or safety-critical decisions. Verify results independently and against the governing codes, standards, project specifications, and manufacturer data.
