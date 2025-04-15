# Instrumentation Amplifier

## Design Question
Design an instrumentation amplifier using 3 op-amp configuration with the following constraints, R1=R3=10k ohm, R2=R4=20k ohm, R5=R6=10k ohm. Calculate Adm for Rg= 10,100,1k,10k,20k ohms. Find Acm and CMRR for each case. Use LTSpice Simulator. Take Vcc= 15V.

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

## Circuit Diagram

![image](https://github.com/user-attachments/assets/86ffc17f-4107-47b3-ad3c-d681a00af8b8)

## Calculations:

To find out Adm we use the formula:

![image](https://github.com/user-attachments/assets/3e2bfb16-51af-4437-a0ea-d17d0ba5cfe6)

To find Vid we use the formula:

**Vid = Vsat/Adm** 

(Vsat= 90% of Vcc)

We do this for each case.

Performing the calculations, we get,

![WhatsApp Image 2025-04-15 at 22 01 55_03ca5c88](https://github.com/user-attachments/assets/a6595af4-9987-4c1d-912c-29ebc4a1ce37)

#### For RG = 10 ohms,

**Transient Analysis:**

![image](https://github.com/user-attachments/assets/bb3d1771-cd8e-4238-9f87-36004cf1aa7c)

Vout p-p = 1.44 uV.

#### For RG = 100 ohms,

**Transient Analysis:**

![image](https://github.com/user-attachments/assets/b7d8323a-ecbe-46b0-8046-0fe2b5465664)

Vout p-p = 14.61 uV

#### For RG = 1k ohms,

**Transient Analysis:**

![image](https://github.com/user-attachments/assets/ccf84c65-379b-4c10-a7f3-97484a42b7bd)

Vout p-p = 146.3 uV

#### For RG = 10k ohms,

![image](https://github.com/user-attachments/assets/02634855-229b-4973-97fe-dbfccd63cf98)

Vout p-p = 974.8 uV

#### For RG = 20k ohms,

![image](https://github.com/user-attachments/assets/14bfb3b7-958a-4398-a988-92e29f656057)

Vout p-p = 1.462 mV

## Results:

**Finding Acm and CMRR for each case:**

![WhatsApp Image 2025-04-15 at 22 21 03_2f6ec407](https://github.com/user-attachments/assets/1dda7104-8a82-402c-b616-305841a93590)
![WhatsApp Image 2025-04-15 at 22 21 04_957a6ca0](https://github.com/user-attachments/assets/e935196d-b462-4b45-a1e1-8afec3234bcd)

## Inference:


