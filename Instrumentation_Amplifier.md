# Instrumentation Amplifier

## Design Question
Design an instrumentation amplifier using 3 op-amp configuration with the following constraints, R1=R3=10k ohm, R2=R4=20k ohm, R5=R6=10k ohm. Calculate Adm for Rg= 10,100,1k,10k,20k ohms. Find Acm and CMRR for each case. Use LTSpice Simulator.

## Theory
An **Instrumentation Amplifier (IA)** is a type of differential amplifier that offers **high input impedance**, **high common-mode rejection ratio (CMRR)**, and **precise gain control**, making it ideal for accurate and low-noise signal amplification.

### Key Features:
- **Three-op-amp configuration:** Most instrumentation amplifiers use three operational amplifiers—two as buffers and one as a differential amplifier.
- **High input impedance:** Prevents loading of the signal source.
- **Low output impedance:** Ensures compatibility with various loads.
- **Adjustable gain:** Often set by a single resistor, simplifying design.
- **Excellent CMRR:** Effectively rejects noise and interference common to both input lines, which is crucial in environments with electrical noise.

### Applications:
- Medical instrumentation (e.g., ECG, EEG)
- Sensor signal amplification (e.g., strain gauges, thermocouples)
- Industrial process controls

Instrumentation amplifiers are widely used when small differential signals need to be accurately amplified in the presence of a noisy environment.

![image](https://github.com/user-attachments/assets/f8cee726-1ec5-455c-bcfd-a30f9f3f79ea)

### Circuit Diagram

![image](https://github.com/user-attachments/assets/86ffc17f-4107-47b3-ad3c-d681a00af8b8)

