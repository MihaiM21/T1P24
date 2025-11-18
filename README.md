<!-- <p align=center>
  <img src="./lib/logo.png" width="200">
</p> -->

<h1 align="center">T1P24 – Aerodynamic RC Vehicle</h1>

<p align="center">
  <b>200 km/h real-world top speed · 350 km/h simulated aerodynamic limit · 0–100 km/h in 2.7s</b><br>
  <b>92 CFD simulations · 40+ structural iterations · Full ground-effect aero package</b><br>
  <b>Carbon-reinforced 3D-printed chassis · 100% custom embedded control firmware</b>
</p>

> [!NOTE]  
> T1P24 is an active development project.  
> All core systems (aero, drivetrain, control firmware) are functional, and new features are added continuously based on aerodynamic validation and testing.

---

## Table of Contents

- [About the Project](#about-the-project)
- [Technical Overview](#technical-overview)
- [Aerodynamics (CFD)](#aerodynamics-cfd)
- [Embedded System](#embedded-system)
- [Wireless Controller](#wireless-controller)
- [Performance](#performance)
- [Materials & Manufacturing](#materials--manufacturing)
- [Contact](#contact)

---

## About the Project

**T1P24** is a high-performance RC vehicle engineered using Formula 1 development principles.  
The project integrates **ground-effect aerodynamics, CFD validation, embedded control systems, wireless communication, and a high-power brushless drivetrain** into a compact test platform for motorsport research.

Key design objectives:

- Recreate Formula 1–style ground-effect aerodynamics at small scale  
- Validate aero performance using CFD (drag, downforce, stability)  
- Develop a custom control architecture (traction control, stabilization)  
- Iterate rapidly using 3D-printed carbon-reinforced structures  

---

## Technical Overview

### Hardware Architecture
- Brushless motor  
- **30A ESC** for high-power delivery  
- Steering servo 
- **NRF24L01** 2.4 GHz wireless module  
- Arduino Nano–based control unit  
- Dual-cell **4S 18650 10Ah** battery system  
- Full chassis printed in **PLA-CF** and **PETG**  
- Ackerman steering geometry for high-speed stability  

### Firmware Architecture
- Modular Arduino-based control firmware  
- Wireless packet decoding using RF24  
- PWM motor and steering control  
- Custom traction-control logic (slip detection)  
- Steering stabilization + fail-safe subsystems  
- Throttle mapping: **ECO / MID / MAX** modes  

---

## Aerodynamics (CFD)

Aerodynamic analysis performed using **SolidWorks Flow Simulation** with over **90 simulation runs**.

Validated results:

- **Drag coefficient (Cd):** 0.28  
- **Lift coefficient (Cl):** –0.25 (downforce generation)  
- Venturi-based ground-effect tunnels  
- Inwash airflow management and body shaping  
- Virtual wind tunnel tests at **200 km/h**  

Simulation outputs include:

- Pressure field maps  
- Velocity distribution  
- Streamline visualization  
- Aero stability behavior at high speed  

**Top speed capability:**  
- **200 km/h** measured experimentally  
- **≈350 km/h** aerodynamic limit in CFD  

---

## Embedded System

The onboard control unit manages:

- PWM motor control (ESC)  
- Steering servo regulation  
- NRF24 wireless communication stack  
- Traction-control algorithm  
- Mode switching logic  
- Fail-safe conditions (signal loss, invalid packets)  

The firmware is fully modular and designed for future expansion.

---

## Wireless Controller

Developed entirely in-house, featuring:

- Arduino Uno transmitter  
- Dual analog joysticks (throttle + steering)  
- I2C LCD for live feedback  
- NRF24 transmitter module  
- 3D-printed ergonomic shell  

Capabilities:

- Low-latency control  
- ECO / MID / MAX throttle modes  
- Stable long-range operation  

---

## Performance

- **0–100 km/h:** ~2.7 seconds  
- **Top speed (real-world):** 200 km/h  
- **Top speed (CFD-simulated):** ~350 km/h  
- Ground-effect underfloor provides high-speed stability  
- Traction-control reduces wheel slip under launch and corner exit  

---

## Materials & Manufacturing

- Structural components: **PLA-CF (carbon fiber reinforced)**  
- Aero surfaces and body: **PETG**  
- Fully 3D-printed, modular construction  
- Rapid prototyping and iterative testing workflow  

---

<p align=center>
  <b>Created by Mihai</b><br>
  Motorsport Software & Telemetry Engineer  
  <a href="https://github.com/MihaiM21">GitHub</a> • <a href="https://turnonehub.com">turnonehub.com</a>
</p>

