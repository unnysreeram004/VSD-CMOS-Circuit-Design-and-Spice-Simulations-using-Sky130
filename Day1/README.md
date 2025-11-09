Start by cloning the following repo:
https://github.com/kunalg123/sky130CircuitDesignWorkshop.git

Goal: To plot the IDS Vs VDS for various values of VGS

Spice File
<img width="970" height="655" alt="image" src="https://github.com/user-attachments/assets/ded6232f-ca27-4d42-a409-77570ea6636a" />

Running the above and including "_plot -vdd#branch_" commands, we get the following:
<img width="927" height="689" alt="image" src="https://github.com/user-attachments/assets/b36011da-1cea-41f5-9469-6d48790e6a6a" />

An update was made to the incoming spice file to make the plots more readable:
<img width="940" height="680" alt="image" src="https://github.com/user-attachments/assets/60789505-23ca-4b5d-aef4-2b710109b01e" />


Left clicking on any point on the plot triggers the below statement in the shell:

<img width="280" height="43" alt="image" src="https://github.com/user-attachments/assets/09640af4-4971-4bcb-9dd7-99e5cc0cc81a" /> 


Appropriate axis labels and titles can also be provided w/ _plot xlabel, plot ylabel_ and _plot title_ commands. 
