Goal: Plot VTC (Vout Vs Vin) of an Inverter

Spice File:

<img width="766" height="672" alt="image" src="https://github.com/user-attachments/assets/50d46bae-ddac-452a-a08d-5a59ebc0a2e1" />

\
Running the above with "_plot out_" generates a VTC as shown below:
<img width="852" height="671" alt="image" src="https://github.com/user-attachments/assets/ebec9008-840d-4e9d-9a43-71b911c6fa63" />

Goal: To determine the switching-threshold from the VTC

By adding "plot out in" to the above simulation, we get the following:
<img width="861" height="630" alt="image" src="https://github.com/user-attachments/assets/2b7499ff-cb9d-4485-b476-6abdfb19cd45" />

The point of intersection is the switching threshold and can be found using:

_ngspice 174 -> let diff = out-in_

_ngspice 176 -> meas vm dc find in when diff=0_

_dc                  =  8.769191e-01_

Goal: How to perform transient analysis on an inverter?

Setup

<img width="738" height="600" alt="image" src="https://github.com/user-attachments/assets/5380d6b1-6ffc-486e-af41-02e2267fe8c9" />

\
The Vin risese to 1.8V in 100ps and stays for 2ns. It then comes down to 0V in 100ps. Repeats every 4ns. This is shown below:
<img width="605" height="542" alt="image" src="https://github.com/user-attachments/assets/62bbe171-2125-4008-86fe-688cec0deab2" />

Combining Out and In:
<img width="1002" height="720" alt="image" src="https://github.com/user-attachments/assets/54ff93c3-48e8-4fd5-a148-5cbd95d19f9f" />

Delay is measured for both rise and fall arcs and is defined at 50% point:

Rise

<img width="283" height="55" alt="image" src="https://github.com/user-attachments/assets/79aecccc-0ffa-43c0-b2b8-9feb10bde1a3" />

\
Fall

<img width="292" height="60" alt="image" src="https://github.com/user-attachments/assets/e2dca83a-c819-4b7f-828e-22881117ca1f" />

\
The rise-times, fall-times and propagation delays can all be calculated using the .meas commands in SPICE. 


