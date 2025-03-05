## **Experiment-3: Differential Amplifier Using MOSFETs**  

## **Aim:**  
To design and analyze a MOSFET-based differential amplifier by performing **DC analysis, transient analysis, and AC analysis** to understand its biasing, time-domain response, and frequency characteristics.
Design question: To Design a basic diffrential amplifier for the following specification Vdd=3.3V,P<=3mW,Vincm=1.72V,Vocm=1.8V,Vp=0.7V,Perform DC Analysis,Transient analysis,AC Analysis and extract the required parameters.


## **Theory:**  
A **MOSFET differential amplifier** is a fundamental circuit used in analog electronics, particularly in operational amplifiers, signal processing, and communication circuits. It amplifies the voltage difference between two input signals while suppressing common-mode signals.

![image](https://github.com/user-attachments/assets/21d8e303-e801-4207-b207-0866e33080ff)


## **Circuit Description:**  
A MOSFET differential amplifier consists of:  
1. **Two matched MOSFETs (M1 and M2)** forming the differential pair.  
2. **A current source (or resistor) at the source terminal** to provide a stable tail current.  
3. **Drain resistors (RD1 and RD2)** to convert current variations into voltage output.  
4. **Supply voltage (V_DD)** to power the circuit.  
5. **Gate terminals receiving the differential inputs (\(V_{in1}\) and \(V_{in2}\)).**

## **Circuit Diagram in LTSpice:**

  ![Diffamp](https://github.com/user-attachments/assets/e47c0b0d-dbfd-4687-9ecf-8b6e531b8d67)

  Below is the aspect ratio taken for the MOSFETs

  ![MosAspect](https://github.com/user-attachments/assets/a2aa8acd-dc60-4887-96c6-a7f8ff10083a)

 ## **1. DC Analysis (Biasing and Operating Point Calculation):**  
DC analysis helps determine the operating point (Q-point) of the MOSFETs.  
- Assume both transistors are in **saturation region**:  

  I_{D} = 1/2 * Mu_n * C_{ox} * {W}/{L} * (V_{GS} - V_{th})^2
  where:  
  - mu_n = Electron mobility  
  - C_{ox} = Oxide capacitance per unit area  
  - W/L = Aspect ratio of MOSFET  
  - V_{GS} = Gate-to-source voltage  
  - V_{th} = Threshold voltage  

  The total **tail current** I_{tail} is split equally between the two transistors when inputs are equal.  
  
  I_D1 = I_D2 = I_{tail}/2
  The **output DC voltage** is given by:  
  V_{out1} = V_{DD} - I_{D1} * R_D
  
  V_{out2} = V_{DD} - I_{D2} * R_D

After designing the amplifier we get the following values: 

![WhatsApp Image 2025-03-05 at 16 16 18_60a48cb9](https://github.com/user-attachments/assets/896b251e-a457-402b-b1d2-e074ce6f6fb9)

Below shown table gives the values obtained from the DC analysis which closely matches the design question

![DCanalysisDA](https://github.com/user-attachments/assets/bef5efe6-9805-49c1-8d25-eddb3a4c046e)

**We have an equation Vid = Vin1 - Vin2**

So when Vin1 is increased to 1.76 V and Vin2 is decreased to 1.68 V we get the following values:

![VidInc](https://github.com/user-attachments/assets/8a5ef67d-36ab-4e7d-bd87-b9646d921923)

Similarly, when Vin1 is decreased to 1.68 V and Vin2 is increased to 1.76 V we get the following values:

![VidDec](https://github.com/user-attachments/assets/eaf5e982-72cd-499a-8fbe-4a42d0d24e36)

**From this, we can infer that when Vid increases Vout1-Vout2 decreases and vice versa.**



## **2. Transient Analysis (Time-Domain Response):**  
- In transient analysis, we apply a time-varying input signal and observe the response at the output.  
- The circuit’s response to step, sinusoidal, or pulse inputs is analyzed.  
- This helps determine the amplifier's **rise time, fall time, and response to fast-changing signals.**

The below picture shows the waveforms obtained after transient analysis:

![Transient](https://github.com/user-attachments/assets/c4c9334a-67fa-4690-a039-403fb2012ece)

Vin Max= VoutCM + Vth

Vin Max= 1.8 V + 0.36 V = 2.16 V

Similarly, Vin Min= Vgs + Vp

Vin Min= 1.02 V + 0.7 V = 1.72 V

When Vin Max is applied in the amplitude of the input sine wave we get the following output of a square wave

![TransMaxDA (2)](https://github.com/user-attachments/assets/b4a3d312-33c5-4add-bc56-ed53fab1dd4e)

Similary for Vin Min, the output will be a square wave

![TransMinDA](https://github.com/user-attachments/assets/dfbdb0eb-d798-4541-bb7a-ec35e02638d3)

## **3. AC Analysis (Small-Signal Gain and Frequency Response):**  
- The small-signal model of the MOSFET is used for AC analysis.  
- The small-signal **differential gain** is given by:  
  A_d = -g_m*R_D 
  where g_m is the transconductance of the MOSFET  
  - Frequency response is determined by analyzing the **3dB bandwidth**.

We get the following frequency response for the given circuit:

![AcanalysisDA](https://github.com/user-attachments/assets/175a7fe8-763c-4cf1-887c-8a8f706e39b8)

The gain of this amplifier is 3.2 dB.

## **4. Inference:**

1. The source voltage increases as Vcm increases.
2. Vout decreases with increase in Vcm, due to increase in drain current Id.
3. If Vcm is too low the Mosfets turn off and the amplifier stops working.
4. If Vcm is too high the Mosfet enters the **triode region** which increases distortion.
5.  **Differential gain (A_d)** is high because the circuit amplifies differences between \( V_{in1} \) and \( V_{in2} \).
6.  **Common-mode gain (A_cm)** should ideally be **zero**, but due to imperfections, it is small but nonzero.
7.  A high **CMRR (\( A_d / A_{cm} \))** is desirable for good performance.
8.  The amplifier is **linear** only within a certain input range.
9.  Exceeding this range leads to **clipping, distortion, and loss of differential gain**.
10. **Choosing \( R_D \) and \( I_{tail} \)** properly balances gain, bandwidth, and power consumption.

## Conclusion

- A differential amplifier provides **high gain for differential signals** while rejecting common-mode noise.
- It has a **limited operating range**, and exceeding \( V_{CM} \) limits causes performance degradation.
- **Tail current stability, MOSFET matching, and frequency response** are crucial design factors.
- The amplifier is widely used in **op-amps, sensor interfaces, and analog signal processing** due to its excellent differential signal amplification properties.
