#### Current Mirror 

### Aim:
Design the Current mirror circuit for Av(Gain)>10,Vdd=1.8V,P<=1mw Design the current mirror ratio 1:1 and 1:2 perform transient and Ac Analysis.

### Components and Libraries Required:
CMOSP(x2),CMOSN(x1),Current source(Reference),Voltage sources , tsmc018.lib

### Theory :

![image](https://github.com/user-attachments/assets/5e5c5fe3-3c5c-493b-b2fd-1efec5881fa0)

The current mirror is an analog circuit that senses the reference current and generates the copy or number of copies of the reference current, with the same characteristics. The replicated current is as stable as the reference current source. The replicated current could be the same as the reference current (Id = Iref),


The relation between the Id and Iref can be given by the following expression.

Id = ( (W/L)1 / (W/L)ref ) * Iref

By changing the W/L ratio of the two transistors, the current which is fraction or multiple of the reference current can be generated. The only thing which needs to be ensured is that, the MOSFET should operate in the saturation region.

#### Simulation 
#### 1) Current mirror circuit with 1:1 ratio
Design a current mirror circuit which has a gain of AV = -10V/V, power supply of Vdd = 1.8V, and power of P <= 1mW. Find reference current (Iref), output current (Id), and total current (Itotal). Perform DC and AC analysis for mirror ratio 1:1, 1:2. Vary length from 180nm -> 500nm -> 1µm and do the analysis.
1) with length as 180n
![image](https://github.com/user-attachments/assets/ec823f17-66d5-4b5b-8f5f-650cb814ca37)
##### Circuit Diagram
Itotal = ( Power / Vdd )
= ( 1m / 1.8 )
= 0.55mA

Iref = Id = ( Itotal / 2 )
= 0.55m / 2
= 0.277mA
#### DC Analysis
![image](https://github.com/user-attachments/assets/66dbaded-8ed4-4f99-b83e-5dc9da33ad1b)
#####  output of DC Analysis


#### Transient Analysis
![image](https://github.com/user-attachments/assets/2ee3938c-dbe8-4c71-81b1-ef285ec5567e)
#####  Output of Transient Analysis

#### AC Analysis
![image](https://github.com/user-attachments/assets/a08667d9-8f63-4a35-ace9-04cbaff65b08)
#####  Output of AC Analysis
AV=29.8364dB Frequency=10MHz
Bandwidth = (29.83dB-3dB) = 26.83dB , Frequency=278.81MHz
##### 2) with length as 500nm
#### DC Analysis
![image](https://github.com/user-attachments/assets/f64a80a7-4786-4999-99bf-0b1218b2585f)
#####  Output of DC Analysis
#### Transient Analysis
![image](https://github.com/user-attachments/assets/f4d94e8a-9685-47f0-9b94-4c83b41d6f14)
##### Output of Transient Analysis
#### AC Analysis
![image](https://github.com/user-attachments/assets/a8f4d2d8-6fa7-48b2-9d69-dd4a77baff54)
#####  Output of AC Analysis
Av=38.8366dB Frequency=11.818MHz
Bandwidth = (38.83-3dB)=35.83 , Frequency= 54.52MHz

##### 3) with length as 1u
#### DC Analysis
![image](https://github.com/user-attachments/assets/8d6ce3e9-8462-4a80-96f4-8f2121979018)
#####  Output of DC Analysis
#### Transient Analysis
![image](https://github.com/user-attachments/assets/65ac6a33-7123-40e3-aa45-97929cde7944)
#####  Output of Transient Analysis
#### AC Analysis
![image](https://github.com/user-attachments/assets/3e3006d5-1031-4fab-9a17-e5f24ec736a3)
#####  Output of AC Analysis
Av=38.526dB Frequency=10MHz
Bandwidth=(38.52-3dB) = 35.52dB , Frequency=41.09MHz


#### Current Mirror CIrcuit with 1:2 Ratio

##### 1) With length as 180nnm
#### DC Analysis
![image](https://github.com/user-attachments/assets/1119a53c-488f-4885-97a6-f60ba8f896a6)
##### Output of DC Analysis
#### Transient Analysis
![image](https://github.com/user-attachments/assets/a99562ab-7e0a-4fe0-8521-ed1228d7f348)
##### Output of Tansient Ananlysis
#### AC Ananlysis
![image](https://github.com/user-attachments/assets/1748a3e7-09f7-422f-8c15-1166af4698dc)
#####  Output of AC Analysis
Av=29.781147dB Frequency=10MHz
Bandwidth=(29.78dB-3dB) = 26.78 , Frrequency=268.26MHz

##### 2) With length as 500nm
#### DC Analysis
![image](https://github.com/user-attachments/assets/b4314a22-119a-4881-8425-eafaaacff93b)
#####  Output of DC Analysis
#### Transient Analysis
![image](https://github.com/user-attachments/assets/3423b70f-38a4-4286-aabf-d5ba49ab598e)
#####  Output of Transient analysis
#### AC Analysis
![image](https://github.com/user-attachments/assets/78c753b5-1885-44ea-9d7d-9191075940b7)
##### Output of AC Analysis
Av=38.83132dB Frequency=11.97085MHz
Bandwidth=(38.83-3dB)=35.83 , Frequency=53.83MHz

##### 3) with length as 1u
#### DC Analysis
![image](https://github.com/user-attachments/assets/ae3d30b9-4fd5-46fd-93e3-946675362218)
#####  Output of DCD Analysis
#### Transient Analysis
![image](https://github.com/user-attachments/assets/499f5454-61a9-4984-a691-9207b74aecb4)
##### Output of Transient Analysis
#### Ac Analysis
![426340776-9edb6d93-75f4-46eb-89b5-560849231f5a](https://github.com/user-attachments/assets/15c69ef2-d9ea-4227-b15c-bdad0e20fb43)

##### Fig 22: Output of AC Analysis
AV=40.56 , Frequency=11.51
(40.56-3dB) = 37.56 , 33.89MHz
 
