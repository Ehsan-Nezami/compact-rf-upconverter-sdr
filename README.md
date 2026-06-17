# Compact RF Upconverter (0–30 MHz)

## Overview

This project presents a compact redesign of an RF Upconverter originally based on an existing open design.
The goal was to improve practicality by introducing USB power input, full SMD implementation, and compact PCB layout while maintaining RF functionality.

This work also includes real-world validation using SDR tools.

---

## Key Improvements

* USB-powered operation (5V input)
* Full migration to SMD components
* Compact PCB layout redesign
* Improved manufacturability and assembly
* RF signal validation using SDR systems

---

## Hardware Design

The PCB was redesigned using EasyEDA with focus on:

* RF signal integrity
* Compact form factor
* Clean power distribution
* Practical assembly process

## PCB Design Note (Ground Plane Strategy)

Due to the prototype being assembled in a home lab environment, the ground polygon was intentionally simplified to improve soldering accessibility and reduce assembly complexity.

This design choice was made to facilitate manual assembly and debugging during the prototyping phase.

For improved RF performance in production versions, a full ground plane (polygon pour) can be restored or enhanced to further improve noise immunity and signal integrity.

Ground optimization is left open for future revisions depending on manufacturing requirements.

---

## Validation Setup

The board was tested using:

* HackRF One
* RTL-SDR

Signal conversion and RF behavior were analyzed using spectrum visualization tools.

---

## Results

The system was successfully validated in a real RF environment.
Converted signals were observable and consistent under SDR analysis.

---

## Project Structure

* `docs/` → schematic and documentation
* `hardware/` → gerber manufacturing files
* `images/` → PCB renders, physical board, and SDR results

---

## Skills Demonstrated

* RF Hardware Design
* PCB Design (EasyEDA)
* SMD Assembly Design
* SDR-Based Signal Validation
* System-Level Debugging

---

## Note

This project is part of my broader exploration of RF systems and hardware-level signal analysis.
