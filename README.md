# Open-Source 3D Printer Rebuild & Conversion  
### CubeX Trio → SKR V1.4 Turbo | TMC2209 | Marlin Firmware

This project documents my full rebuild of a commercial CubeX Trio 3D printer by stripping out the proprietary electronics and converting the machine into a modern open-source platform powered by an SKR V1.4 Turbo controller and TMC2209 stepper drivers.

The goal of this rebuild is to modernize an older industrial machine, improve print quality, enable open-source freedom, and understand the hardware–firmware stack at a deep systems-engineering level.

---

## 🚀 Key Features

- Converted proprietary CubeX Trio electronics to a fully open-source architecture  
- Reverse-engineered all stepper pinouts, thermistor values, heater wiring, and endstop logic  
- Designed a new wiring harness compatible with the SKR V1.4 Turbo  
- Upgraded to TMC2209 drivers for quiet operation, current control, and improved motion  
- Configured Marlin firmware from scratch with proper kinematics, steps/mm, thermistor tables  
- Documented teardown, troubleshooting, firmware flashing, and hardware tuning  
- Added CAD-ready mounts for boards, fans, and cable management  

---

## 🛠️ Repository Layout

### `firmware/`
Contains Marlin configuration files, flashing instructions, and notes about tuning stepper drivers, PID tuning, and EEPROM storage.

### `hardware/`
Documentation of wiring, thermistor tables, reverse-engineered pinouts from the original CubeX Trio, and the complete bill of materials.

### `cad/`
STL/STEP files for mounts, brackets, and cable routing components.

### `project_notes/`
Work logs, troubleshooting notes, tuning guides, and mechanical adjustments.

### `media/`
Before/after photos, wiring harness pictures, and diagrams.

---

## 🧩 Why This Project?

Modern 32-bit controllers dramatically improve reliability, noise, motion control, and accessibility.  
This rebuild transforms a locked-down printer into a fully customizable open-source machine—ideal for engineering learning and experimentation.

This project also demonstrates hands-on experience across:

- Embedded systems  
- Hardware integration  
- Firmware configuration  
- Diagnostics and troubleshooting  
- PCB-level wiring and electronics  
- Mechanical adaptation and CAD  

---

## 🔧 Hardware Overview

- **Controller:** SKR V1.4 Turbo  
- **Drivers:** TMC2209 (UART mode)  
- **Hotend:** Stock CubeX assembly (thermistor table: TBD)  
- **Heated Bed:** 24V MOSFET-switched bed  
- **Motors:** NEMA 17 (original CubeX), tested for microstepping and current rating  
- **Power Supply:** OEM 24V supply  

Full bill of materials is in `hardware/bill_of_materials.md`.

---

## 📦 Status

✔ Electronics fully replaced  
✔ Wiring harness rebuilt  
✔ Marlin boots successfully  
✔ Endstops & motion verified  
⬜ Bed leveling calibration  
⬜ Extruder calibration  
⬜ Final enclosure & cable management  
⬜ PLA test print

---

## 📚 License

MIT License.
