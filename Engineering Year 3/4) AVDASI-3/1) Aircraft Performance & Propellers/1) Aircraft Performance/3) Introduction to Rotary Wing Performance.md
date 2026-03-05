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
![[Pasted image 20260303184135.png|336]]![[Pasted image 20260303184220.png|309]]
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
$$FoM=\frac{T}{P}\sqrt{\frac{T}{2\rho A}}=\frac{T}{P}\frac{1}{\sqrt{2}}\sqrt{\frac{T}{\rho \pi R^{2}}}$$
$$FoM=PL\sqrt{\frac{DL}{2\rho}}$$
Where $T/P=PL$ otherwise known as Power Loading, and $T/A=DL$ otherwise known as Disk Loading. Then $$PL=1.565 FoM\frac{1}{\sqrt{DL}}$$
Which is dimensional, based upon $\rho$.
![[Pasted image 20260303185223.png|centre]]
Some specialised or stretched larger helicopters have disc loading greater than 58 kg/m2. A new design for a large transport type of helicopter would favour a lower disc loading to provide margins for in-service weight growth.
At the small end of the range of helicopter sizes typical disc loading values can be found well below 15-50kg/m2. Very light helicopters can have a smaller disc loading.
![[Pasted image 20260303185252.png|338]]
### Rotor Solidity
$\sigma$ is the rotor solidity, defined as:
$$\sigma=\frac{A_{b}}{A}=\frac{\text{Blade Area}}{\text{Disc Area}}=\frac{Nc}{\pi R}$$
Where $N$ is the number of blades, and $c$ is the blade chord.
![[Pasted image 20260303185619.png|295]]![[Pasted image 20260303185634.png|345]]
### Rotor Performance Coefficients
The thrust coefficient is:
$$C_{T}=\frac{T}{\rho A(\Omega R)^{2}}=\frac{T}{\rho A V^{2}_{t}}$$
where $V_{t}=\Omega R$ is the blade tip speed.

Blade loading is therefore:
$$\frac{C_{T}}{\sigma}=\frac{T}{\rho A\sigma (\Omega R)^{2}}=\frac{T}{\rho N c R V^{2}_{t}}$$
$$\overline{CL} =6 C_{T}/\sigma$$
The torque coefficient, and power coefficient can be calculated as:
$$C_{Q}=\frac{Q}{\rho A R(\Omega R)^{2}},~~~~~~~~C_{P}=\frac{P}{\rho A(\Omega R)^{3}}$$
Therefore $C_{P}=C_{Q}$ since $P=Q\Omega$.

The **Advance Ratio**:
$$\mu=\frac{V_{F}\cos\alpha}{\Omega R}$$
Where $V_{F}$ is the helicopter forward speed and $\alpha$ is the angle of attack of the rotor.
**The Inflow Ratio**:
$$\lambda=\frac{V_{V}+v}{\Omega R}$$
Where $V_{V}$ is the vertical speed of the helicopter. In hover $\lambda = \frac{v}{\Omega R}$.

### The Figure of Merit
We have previously seen:
$$FoM=\frac{Tv}{P}=\frac{C_T}{C_{P}}\lambda=\frac{1}{\sqrt{2}}\frac{C_{T}^\frac{3}{2}}{C_{P}}$$
For ideally twisted blades:
$$C_{P}=\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}+\frac{\sigma \delta}{8}$$
Therefore the FoM is:
$$FoM=\frac{\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}}{\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}+\frac{\sigma \delta}{8}}$$
#### The FoM for General Cases
$$C_{P}=k\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}+\frac{\sigma\delta}{8}$$
Where $k$ is the induced power correction factor (k=1.1 to 1.15).
$$FoM=\frac{\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}}{k\frac{C_{T}^\frac{3}{2}}{\sqrt{2}}+\frac{\sigma\delta}{8}}$$
#### Maximising the Figure of Merit
![[Pasted image 20260303191525.png|centre]]
### Endurance
The fuel flow for a power plant delivering a power $P$:
$$m_{f}=SFC\cdot P$$
The weight loss due to fuel consumption:
$$\frac{dW}{dt}=-\frac{dW_{f}}{dt}=-g \cdot SFC\cdot P=-g\cdot SFC \cdot \rho A(\Omega R)^{3}C_{p}$$
We also have:
$$\frac{dW}{dT}=\frac{dT}{dt}=\rho A(\Omega R)^{2}C_{T}$$
Therefore, the endurance can be given as:
$$E=\frac{1}{g\cdot SFC}\frac{1}{\Omega R}\int_{end}^{initial} \frac{dC_{T}}{C_{P}}$$
## Helicopter Performance in Forward Flight 
### Induced Velocity in Translational Flight
![[Pasted image 20260303193645.png|centre]]
### Induced Velocity in Translational Flight
![[Pasted image 20260303193954.png|centre]]
### Power of the Main Rotor in Forward Flight
![[Pasted image 20260303194139.png|centre|532]]

### Breakdown of Helicopter Power
![[Pasted image 20260303194200.png|centre]]
### Effects of Weight and Altitude on Power
![[Pasted image 20260303194220.png|centre]]
### Maximum Range and Maximum Endurance
![[Pasted image 20260303194236.png|centre]]
### Payload Range Diagram
![[Pasted image 20260303194250.png|centre]]
