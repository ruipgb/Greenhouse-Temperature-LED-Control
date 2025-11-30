# Greenhouse Temperature & LED Control

Temperature monitoring and LED brightness control system for a small greenhouse.  
As the temperature changes, the brightness of several LEDs changes proportionally, giving a clear visual indication of the current thermal conditions.

---

## Overview

This project implements:

- 🌡️ **Temperature monitoring** of a greenhouse environment  
- 💡 **LED brightness control** — LEDs become brighter as the temperature increases (or follow a defined temperature–brightness profile)  
- 📊 **Simulations and analysis** to validate the behavior of the system before implementation

All the design details and results are documented in the attached PDF report.

---

## Technologies & Tools

- **LabVIEW** – main environment used to implement the monitoring and control logic  
- **Electronic simulation tools** (e.g. PSpice/OrCAD) – to design and test the LED driver and comparator circuits  
- **Temperature sensor + LEDs** – simulated and/or implemented as the main plant of the system

---

## Repository Contents

- `Greenhouse-Temperature-LED-Control-Report.pdf`  
  Complete report describing:
  - system requirements  
  - circuit design and simulations  
  - LabVIEW implementation  
  - test results and conclusions  

- `mostrar_temperatura.vi`  
  LabVIEW VI responsible for:
  - acquiring temperature  
  - processing the measured values  
  - updating LED brightness according to the temperature

- `Simulações/` (or ZIP file)  
  Simulation files used to design and validate the electronic part of the project (comparators, LED circuits, etc.).

---

## How It Works (summary)

1. The **temperature** of the greenhouse is measured or simulated.  
2. The **LabVIEW code** or electronic comparator processes the measured value.  
3. The **LEDs brightness** is adjusted according to the temperature:
   - lower temperature → dimmer LEDs  
   - higher temperature → brighter LEDs  

This allows quick visual feedback of the greenhouse thermal conditions.

---

## Future Work

Planned future improvements for this project include:

- ❄️ **Adding a cooling fan** controlled by the measured temperature  
  - fan automatically turns on above a configurable threshold  
  - closed-loop behaviour to keep the greenhouse within a safe temperature range  

- 📈 **More advanced control strategies**, such as hysteresis or PID-based control for the fan

---

If you want to see all the details, please check the PDF report in this repository.
