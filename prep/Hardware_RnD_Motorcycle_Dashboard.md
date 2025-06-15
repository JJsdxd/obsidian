# 12-Week Plan for Hardware R&D Careers + Custom Motorcycle Dashboard Build

---

## 🧬 Goal
Build deep skills in digital and hardware design for high-end R&D roles **and** construct a custom motorcycle dashboard system using a repurposed Samsung Galaxy Core Prime Duos.

---

## ✅ Core Outcomes by Week 12
- ✅ Verilog and SystemVerilog (SV) for RTL design
- ✅ One RISC-V core or UART/SPI project run through synthesis + PnR
- ✅ Basic UVM testbench understanding
- ✅ GitHub + blog portfolio + internship-ready resume
- ✅ Embedded dashboard system featuring:
  - Navigation (offline GPS)
  - TPMS (BLE)
  - Voltage + ambient temp monitoring
  - Phone hardware mod (battery removal + USB-C swap)

---
Here’s a **clean, barebones list** of just the **parts and tools** you’ll need for both your **Hardware R&D workflow** and **motorcycle dashboard system**:

---

## 🧩 Components

### 🔧 Core Dashboard Hardware

- [ ]  Samsung Galaxy Core Prime Duos (rooted / modded)
- [ ]  USB Type-C breakout board or replacement port
- [ ]  5V/2A Buck converter (12V → 5V power from bike battery)
- [ ]  BLE TPMS sensors (x2 or x4)
- [ ]  I2C temperature sensor (e.g. BMP280 or LM35)
- [ ]  Analog voltage divider circuit (for battery monitoring)
- [ ]  Optional: ESP32 (if offloading TPMS parsing)

### ⚙️ Embedded + R&D Components

- [ ]  Breadboard + jumper wires
- [ ]  Verilog simulation tools (Yosys, GTKWave – software)
- [ ]  Logic analyzer (optional, USB-type)
- [ ]  Multimeter
- [ ]  Optional FPGA dev board (e.g., iCEBreaker, Basys 3)

---

## 🛠️ Tools & Supplies

- [ ]  Soldering iron (fine tip)
- [ ]  Solder wire + flux
- [ ]  Hot glue gun or epoxy (for port reinforcement)
- [ ]  Isopropyl alcohol (90%+) for cleaning
- [ ]  ESD-safe brush
- [ ]  Precision screwdriver set (Philips 000+)
- [ ]  Multimeter (basic digital type)
- [ ]  Optional: magnifier/loupe
---

----
## 📅 Phase 1: Digital & RTL Foundations (Weeks 1–4)

### Week 1: Digital Logic + Verilog Basics
- [ ] Review combinational logic, FSMs, latches vs flip-flops
- [ ] Simulate basic Verilog modules using HDLBits and GTKWave
- [ ] Build first AND/OR gate + counter modules

### Week 2: RTL Projects + Practice
- [ ] FSM-based traffic light controller
- [ ] Binary to gray code converter
- [ ] Simulate state machines and document in GitHub repo

### Week 3: Parameterization + Basic Testbenching
- [ ] Add parameterized widths using `parameter`
- [ ] Write testbench with `$display`, `$monitor`, `$finish`
- [ ] Use `generate` block for scalable instancing

### Week 4: Mini RISC-V Core (Datapath)
- [ ] Build 4-stage core: IF, ID, EX, WB
- [ ] Support ADD, SUB, AND, OR, IMM ops
- [ ] Simulate core with instruction sequence

---

## 📅 Phase 2: Toolchain & Open EDA Flow (Weeks 5–8)

### Week 5: Synthesis via Yosys
- [ ] Install Yosys and synthesize UART/ALU
- [ ] Analyze gate-level output and path delays
- [ ] Compare RTL vs netlist differences

### Week 6: Layout with OpenROAD
- [ ] Install OpenROAD with sky130
- [ ] Perform floorplan, placement, routing
- [ ] Export GDSII, visualize layout with KLayout

### Week 7: SoC Integration + RAM/IP
- [ ] Add instruction/data RAM + UART peripheral
- [ ] Define address map and simulate SoC top module

### Week 8: Recap + Blog + Debug
- [ ] Fix bugs, clean design
- [ ] Capture waveforms
- [ ] Blog: SoC design end-to-end

---

## 📅 Phase 3: Verification + Embedded Dashboard Build (Weeks 9–12)

### Week 9: SystemVerilog + UVM Intro
- [ ] Learn SV class, sequence, transaction, interface
- [ ] Implement UVM testbench for UART

### Week 10: Finalize UVM Testbench
- [ ] Scoreboard, coverage, corner-case tests
- [ ] Push to GitHub, document process

### Week 11: Embedded System – Dashboard Start
- [ ] Root and clean Galaxy Core Prime
- [ ] Remove bloatware or flash minimal ROM
- [ ] Inspect USB daughterboard + port clearance
- [ ] Begin battery removal plan + charging bypass
- [ ] Begin BLE TPMS parser (in Python or Android)

### Week 12: Dashboard Finalization + Display
- [ ] Replace micro-USB with USB-C manually (or breakout board)
- [ ] Test stable boot with direct power (with/without battery)
- [ ] Connect GPS and BLE modules
- [ ] Build Kivy or Qt UI: Nav + TPMS + battery/temp display
- [ ] Blog: Building a Custom Motorcycle Dashboard on Android Hardware

---

## 🧠 Optional Commuter Features
- [ ] Battery voltage reader (via analog sensor)
- [ ] Ambient temperature (via I2C sensor)
- [ ] GPS-based odometer + trip tracking
- [ ] Service alert logger (chain/oil interval)
- [ ] Real-time clock + system time from GPS

---

## 🛠️ Hardware Mods & Tools Checklist
- [ ] Isopropyl alcohol, brushes, ESD tools for cleaning
- [ ] USB Type-C breakout or donor port
- [ ] Fine soldering iron + flux + multimeter
- [ ] Voltage regulator 5V (buck converter from 12V)
- [ ] BLE TPMS sensors (AliExpress, Vesdo, etc.)
- [ ] Optional ESP32 for alternate TPMS path
- [ ] GPSD or Android LocationManager interface (depending on OS base)

---

## 🔔 Weekly Routine
- 3x 2.5hr focused sessions
- 1x lighter session (reading/blogging)
- 2 rest or catchup days

---

## 💼 Portfolio Output
- [ ] GitHub: RTL + SoC + TPMS code
- [ ] Blog: Hardware R&D projects + dashboard series
- [ ] Slide deck: SoC project + embedded hardware
- [ ] Internship-ready resume
- [ ] Operational motorcycle dashboard system with offline nav + BLE TPMS
