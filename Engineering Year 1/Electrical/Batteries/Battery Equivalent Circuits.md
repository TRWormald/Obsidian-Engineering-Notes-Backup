The equivalent circuit for a battery is as follows:
![[Pasted image 20240425102425.png|center|400]]
It consists of a voltage source, and a parallel resistor.
$V_{OCV}$ is the open circuit voltage of the battery
$R_{0}$ is the internal resistance of the battery
\
Both of these values vary with the SOC and the Temperature, for example the following table is for $R_{0}$:
![[Pasted image 20240425102647.png|center|400]]
To find the $V_{OCV}$ we just need to look at our graph:
![[Pasted image 20240425102742.png|center|400]]
\
At each time step in the model, the known state of charge (and temperature) is used to approximate values for $R_{0}$ and $V_{OCV}$.
