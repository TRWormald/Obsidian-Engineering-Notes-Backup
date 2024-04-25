Are batteries a constant voltage source? **NO**
As they discharge they lose voltage:
![[Pasted image 20240424110937.png|center|400]]
The above graph shows the open circuit voltage for a lithium-ion cell - this is typically called the OCV. 
As we can see the OCV decreases as the State of Charge (SOC) decreases.
\
For the following **Ideal** cell, where the resistor has a resistance of 10$\Omega$ :
![[Pasted image 20240425095603.png|center|300]]
When the cell is at 100% SOC the cell has voltage 4.2V
When the cell is at 0% SOC the cell has voltage 2.7V
\
Therefore, using Ohms Law:
Current at 100% SOC = $\frac{4.2}{10}$= 4.2A
Current at 0% SOC = $\frac{2.7}{10}$= 0.27A
### Nominal Battery Voltage
This is an arbitrary approximate voltage, for a Lithium Ion cell the nominal voltage is usually somewhere between 3.6 and 3.8 Volts.
The Nominal Voltage will be defined on the cell datasheet.
![[Pasted image 20240425095933.png|center|400]]
### Overpotential
Due to the fact that batteries have internal resistance, there is a difference between their open circuit voltage and their terminal voltage.
![[Pasted image 20240425100139.png|center]]
In discharge this results in a lower voltage as some energy is lost to the resistor (as it effectively operates as a potential divider) whilst when charging it results in a greater time to charge as energy is lost to resistance.
In both cases the lost energy goes to heat.