### Thermodynamics Recap
#### Thrust and Propulsive Efficiency
>**Thrust** is equal to the rate of change of momentum:
>$$F=\dot{m}(C_{jN}-C_{a})+A_{j}(P_{j}-P_{a}), ~~~~~~\dot{m}_{f}<<\dot{m}$$
>Where fuel flow is $\dot{m}_{f}$ and the net calorific value of fuel is $Q_{net}$
>![[Pasted image 20260127110356.png|centre|400]]

The efficiency of energy conversion is equal to the useful mechanical energy supplied by the fuel:
$$\mathbf{\eta_{e}}=\frac{1}{2}\dot{m}\frac{(C_{j}^{2}-C_{a}^{2})}{Q_{net}\cdot \dot{m}_{f}}$$
The propulsive efficiency is equal to the useful work/useful work + unused KE in the jet: (assuming fully expanded jet from the propelling nozzle)
$$\mathbf{\eta_{p}}=\frac{F\cdot C_{a}}{F\cdot C_{a}+\frac{1}{2} \dot{m}(C_{j}-C_{a})^{2}}=\frac{2}{1+C_{j}/C_{a}}$$
The overall efficiency is the product of the efficiency of energy conversion and propulsive efficiency:
$$\huge{\boxed{\eta_{overall}=\eta_{e}\cdot\eta_{p}}}$$
So:
$$\eta_{overall}=\frac{F\cdot C_{a}}{\dot{m}_{f}\cdot Q_{net}}$$
And:
$$SFC=\frac{\dot{m}_{f}}{F}$$
Hence the overall efficiency (for a given fuel) is directly proportional to the flight speed/SFC:
$$\eta_{overall}=\frac{C_{a}}{SFC\cdot Q_{net}}$$
And thus SFC is a measure of overall efficiency.

The Fuel Air Ratio (FAR) is:
$$FAR=\frac{\text{fuel flow}}{\text{air flow}}=\frac{\dot{m}_{f}}{\dot{m}}$$
The Specific Thrust (ST) is equal to the Thrust divided by the unit Mass flow:
$$ST=\frac{F}{\dot{m}}=(C_{j}-C_{a})$$
This means that:
$$SFC=\frac{FAR}{ST}=\frac{\dot{m}_{f}}{F}$$
#### Basic Thermodynamic Relationships
The laws of thermodynamics are empirical. The first law of thermodynamics yields the steady flow energy equation, per unit mass flow rate:
$$Q=(h_{2}-h_{1})+ \frac{1}{2}(C_{2}^{2}-C_{1}^{2})+W$$
Where the stagnation (total) Enthalpy is:
$$h_{0}=h+\frac{C^{2}}{2}$$
and:
$$h=C_{p}T$$
so:
$$T_{0}=T+\frac{C^{2}}{2\cdot C_{p}}$$
since:
$$h_{0}=C_{p}T_{0}$$

The second law of thermodynamics yields:
$$ds=\left(\frac{dQ}{T}\right)_{rev}$$
This is the concept of entropy - a property of thermodynamic systems.

**Specific Heats**
The quantity of heat needed to raise the temperature of unit mass of a substance by 1K is the specific heat. It is a function of temperature only for normal conditions in a GTE. It is often considered constant to simplify preliminary analysis.

Typical Values for Air:
$$C_{pa}=1005~ J/kgK,~~~~\gamma_{a}=\frac{C_{p}}{C_{V}}=1/4,~~~~\frac{\gamma}{\gamma-1}=3.5,~~~~C_{p}-C_{V}=R$$
For Exhaust Gasses:
$$C_{pg}=1148~ J/kgK,~~~~\gamma_{g}=\frac{C_{p}}{C_{V}}=1.333,~~~~\frac{\gamma}{\gamma-1}=4$$
For both air and exhaust gasses the gas constant $R=287.1~J/kgK$ 

**Total Temperature**
$$T_{0}=T+ \frac{C^{2}}{2\cdot C_{P}}~~~~ or~~~~T_{0}=T\left[1+\frac{\gamma-1}{2}M^{2}\right]$$
**Total Pressure** (for isentropic)
$$P_{0}=P\left[1+\frac{\gamma-1}{2}M^{2}\right]^{\frac{\gamma}{\gamma-1}}$$
Note also (for isentropic):
$$\frac{P_{02}}{P_{01}}=\left[\frac{T_{02}}{T_{01}}\right]^{\frac{\gamma}{\gamma-1}}$$
### The Ideal Joule-Brayton Cycle
Assumptions:
- The working fluid is air and behaves as a perfect gas
- The mass-flow through the cycle is constant
- The kinetic energy change between inlet and outlet of components is negligible
- No component pressure losses
- Isentropic compressions and expansions
![[Pasted image 20260127112430.png|centre|400]]
![[Pasted image 20260127112451.png|centre|300]]


The efficiency of the cycle is the net work produced by the cycle divided by the heat energy input:
![[Pasted image 20260127112548.png|centre|400]]
Therefore cycle efficiency is:
$$\large{\boxed{\eta_{th}=1-\left(\frac{1}{PR}\right)^{\frac{\gamma-1}{\gamma}}}}$$
**The cycle efficiency is only a function of pressure ratio!**
![[Pasted image 20260127112725.png|centre|300]]
Remembering that:
$$T_{2}=T_{1}\left(\frac{P_{2}}{P_{1}}\right)^{\frac{\gamma-1}{\gamma}}$$
So if we want an expression for net work in terms of PR and maximum cycle temperature:
$$\text{Net Work}=W=W_{34}-W_{12}=C_{p}\times((T_{3}-T_{4})-(T_{2}-T_{1}))$$