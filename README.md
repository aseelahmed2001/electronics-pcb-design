# Electronics & PCB Design Portfolio

A collection of electronics and PCB design projects developed using **Altium CircuitMaker**, covering schematic capture, analog and digital circuit design, PCB layout and routing, component selection, design verification, and manufacturing preparation.

The projects in this repository were developed while completing the *Crash Course Electronics and PCB Design* course on Udemy and were used to build practical experience with electronic hardware development.

The portfolio progresses from course-guided PCB designs to a customized microcontroller-based hardware project.

---

## Projects

### 1. SimonDuino Custom Hardware

**Status:** Schematic complete — custom PCB design in progress

A customized microcontroller-based Simon game hardware platform built around the **ATmega328P**.

The overall architecture originated from the course project, while this implementation was adapted for currently available components, revised pin assignments, modified interconnections, and a custom PCB arrangement currently under development.

Key hardware includes:

- ATmega328P microcontroller
- 8-to-3 priority encoder
- Eight player/control buttons
- Four game LEDs
- Audio amplifier and speaker output
- USB-to-UART interface
- ICSP programming header
- Arduino Nano-style I/O headers
- 9 V input with regulated 5 V supply
- Reset and difficulty controls

**Skills demonstrated:**

`Embedded Hardware` `ATmega328P` `Component Selection` `Pin Mapping` `USB-UART` `Digital Logic` `Audio Electronics` `Power Supply Design`

➡️ [View SimonDuino Project](simon-duino-custom/)

---

### 2. 555 Timer Mini-Organ

**Status:** PCB design and manufacturing files complete

A 12-note electronic mini-organ based on a **555 timer astable oscillator**.

Twelve selectable timing resistors modify the oscillator frequency to generate musical notes from C4 to B4.

The project includes:

- 555 timer oscillator
- 12-note resistor selection network
- 5 V regulated power supply
- Transistor output stage
- Test points
- PCB layout and routing
- Bill of Materials
- Gerber files
- NC drill files

**Skills demonstrated:**

`555 Timer` `Analog Electronics` `Oscillator Circuits` `Transistor Circuits` `PCB Routing` `BOM Generation` `Gerber Generation`

➡️ [View 555 Timer Mini-Organ](555-timer-organ/)

---

### 3. Magic Wand LED Sequencer

**Status:** PCB design and manufacturing files complete

A sequential LED circuit combining a **555 timer clock generator**, binary counter, and **3-to-8 decoder**.

The 555 timer generates a continuous clock signal which advances a binary counter. The resulting binary value is decoded to sequentially control an eight-LED array.

The project includes:

- 555 timer clock generator
- Adjustable timing circuit
- SN74HC393 binary counter
- 74HC138 3-to-8 decoder
- Eight-LED output array
- 4.5 V battery supply
- PCB layout and routing
- Gerber files
- NC drill files

**Skills demonstrated:**

`Digital Logic` `Binary Counters` `Decoders` `555 Timer` `LED Driving` `PCB Design` `PCB Manufacturing Preparation`

➡️ [View Magic Wand Project](magic-wand/)

---

## Technical Skills

### Electronics

- Analog and digital circuit fundamentals
- 555 timer circuits
- RC timing and oscillator circuits
- Transistor circuits
- Digital logic
- Binary counters and decoders
- Microcontroller hardware integration
- Voltage regulation
- Supply filtering and decoupling
- LED and audio output circuits
- USB-to-UART interfaces
- ICSP programming interfaces

### PCB Design

- Schematic capture
- Component selection
- Datasheet interpretation
- Symbol and footprint assignment
- Component placement
- PCB routing
- Power and ground routing
- PCB layer management
- Design Rule Checking
- 3D PCB inspection
- Test-point implementation

### Manufacturing Preparation

- Bill of Materials generation
- Gerber generation
- NC drill generation
- PCB manufacturing output preparation

---

## Tools

- **Altium CircuitMaker**
- Electronic component datasheets
- PCB 3D visualization
- Gerber and manufacturing output tools

---

## Repository Structure

```text
electronics-pcb-design/
│
├── README.md
│
├── 555-timer-organ/
│   ├── README.md
│   ├── design_files/
│   ├── images/
│   └── manufacturing/
│
├── magic-wand/
│   ├── README.md
│   ├── design_files/
│   ├── images/
│   └── manufacturing/
│
└── simon-duino-custom/
    ├── README.md
    ├── design_files/
    ├── images/
    └── manufacturing/
```

Each project contains its own README with additional information about the circuit architecture, design process, project status, and available design/manufacturing files.

---

## Project Progression

The projects represent a progression in electronics and PCB design complexity:

```text
Magic Wand
555 Timer + Digital Logic
        │
        ▼
555 Timer Mini-Organ
Analog Timing + Output Electronics
        │
        ▼
SimonDuino
Microcontroller + Digital Logic + USB + Audio + Custom Hardware
```

The first projects focus on practical circuit implementation and PCB development, while the SimonDuino project extends these skills into component adaptation and embedded hardware integration.

---

## Current Development

The **SimonDuino custom PCB** is currently under development.

Upcoming work includes:

- Custom component placement
- PCB routing
- Design Rule Checking
- 3D PCB verification
- Manufacturing file generation
- PCB fabrication
- Hardware assembly and testing

---

## Project Context

These projects were developed while completing the **Crash Course Electronics and PCB Design** course on Udemy.

The Magic Wand and 555 Timer Mini-Organ are course-guided projects used to develop practical experience with electronic circuits and PCB design.

The SimonDuino project builds upon a course-provided circuit architecture but has been adapted for currently available components, revised pin assignments, modified schematic connections, and a custom PCB design.

The purpose of this repository is to document my practical development in **electronics, PCB design, and embedded hardware engineering**.
