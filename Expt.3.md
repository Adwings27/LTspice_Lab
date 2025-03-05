**Differential Amplifier Using MOSFETs**  

**Aim:**  
To design and analyze a MOSFET-based differential amplifier by performing **DC analysis, transient analysis, and AC analysis** to understand its biasing, time-domain response, and frequency characteristics.


**Theory:**  
A **MOSFET differential amplifier** is a fundamental circuit used in analog electronics, particularly in operational amplifiers, signal processing, and communication circuits. It amplifies the voltage difference between two input signals while suppressing common-mode signals.


**Circuit Description:**  
A MOSFET differential amplifier consists of:  
1. **Two matched MOSFETs (M1 and M2)** forming the differential pair.  
2. **A current source (or resistor) at the source terminal** to provide a stable tail current.  
3. **Drain resistors (RD1 and RD2)** to convert current variations into voltage output.  
4. **Supply voltage (\(V_{DD}\))** to power the circuit.  
5. **Gate terminals receiving the differential inputs (\(V_{in1}\) and \(V_{in2}\)).**  

---

**Types of Analysis:**

**1. DC Analysis (Biasing and Operating Point Calculation):**  
DC analysis helps determine the operating point (Q-point) of the MOSFETs.  
- Assume both transistors are in **saturation region**:  
  \[
  I_{D} = \frac{1}{2} \mu_n C_{ox} \frac{W}{L} (V_{GS} - V_{th})^2
  \]
  where:  
  - \( \mu_n \) = Electron mobility  
  - \( C_{ox} \) = Oxide capacitance per unit area  
  - \( W/L \) = Aspect ratio of MOSFET  
  - \( V_{GS} \) = Gate-to-source voltage  
  - \( V_{th} \) = Threshold voltage  

- The total **tail current** \(I_{tail}\) is split equally between the two transistors when inputs are equal.  
  \[
  I_{D1} = I_{D2} = \frac{I_{tail}}{2}
  \]
- The **output DC voltage** is given by:  
  \[
  V_{out1} = V_{DD} - I_{D1} R_D
  \]
  \[
  V_{out2} = V_{DD} - I_{D2} R_D
  \]

**2. Transient Analysis (Time-Domain Response):**  
- In transient analysis, we apply a time-varying input signal and observe the response at the output.  
- The circuit’s response to step, sinusoidal, or pulse inputs is analyzed.  
- This helps determine the amplifier's **rise time, fall time, and response to fast-changing signals.**  

**3. AC Analysis (Small-Signal Gain and Frequency Response):**  
- The small-signal model of the MOSFET is used for AC analysis.  
- The small-signal **differential gain** is given by:  
  A_d = g_m*R_D
  where g_m (transconductance) is:  
  g_m = \frac{\partial I_D}{\partial V_{GS}} = \mu_n C_{ox} \frac{W}{L} (V_{GS} - V_{th})
  \]
- The **common-mode gain** is ideally low, and the **common-mode rejection ratio (CMRR)** is calculated as:  
  \[
  CMRR = \frac{A_d}{A_c}
  \]
- Frequency response is determined by analyzing the **3dB bandwidth**, which depends on the **parasitic capacitances and load capacitance.**

---

### **Conclusion:**  
By performing **DC analysis, transient analysis, and AC analysis**, we can evaluate the MOSFET differential amplifier’s operating point, dynamic response, and frequency characteristics. This helps in designing high-performance analog circuits with optimized gain, bandwidth, and noise performance.
