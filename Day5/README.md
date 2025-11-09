Goal: To check the impact of the supply variation on the gain of the devices. 

Spice File:

<img width="1459" height="830" alt="image" src="https://github.com/user-attachments/assets/93bcb615-1f62-45c7-8d59-ab784e8ed131" />

\
Running the above file w/ NGSPICE:

<img width="1253" height="940" alt="image" src="https://github.com/user-attachments/assets/98effa77-7ff6-431b-8000-b718b59cf2c8" />

Gain at 1.8V = 7.89

<img width="329" height="98" alt="image" src="https://github.com/user-attachments/assets/f19801dd-974d-44db-aeaf-bac33b2cb5f4" />

 
Gain at 0.8V = 9.12

<img width="344" height="99" alt="image" src="https://github.com/user-attachments/assets/02468e76-cc5d-4ee5-983f-71146dc0b000" />

\
Goal: To assess the impact of device variation on the switching threshold. 
 
Spice File: 

<img width="1033" height="844" alt="image" src="https://github.com/user-attachments/assets/9ed96d5a-23ba-4456-8684-57f9f434ffad" />
PMOS is kept wider significantly compared to NMOS.

\
Results

<img width="761" height="684" alt="image" src="https://github.com/user-attachments/assets/fa835520-53f0-45fb-9413-3a2ce5e4a6fd" />


VM = 0.988V (0.5*VDD = 0.9V). There is only a variation of ~90mV for such a huge variation in the device width. Hence, CMOS can be  considered very robust.

