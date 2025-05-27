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


