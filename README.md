# Experiment-1
Question : Given that POWER, P=100µ W; Perform DC Analysis, Transient Analysis and AC Analysis for the Given Circuit Designs and also check what happens when the width is increased or decreased of each mosfet;

# Design-1 :

   ![image](https://github.com/user-attachments/assets/9a8fab35-b076-453d-8c19-eeb2f14c3d76)


Using the Formula for Power, 

P=V*I

We will get the Values of Id as,

Id= 5.56 * 10^-5 A

we have to get the output current, Id for the given circuits by adjusting the values of L & W( Length and Width of the Channel of the MOSFET)

Length and Width of the Channel used to obtain the given Current is shown in the figure below;

![image](https://github.com/user-attachments/assets/ec9e6aa6-a01f-4d13-ace0-4f4f2aba9d79)

1) DC ANALYSIS:

   Procedure for Performing DC Analysis:
   we have to select the dc output print(DC op pnt) in the Edit Simulation Command and Run the Simulation

   ![Screenshot 2025-02-16 121422](https://github.com/user-attachments/assets/8dbd733e-f0a2-4165-8a8e-ebee3b28ace2)

   The Figure below shows the Values obtained from the DC Analysis : 

   ![image](https://github.com/user-attachments/assets/84e637eb-3a92-4350-abb8-5438f0bb0bc1)


2) Transient Analysis:

   Procedure for Performing Transient Analysis:
   we have to select the Transient Analysis in the Edit Simulation Command,  Give the stop time as 1ms and Run the Simulation.

   ![Screenshot 2025-02-16 122038](https://github.com/user-attachments/assets/e43f0303-c135-4a82-bc71-12e6ae6000b9)

   The Graphs below shows the Transient Response of the Given Design;

   ![image](https://github.com/user-attachments/assets/3e2f6c3e-e915-4dbc-aa56-36eaa5ec92e2)
   ![image](https://github.com/user-attachments/assets/c644c390-a82f-473c-9cb5-f333b28ba855)


   
4) AC Analysis:
   
   Procedure for Performing AC Analysis:
   we have to select the AC Analysis in the Edit Simulation Command,  Give the values as shown in the figure beowl and Run th Simulation.

   ![Screenshot 2025-02-16 122508](https://github.com/user-attachments/assets/f67f362a-312c-45c6-869a-bd410a0e133a)

   The Graph below shows the AC Analysis of the Given Design;

   ![image](https://github.com/user-attachments/assets/587d4c80-1cfa-4723-b3e9-88cfd30848e4)


# RESULT( Design-1):
 1) DC Analysis:
     1. The calculated drain current (Id) matches the expected value based on power and voltage, Id = 5.56*10^-5 A.
     2. By adjusting the MOSFET’s channel dimensions (L & W) where L=500nm and W= 1053nm, The current requirement was succesfully achecived.
     4. The circuit behaves as expected under DC conditions.

 2) Transient Analysis:
     1. The transient response graph shows how the circuit behaves over time.
     2. The response is smooth, with no unexpected delays or distortions.
     3. The circuit reacts well to changes, confirming its stability.

 3) AC Analysis:
     1. The AC response graph confirms that the circuit remains stable at different frequencies.
     2. The gain(10 dB) and phase shift(which is nearly 180deg) align with theoretical expectations.
     3. The circuit maintains its performance across the tested frequency range.

# INFERENCE( Design-1):
   1. The experiment confirms that by properly selecting the MOSFET dimensions, we can control the drain current effectively.
   2. Impact of Width Adjustments:
         1. M1 has a influence on Id, meaning its width affects the output current.
   3. The circuit performs well in all three analyses—DC, transient, and AC—demonstrating its reliability.
   4. Overall, the design works as intended, following theoretical predictions and proving its practical feasibility.



# Design-2

![image](https://github.com/user-attachments/assets/9fb14382-e1a6-4662-a5f5-48cc425f37aa)

Using the Formula for Power, 

P=V*I/n

We will get the Values of Id as,

Id= 5.56 * 10^-5 A

we have to get the output current, Id for the given circuits by adjusting the values of L & W of both the MOSFETS M1 & M2 ( Length and Width of the Channel of the MOSFET)
        
DC SWEEP Analysis: This analysis is done for obataing the value of Vin in Saturation range;

we have to select the DC SWEEP in the Edit Simulation Command,  Give the values as shown in the figure below and Run th Simulation.

![image](https://github.com/user-attachments/assets/b26e13fb-57be-4522-8e21-9b4730448512)

The Graph beow represents the VTC Curve and the value of the vin is selected as 0.7V as it is present in the saturation region of the VTC Curve

![image](https://github.com/user-attachments/assets/fdf95436-c71a-4046-bcca-ddba2ffd6523)


Then the input voltage parameters are given as;

![image](https://github.com/user-attachments/assets/159fb9f1-5839-4019-9967-1b1735c9b175)


Length and Width of the Channel of the two MOSFETS used to obtain the given Current is shown in the figure below;

![image](https://github.com/user-attachments/assets/dd6df468-7957-4602-bd00-801673f71ae5)
![image](https://github.com/user-attachments/assets/f2490db8-57c7-4949-9e67-ba6728b574c2)


Now we will be performing the DC, Transient and AC Anlaysis;

1) DC ANALYSIS:

   Procedure for Performing DC Analysis:
   we have to select the dc output print(DC op pnt) in the Edit Simulation Command and Run the Simulation

   ![Screenshot 2025-02-16 121422](https://github.com/user-attachments/assets/fe699e4e-be59-4a89-a524-8d88a54555c4)

   The Figure below shows the Values obtained from the DC Analysis :

   ![image](https://github.com/user-attachments/assets/e935cc0f-9d3d-473e-9b6d-9542b8d84477)


2) Transient Analysis:

   Procedure for Performing Transient Analysis:
   we have to select the Transient Analysis in the Edit Simulation Command,  Give the stop time as 1ms and Run the Simulation.

   ![Screenshot 2025-02-16 130048](https://github.com/user-attachments/assets/c3faea32-8fd7-4cdb-9d7b-0b454f8d626b)

   The Graphs below shows the Transient Response of the Given Design;

  ![image](https://github.com/user-attachments/assets/70c99a18-0c4b-42de-8288-d95d9795932c)
  ![image](https://github.com/user-attachments/assets/1975eba0-4e02-4469-bb43-43d098f3aa52)



3) AC Analysis:
   
   Procedure for Performing AC Analysis:
   we have to select the AC Analysis in the Edit Simulation Command,  Give the values as shown in the figure beowl and Run th Simulation.

   ![image](https://github.com/user-attachments/assets/80e2d1d3-f2f6-4ce8-b26e-0a803006303a)

   The Graph below shows the AC Analysis of the Given Design;

   ![image](https://github.com/user-attachments/assets/12fadf99-8548-466c-8d8d-cb1cd62253b2)



# RESULT(DESIGN-2)
1.DC Analysis:

   1. The calculated drain current (Id) aligns with the expected value based on power and voltage, where the value of Id = 5.56*10^-5 A .
   2. By fine-tuning the channel dimensions (L & W) of both MOSFETs ( M1 & M2), the desired current was achieved,
         1. M1 : L= 180nm  , W= 1105nm.
         2. M2 : L= 180nm  , W= 1105nm.      
   4. The circuit operates correctly within the selected DC parameters.

2.Transient Analysis:

   1. The transient response graph confirms that the circuit transitions smoothly over time.
   2. The circuit responds effectively to input variations, indicating stable operation.

3.AC Analysis:

   1. The AC response graph confirms that the circuit maintains stability over the tested frequency range.
   2. The gain(-0.4 dB) and phase shift (which is nearly 180deg) align with theoretical expectations.
   3. The circuit functions as expected under AC conditions.

# Inference (Design-2):
  1. The experiment validates that by appropriately selecting the MOSFET dimensions (L & W), the drain current can be precisely controlled.
  2. The voltage transfer characteristics (VTC) helped in selecting the correct operating voltage (0.7V) for saturation.
  3. Impact of Width Adjustments:
     
     1. M2 has a stronger influence on Id, meaning its width significantly affects the output current.
     2. M1 has a smaller influence, meaning changes in its width result in only minor variations in Id.
  5. The design meets the expected performance criteria and follows theoretical predictions, demonstrating its feasibility in practical applications.
