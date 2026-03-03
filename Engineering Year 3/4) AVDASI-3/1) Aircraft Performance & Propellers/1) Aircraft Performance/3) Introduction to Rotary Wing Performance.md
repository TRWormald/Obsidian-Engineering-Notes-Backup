## Performance Breakdown
### Helicopter Mass Breakdown
![[Pasted image 20260303182449.png|491]]
$$\text{Mass}_{Final}=\text{Mass}_{Inital}-\text{Trip Fuel}$$
![[Pasted image 20260303182543.png]]
### Power Breakdown
In general, the total power required for a helicopter is:
$$P_{tot}=P_{i}+P_{o}+P_{p}+P_{TR}+P_{t}+P_{aux}$$
![[Pasted image 20260303182649.png]]
## Actuator Disc Theory in Axial Flight
We have previously covered actuator disc theory, so let's cover some of the basics again quickly. A stream tube is formed which contains all of the air which will pass through the rotor disc. We then apply Bernoulli across the rotor disk to calculate the velocities before and after. 
![[Pasted image 20260303183039.png|236]]
Where thrust is given by:
$$T=2\rho A(V+v)v$$
And power by:
$$P=T(V+v)$$
### Momentum Theory in Hover
For a lifting rotor in hover, when the onset velocity $V=0$. The induced velocity in hover can be calculated as:
$$v_{h}=\sqrt{\frac{T}{2\rho A}}$$
With the induced power in hover:
$$P_{h}=Tv_{h}$$
Hence:
$$P_{h}=\frac{T^\frac{3}{2}}{\sqrt{2\rho A}}$$
The main rotor thrust can be given as:
$$T=AUW(1+DLF)$$
Where the DLF is a download factor due to airframe drag.
### Operation in Ground Effects
![[Pasted image 20260303184135.png|399]]
![[Pasted image 20260303184220.png|350]]
Or in terms of power for a constant thrust:
$$\frac{P_{IGE}}{P_{OGE}}=k_{g}(z,D)\le 1$$
### Rotor Efficiency
The efficiency is just the Output Power divided by the Input Power:
$$\eta=\frac{\text{Output Power}}{\text{Input Power}}$$
For a rotor:
![[Pasted image 20260303184745.png|centre|622]]
### Rotor Efficiency in the Hover
The figure of merit is defined as:
$$\eta_{r}=FoM=\frac{P_{i}}{P}=\frac{Tv}{P}$$
Where $P_{i}$ is the induced power and $P$ is the rotor shaft power.
We can therefore rearrange the above equation to give:
$$FoM=\frac{T}{P}\sqrt{\frac{T}{2\rho A}}=\frac{T}{P}\frac{1}{}$$