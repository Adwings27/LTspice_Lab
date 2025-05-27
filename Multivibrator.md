# Monostable multivibrator
## Aim
### Generate pulse of width 0.5ms using 555 timer IC.
## Theory
Monostable multivibrators have only one stable state that is used to generate a single o/p pulse of a specified width either high or low when an external trigger pulse is applied. This trigger pulse starts a timing cycle, which causes the o/p to change its state at the time of start of timing cycle and continues in the second state which is decided by the time constant of the capacitor C and resistor R until it returns to its original state. It will continue in this state until another i/p signal is received. Monostable multivibrators can produce a much longer rectangular waveform. When a trigger pulse is applied externally then the leading edge of the waveform rises with the externally applied trigger. Here, trailing edge depends upon the RC time constant of the feedback components used. This RC time constant may be varied with time to produce a series of pulses which have a fixed time delay to the original triggered pulse.
## Working
The output of the monostable multivibrator using 555 timer remains in its stable state until it gets a trigger. In monostable 555 multivibrator, when both the transistor and capacitor are shorted then this state is called as a stable state. When the voltage goes below at the second pin of the 555 IC, the o/p becomes high. This high state is called quasi stable state. When the circuit activates then the transition from a stable state to quasi stable state. Then the discharge transistor is cut off and capacitor starts charging to VCC. Charging of the capacitor is done via the resistor R1 with a time constant R1C1. Hence, the voltage of the capacitor increases and finally exceeds 2/3 Vcc, it will change the internal control flip flop, thereby turning off the 555 timer IC. Thus the o/p goes back to its stable state from an unstable state.
The Time duration of the pulse is given by
T = 1.1RC
Where, R is in Ω and C in Farads.
Finally we can conclude that, in the monostable multivibrator using 555 timer, the o/p stays in a low state until it gets a trigger i/p. This type of operation is used in push to operate systems. When the input is triggered, then the o/p will go to high state & comes back to its original state.
## Circuit Diagram:
![image](https://github.com/user-attachments/assets/f09d2014-f234-4cf1-947f-79f882f99862)
## Calculation:
Given that T=0.5ms and assume c=1uF.


T=1.1RC



R =  0.5mS/(1.1×1uF) = 454.54 Ohm.
## Procedure
1.	Build the circuit as per the Circuit diagram.
2.	Calculate the resistor R and capacitor C using the formula ton=1.1RC.
3.	In simulation we used signal generator for triggering the circuit. 
4.	Analyze the capacitor charging and discharging Voltage per time.
5.	Analyze the ton period when input is triggered. 
## Output Waveform
![image](https://github.com/user-attachments/assets/141243cc-a94a-4485-b145-532742e47138)

First waveform is triggering pulse for Monostable Multivibrator, Second waveform is Voltage across the Capacitor and Third waveform is output Pulse of 0.5ms
## Inference
•	The output of the circuit remains LOW in its stable state until a trigger input is applied.

•	Upon receiving the trigger, the output switches to HIGH and stays in that state for a time period determined by the RC time constant.

•	With the capacitor value chosen as 1 µF, the required resistor value was calculated to be approximately 454.54 Ω to achieve a 0.5 ms pulse.

•	This experiment demonstrates the use of a 555 timer in monostable mode for generating precise time delays.

## Conculsion
The 555 timer IC in monostable mode successfully generated a 0.5 ms output pulse in response to a trigger input. The output pulse duration matched the calculated value using the formula T = 1.1 × R × C, demonstrating the timer’s effectiveness in generating precise time delays.


# Astable multivibrator and monostable multivibrator using 555 timer IC
## Aim
## Generate pulse of width 0.5ms using 555 timer IC.
## Theory
An astable multivibrator, often called a "free-running" multivibrator, is a circuit that generates a continuous rectangular waveform. Unlike its monostable counterpart, it doesn't need an external trigger to switch its output state. Instead, the duration of its high and low output states is determined by two resistors and a capacitor connected externally to the 555 timer chip.   


In a differentiator amplifier circuit, the positions of the capacitor and resistor are swapped compared to an integrator. Here, the capacitor 
 is connected to the input of the inverting amplifier, while the feedback element across the operational amplifier remains a resistor 
 This circuit performs the mathematical operation of differentiation. Essentially, the faster or larger the change in the input voltage signal, the greater the input current, and consequently, the more pronounced the output voltage change will be, often appearing as a "spike." Similar to the integrator, the RC network formed by the resistor and capacitor plays a crucial role, with the capacitor's reactance 
 being particularly significant in the differentiator's performance. 

 A clipper circuit is used to remove or "clip" specific portions of a waveform, such as negative voltage spikes. The output of this clipper circuit then serves as the trigger signal for a monostable multivibrator.   

A monostable multivibrator, also known as a one-shot, has only one stable state. Its purpose is to generate a single output pulse of a specific width (either high or low) when an external trigger pulse is applied. This trigger pulse initiates a timing cycle, causing the output to change its state. The output then remains in this second, unstable state for a duration determined by the RC time constant of its capacitor (C) and resistor (R), after which it automatically reverts to its original stable state. It will stay in this stable state until another input signal is received. Monostable multivibrators are capable of producing much longer rectangular waveforms. The rising edge of the output waveform coincides with the external trigger pulse, while the falling (trailing) edge is governed by the RC time constant of the feedback components. This RC time constant can be adjusted over time to produce a series of pulses, each with a fixed time delay relative to the original triggered pulse.
## Procedure
1.	Build the circuit as per the Circuit diagram.
2.	Calculate the resistor R and capacitor C for Astable multivibrator Differentiator, clipper and Monostable multivibrator.
3.	Analyze the capacitor charging and discharging Voltage per time.
4.	Analyze the ton period when input is triggered.

## Calculation
![WhatsApp Image 2025-05-25 at 10 27 49 PM](https://github.com/user-attachments/assets/5732fca0-5e8c-4797-a74b-34de441e5371)

![WhatsApp Image 2025-05-25 at 10 27 50 PM](https://github.com/user-attachments/assets/e16eea9b-03ac-435c-aa1e-872aebd2f6d0)


## Circuit Diagram:
![image](https://github.com/user-attachments/assets/b07bcbbe-72dd-4548-a828-e1ff5dc9cebd)


## Waveform
### Case 1:
![image](https://github.com/user-attachments/assets/bdcbd7d8-b042-44d8-a02f-16989a367a90)

First wave is output of Astable Multivibrator, Second waveform is Output of Differentiator Circuit output, 3rd wave is the output of Negative Clipper circuit and fourth waveform is output of Monostable Multivibrator pulse width is 0.5ms.

### Case 2:
![image](https://github.com/user-attachments/assets/bb0dabe9-f63f-4be1-9e6b-fbbc78f23174)

First wave is output of Astable Multivibrator, Second waveform is Output of Differentiator Circuit output, 3rd wave is the output of Negative Clipper circuit and fourth waveform is output of Monostable Multivibrator pulse width is 0.5ms.
 cap value .1u

 ### Case 3:

 in case 3 the ton<toff which is not possible in astable Multivibrator , thus we can use an inverter to invert the pulse generated.
 
![image](https://github.com/user-attachments/assets/62330045-4a0a-422d-b977-9699a629bb00)

![image](https://github.com/user-attachments/assets/5974cd20-b140-48e9-b307-9e661e8e4906)



First wave is output of inverted Astable Multivibrator, Second waveform is Output of Differentiator Circuit output, 3rd wave is the output of Negative Clipper circuit and fourth waveform is output of Monostable Multivibrator pulse width is 0.5ms.

## Inference
- Controlling ON and OFF Times Isn't Always Straightforward
We saw that changing resistor and capacitor values lets us control how long the signal stays ON and OFF. But it’s not always possible to get any values we want with the basic 555 timer setup.

- The 555 Timer Has Its Limits
In some cases (like when OFF time needs to be longer than ON), the normal 555 astable circuit can’t give us the result directly. That’s why in Case 3, we had to flip the signal using an inverter.

- Inverters Can Help Us Get the Waveform We Want
By adding a simple NOT gate (built using a transistor), we were able to reverse the timing — this gave us more flexibility in generating the waveform we needed.

- Very Short Pulses Need Precise Components
In Case 2, we worked with very fast pulses (just fractions of a millisecond). To do that, we needed low resistor and capacitor values — which also showed us the importance of accuracy and how component selection affects timing.

- We Can Detect Edges Using a Differentiator
A differentiator circuit helped us catch the exact moment the signal goes from LOW to HIGH. This is useful when we only want to react to changes, not the full pulse.

- Monostable 555 Gives Clean, Consistent Pulses
Finally, when we triggered a monostable 555 with those edges, we got clean, uniform pulses every time. This is super helpful when we need a reliable output regardless of input width.

| **Case** | **Configuration** | **What We Learned** |
|----------|-------------------|----------------------|
| **Case 1**<br>(ON = 0.2 ms, OFF = 0.3 ms) | Direct astable 555 output | Basic control of ON/OFF time using R1, R2, and C values works well within certain timing ranges. |
| **Case 2**<br>(ON = 0.1 ms, OFF = 0.05 ms) | High-speed pulse using small R and C | Fast switching is possible but requires precise low-value components. Useful for short pulse generation. |
| **Case 3**<br>(ON = 0.3 ms, OFF = 0.4 ms)<br>with inverter | Inverter used after 555 output | Shows how logical inversion helps overcome 555 timer’s limitations, allowing ON < OFF timing. |


# Simulation in Virtual Lab Astable Multivibrator
## Procedure:
1.	Connect the components as mentioned below: L1-L12, L14-L12, L16-L12, L4-L9, L8-L9, L10-L19, L3-L17, L11-L13, L7-L19, L6-L13, L2-L13, L5-L15, L18-L9.(For eg. click on 1 and then drag to 12 and so on.)
2.	Click on 'Check Connection' button to check the connections.
3.	If connected wrong, click on the wrong connection. Else click on 'Delete all connection' button to erase all the connections.
4.	Intially set R a=3.3 kΩ, R b=6.8kΩ, C=0.1µf, Vcc=5 V.
5.	Click on "Calculate" button.
6.	Now note the output voltage.
7.	Click on "Plot" button to plot Output Voltage, Capacitance Voltage
8.	Click on "Clear" button to clear the data.
9.	Repeat the experiment for another set of resistance value.
10.	Set the Resistance (Ra) value (1 kΩ - 10 kΩ).
11.	Set the Resistance (Rb) value (1 kΩ - 10 kΩ).
12.	Set the Capacitance (C) value (0.1 µf - 10 µf) .
13.	Set supply voltage (Vcc).

## Circuit Diagram
![image](https://github.com/user-attachments/assets/303eba91-66eb-4a6a-9dbc-12f03dbb176c)


## Otuput Waveform
Voltage Across the Capacitor: 
![image](https://github.com/user-attachments/assets/3894310a-e307-4e17-a570-e0371812d10f)


Output Waveform: -
![image](https://github.com/user-attachments/assets/df261aa6-19a1-41bf-82f9-d65b0f5742c9)
