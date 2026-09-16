# BJT H-Bridge Motor Driver

<p align="center">
  <img src="images/assembled-pcb-angle.jpeg" width="750">
</p>

## Overview

This project presents the design and implementation of a **discrete BJT-based H-Bridge motor driver** for bidirectional DC motor control.

The main objective of this project was to design, simulate, manufacture, and test a complete motor driver circuit from the initial schematic stage to a physical PCB prototype.

The project demonstrates practical experience in:

- Electronic circuit design
- Power switching circuits
- PCB design and fabrication
- Hardware prototyping
- Motor control fundamentals

The schematic and PCB were designed using **Altium Designer**, and the final circuit was manufactured and assembled as a functional hardware prototype.

---

# Project Objectives

The main goals of this project were:

- Designing a transistor-based H-Bridge topology
- Controlling the direction of a DC motor
- Implementing a custom PCB design
- Selecting appropriate switching and protection components
- Fabricating and assembling the final PCB
- Testing the hardware implementation

---

# Working Principle

An H-Bridge is a motor driver topology that allows changing the polarity applied to a DC motor.

By controlling the switching states of the four BJT transistors, the direction of current through the motor can be changed, allowing:

- Forward rotation
- Reverse rotation
- Motor stop state


Basic operation:

```
          +V Supply

              |
        +-----+-----+
        |           |
       Q1           Q2
        |           |
        +---- Motor +
        |
        Motor
        |
        +---- Motor -
        |           |
       Q3           Q4
        |           |
        +-----+-----+

              |
             GND
```

---

# Hardware Design

## Main Components

| Component | Function |
|---|---|
| BJT Transistors | Switching elements for H-Bridge |
| Flyback Diodes | Protection against voltage spikes |
| Resistors | Base current limiting and biasing |
| Motor Terminals | DC motor connection |
| Power Terminals | Supply input |
| Custom PCB | Hardware implementation |

---

# Circuit Design

The complete schematic was designed using **Altium Designer**.

The design includes:

- Four-transistor H-Bridge switching stage
- Base drive networks
- Motor connection interface
- Protection components
- Power supply section


Project files:

```
altium/
│
├── Sheet1.SchDoc
├── PCB1.PcbDoc
└── PCB_Project1.PrjPCB
```

---

# PCB Design

The PCB layout was developed in Altium Designer.

The design process included:

- Component placement
- Routing optimization
- Through-hole footprint selection
- Manufacturing preparation
- 3D PCB verification


## PCB Layout

<p align="center">
  <img src="images/pcb-layout.png" width="800">
</p>


## 3D PCB View

<p align="center">
  <img src="images/pcb-3d-view.png" width="800">
</p>

---

# Hardware Fabrication

After completing the PCB design, the board was fabricated and assembled.

The final prototype includes:

- BJT switching stage
- Protection components
- Motor connection terminals
- Power input section


## Manufactured PCB

<p align="center">
  <img src="images/assembled-pcb.jpeg" width="700">
</p>


<p align="center">
  <img src="images/assembled-pcb-angle.jpeg" width="700">
</p>

---

# Repository Structure

```
BJT-H-Bridge-Motor-Driver

│
├── altium
│   ├── Sheet1.SchDoc
│   ├── PCB1.PcbDoc
│   └── PCB_Project1.PrjPCB
│
├── images
│   ├── pcb-layout.png
│   ├── pcb-3d-view.png
│   ├── assembled-pcb.jpeg
│   └── assembled-pcb-angle.jpeg
│
└── README.md
```

---

# Design Workflow

The project workflow consisted of:

```
Circuit Concept

      ↓

Schematic Design

      ↓

PCB Layout

      ↓

3D Verification

      ↓

PCB Fabrication

      ↓

Component Assembly

      ↓

Hardware Testing
```

---

# Skills Demonstrated

This project demonstrates practical skills in:

- Analog Electronics
- Digital Electronics
- Power Electronics
- BJT Switching Circuits
- DC Motor Control
- PCB Schematic Design
- PCB Layout Design
- Altium Designer
- Hardware Prototyping
- Circuit Debugging

---

# Engineering Considerations

## Switching Design

The H-Bridge design required careful consideration of transistor switching behavior, base drive requirements, and protection against inductive load effects.

## PCB Implementation

The schematic was converted into a manufacturable PCB while considering:

- Component placement
- Routing constraints
- Power connections
- Mechanical organization

## Prototype Validation

The manufactured PCB was assembled and evaluated to verify the physical implementation of the designed circuit.

---

# Possible Improvements

Future improvements could include:

- Replacing BJTs with MOSFETs for higher efficiency
- Adding PWM speed control
- Adding current sensing protection
- Integrating a microcontroller control interface
- Implementing closed-loop motor speed control

---

# Author

Arghavan Memari
Erfan Feghhi
Alireza Montajab

Electronics Design | Embedded Systems | PCB Design
