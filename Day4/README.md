Goal: To calculate the noise-margin of an inverter

Spice File: 

<img width="744" height="675" alt="image" src="https://github.com/user-attachments/assets/e10272a6-a4ec-44fb-b350-5d54ba3cca14" />

The derivate function is used to compute the Vin at which the slope becomes -1. 


VTC:

<img width="773" height="661" alt="image" src="https://github.com/user-attachments/assets/6f655e3b-f4ba-4dd7-9f0d-51713d568543" />

\
Plotting the slope of the above curve and adding a constant reference signal:
<img width="1081" height="746" alt="image" src="https://github.com/user-attachments/assets/3815837d-176a-4de4-833f-4399ed891705" />

<img width="249" height="62" alt="image" src="https://github.com/user-attachments/assets/66116224-3cfb-4530-adde-649a1ef3a8c5" />

VIL = 0.74V
VIH = 1V

By using the print out statement, the corresponding Vout values can be derived.  VOH= 1.75V, VOL = 0.08V

NH = 0.75V
NL = 0.66V

There are some inaccuracies to be expected due to rounding off significant digits. 
