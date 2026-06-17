# Compact RF Upconverter (0–30 MHz)

![Project Cover](images/cover.png)

## Overview

This project is a compact RF upconverter designed to enable HF signal reception (0–30 MHz) using SDR platforms such as HackRF and RTL-SDR.

The design is based on an existing open-source architecture and has been redesigned for improved practicality, compactness, and ease of assembly.

The implementation includes full hardware redesign, USB power integration, and real-world SDR validation.

---

## Key Improvements

* USB-powered architecture (5V input)
* Full migration to SMD components
* Compact PCB layout optimization
* Improved manufacturability for prototype assembly
* SDR-based RF validation (HackRF / RTL-SDR)

---

## Hardware Design

The PCB was redesigned in EasyEDA with focus on:

* Controlled RF signal routing
* Compact board footprint
* Stable power distribution
* Practical home-lab assembly considerations

---

## PCB Design Note (Ground Strategy)

Due to prototyping in a home-lab environment, the ground polygon was intentionally simplified to improve soldering accessibility and reduce assembly complexity.

This trade-off was made to support faster iteration and easier debugging during early-stage development.

For production-level designs, a full ground plane is recommended to improve RF performance, reduce noise coupling, and enhance overall signal integrity.

---

## Power Supply Considerations

For optimal RF measurement accuracy, a clean power source such as a battery or high-quality power bank is recommended instead of a laptop USB port.

Laptop USB power may introduce switching noise and ground contamination, which can degrade RF signal purity and measurement stability.

---

## Validation Setup

The system was evaluated using:

* HackRF One
* RTL-SDR

Signal behavior and frequency conversion were verified using spectrum analysis tools.

---

## Results

The system successfully demonstrated stable frequency conversion under real RF conditions.

Converted signals were clearly observable and consistent in SDR-based spectrum analysis.

---

## Project Structure

* `docs/` → schematic and documentation
* `hardware/` → Gerber manufacturing files
* `images/` → PCB renders, physical board, and SDR results

---

## Skills Demonstrated

* RF Hardware Design
* PCB Design (EasyEDA)
* SMD Implementation
* SDR Signal Analysis
* System-Level Debugging

---

## Note

This project is part of an ongoing exploration of RF systems and hardware-level signal processing.
