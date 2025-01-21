### What Happens to Temperature Along a Stream-tube
A streamtube is defined by streamlines - with no flow normal to the streamlines the mass flow at 1 must equal the mass flow at 2:
$$\dot{m}=\rho_{1}A_{1}V_{1}=\rho_{2}A_{2}V_{2}$$
Then, with the following defined:
$$\text{Rate of KE entering}~~~~~~~~\frac{1}{2}\dot{m}v^{2}$$
$$\text{Rate of work done by pressure forces}~~~FV=pAV$$
$$\text{Rate internal energy entering}~~~~\dot{m}C_{v}T$$
Therefore is we consider energy conservation between 1 and 2:
$$\begin{align*}
const.&= p_{1}A_{1}V_{1}+ \frac{1}{2}\dot{m}V_{1}^{2}+\dot{m}C_{v}T_{1}\\
&= p_{2}A_{2}V_{2}+ \frac{1}{2}\dot{m}V_{2}^{2}+\dot{m}C_{v}T_{2}
\end{align*}$$
We can then rewrite $AV$ as $\dot{m}/\rho$ to get:
$$\begin{align*}
const.&= \frac{p_{1}}{\rho_{1}}\dot{m}+ \frac{1}{2}\dot{m}V_{1}^{2}+\dot{m}C_{v}T_{1}\\
&= \frac{p_{2}}{\rho_{1}}\dot{m}+ \frac{1}{2}\dot{m}V_{2}^{2}+\dot{m}C_{v}T_{2}
\end{align*}$$
And finally we can cancel the mass flow rate:
$$\boxed{\begin{align*}
const.&= \frac{p_{1}}{\rho_{1}}+ \frac{1}{2}V_{1}^{2}+C_{v}T_{1}\\
&= \frac{p_{2}}{\rho_{1}}+ \frac{1}{2}V_{2}^{2}+C_{v}T_{2}
\end{align*}}$$
Which we can rewrite in terms of enthalpy:
$$\boxed{h_{1}+ \frac{1}{2}V_{1}^{2}=h_{2}+ \frac{1}{2}V_{2}^{2}}$$
From which we can see enthalpy is conserved.
Hence we get "compressible Bernoulli":
$$\boxed{h_{0}=h+ \frac{1}{2}V^{2}=const.}$$
Which we can also rewrite for a calorically perfect gas:
$$\boxed{C_{p}T+ \frac{1}{2}V^{2}=const.=h_{0}=C_{p}T_{0}}$$
Finally we can rewrite the above equation using Mach number and obtain an equation for the stagnation Temperature $T_{0}$:
$$\boxed{T_{0}=T\left(1+\frac{(\gamma-1)M^{2}}{2}\right)}$$
### A Return to Basic Thermodynamics
For a calorically perfect gas:
$$h=c_{p}T$$
Hence:
$$\boxed{c_{p}T+ \frac{V^{2}}{2}=c_{p}T_{0}}$$
Where $T_{0}$ is the total or stagnation or reservoir temperature, more specifically it is the temperature of a fluid element brought to rest adiabatically.
*No assumption about entropy made in derivation.*
Note that:
- In an isentropic process $T_0$, $p_0$ and $\rho_{0}$ are constant
	- A sound wave
- In a  non-isentropic (but adiabatic) process only $T_0$ is constant
	- A shock wave
#### The Link Between Total Pressure and Entropy
Consider an adiabatic process from condition 1 to 2.
First we will consider the path from condition 1 to condition 01 - the conditions at a stagnation point. This is an isentropic deceleration.
Similarly if we go from 02 to 2 there is an isentropic acceleration.
Going from 1 to 2 (assuming the flow is adiabatic) the entropy change between 1 and 2 equals the entropy change in stagnation values:
$$s_{2}-s_{1}=c_{p}\ln\left(\frac{T_{2}}{T_{1}}\right)-R\ln\left(\frac{p_{2}}{p_{1}}\right)=c_{p}\ln\left(\frac{T_{02}}{T_{01}}\right)-R\ln\left(\frac{p_{02}}{p_{01}}\right)$$
However for adiabatic flow:
$$T_{01}=T_{02} \rightarrow \ln\left(\frac{T_{02}}{T_{01}}\right)=0$$
Therefore the change in entropy is only dependant on the change of total pressure:
$$-\frac{s_{2}-s_{1}}{R}=\ln\left(\frac{p_{02}}{P_{01}}\right)$$
Or:
$$\boxed{\frac{p_{02}}{p_{01}}=e^{-(\frac{s_{2}-s_{1}}{R})}}$$
Hence for non-isentropic flow total pressure is "lost" - $\frac{p_{02}}{p_{01}}<1 \rightarrow p_{02}<p_{01}$
However for isentropic flow total pressure is "conserved" - $\frac{p_{02}}{p_{01}}=1 \rightarrow p_{02}=p_{01}$
### The Speed of Sound
