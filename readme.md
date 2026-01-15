# Inverting Op-Amp Amplifier – Schematic & PCB

## Overview

This repository contains the schematic and PCB design for an inverting operational amplifier (op-amp) experiment board.
The board is intended for educational and laboratory use, allowing users to explore closed-loop gain, feedback, and signal behaviour in a practical, hands-on way.

The circuit implements a classic inverting amplifier configuration, where the gain is determined by the ratio of the feedback and input resistors selected during board population.

## Circuit Description

The op-amp is configured as an inverting amplifier with:

- Configurable input resistor (Rin)
- Configurable feedback resistor (Rf)
- Closed-loop gain defined by:

$$
𝐴𝑣 = −\frac{𝑅_𝑓}{𝑅_{𝑖}}
$$

By choosing different resistor values, users can easily experiment with different gain magnitudes while observing the effect on the output signal.

## Power Supply

The PCB includes dedicated power supply terminals to support flexible operation:

- Designed to work with dual-rail supplies (e.g. ±9 V, ±12 V, ±15 V)
- Supply rails are clearly labeled on the PCB
- No onboard regulation is included — the op-amp is powered directly from the external supply

> ⚠️ Ensure the selected op-amp is operated within its specified supply voltage limits.

## Test & Measurement Points

To support analysis and troubleshooting, the board includes clearly marked probe pads for oscilloscope or multimeter connections:

- Input signal (Vin)
- Output signal (Vout)
- Ground reference
- (Optional) supply rail probe points, if populated

These pads allow users to:

- Measure gain directly
- Observe phase inversion
- Inspect clipping and saturation
- Compare theoretical vs measured performance

## Intended Use

This board is suitable for:

- Op-amp laboratory experiments
- Demonstrating inverting amplifier behaviour
- Teaching closed-loop gain and feedback concepts
- Signal measurement with oscilloscopes and function generators
- Quick resistor-swap experiments without rewiring a breadboard

## Repository Contents

- Schematic files – complete circuit diagram of the inverting amplifier
- PCB layout files – board layout matching the schematic
- (Optional) Gerber files – for PCB fabrication
- This README

## Notes & Best Practices

- Populate only one set of input/feedback resistors at a time unless explicitly designed for parallel options.
- Use precision resistors for accurate gain measurements.
- Always connect the ground reference of the signal generator and oscilloscope to the PCB ground.
- Avoid driving the output beyond the op-amp’s output swing limits to prevent distortion.

## License / Usage

This design is intended for educational and experimental use.
Feel free to modify and adapt it for teaching, labs, or personal projects.