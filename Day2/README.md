Goal: To understand the relationship b/w IDS and VGS at a constant VDS
 
Spice File: 

<img width="852" height="589" alt="image" src="https://github.com/user-attachments/assets/b912cdb9-4971-45b4-b364-bb379142cdc1" />  

\
Plotting IDS Vs VDS
<img width="892" height="675" alt="image" src="https://github.com/user-attachments/assets/393914df-c88a-43dc-a681-755dd0093457" />

To get the max value, enter the following commands in the shell:

ngspice 158 -> print maximum (-vdd#branch)
maximum (-vdd#branch) = 1.978350e-04

We note from the above plot that with an increase in VGS, the relationship b/w IDS and VGS becomes linear. To show the linear behavior, we plot IDS Vs VGS.

Spice File:

<img width="859" height="656" alt="image" src="https://github.com/user-attachments/assets/4f374bfc-6380-42a3-ad18-a55ced0bdfec" />

\
Now, we are plotting IDS Vs VGS (and not VDS like the one before). VDS is kept constant at 1.8V. Dimensions of the devices are the same. 
<img width="728" height="608" alt="image" src="https://github.com/user-attachments/assets/c3f715cb-b571-4907-998c-b4c27aa6344a" />

The linear behavior is primarily due to the short channel effect. 



