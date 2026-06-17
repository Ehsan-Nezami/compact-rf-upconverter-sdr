# Compact RF Upconverter (0–30 MHz)

## Overview

This project presents a compact redesign of an RF upconverter based on an existing open-source design.

The goal of this work was to improve practical usability by introducing USB power input, migrating the design to full SMD implementation, and optimizing the PCB layout while preserving RF functionality.

The implementation was validated through real-world testing using SDR-based measurement tools.

---

## Key Improvements

* USB-powered operation (5V input)
* Full migration to SMD components
* Compact PCB layout redesign
* Improved manufacturability and assembly process
* RF signal validation using SDR systems (HackRF / RTL-SDR)

---

## Hardware Design

The PCB was redesigned using EasyEDA with a focus on:

* RF signal integrity and controlled routing
* Compact form factor optimization
* Clean power distribution strategy
* Practical assembly and prototyping considerations

---

## PCB Design Note (Ground Plane Strategy)

Due to the prototype being assembled in a home lab environment, the ground polygon was intentionally simplified to improve soldering accessibility and reduce assembly complexity.

This trade-off was made to facilitate rapid prototyping and debugging during early-stage development.

For production-level implementations, a continuous ground plane (polygon pour) is recommended to improve RF performance, reduce noise coupling, and enhance signal integrity.

Ground optimization is intentionally left open for future hardware revisions.

---

## Validation Setup

The system was evaluated using:

* HackRF One
* RTL-SDR

RF signal behavior and frequency conversion were analyzed using spectrum visualization tools.

---

## Results

The system was successfully validated in a real RF environment.

Converted signals were clearly observable and consistent during SDR-based spectrum analysis.

---

## Project Structure

* `docs/` → schematic and documentation
* `hardware/` → Gerber manufacturing files
* `images/` → PCB renders, physical board, and SDR measurement results

---

## Skills Demonstrated

* RF Hardware Design
* PCB Design (EasyEDA)
* SMD Implementation
* SDR-Based Signal Analysis
* System-Level Debugging

---

## Power Supply Considerations

For improved noise performance during testing, a clean power source such as a battery or high-quality power bank is recommended instead of a laptop USB port.

Laptop USB ports may introduce switching noise and ground contamination, which can affect RF signal purity and measurement accuracy.

Using an isolated or battery-powered supply helps reduce unwanted noise coupling into the RF front-end and improves measurement reliability during spectrum analysis.

---

## Note

This project is part of a broader exploration of RF systems and hardware-level signal analysis.
