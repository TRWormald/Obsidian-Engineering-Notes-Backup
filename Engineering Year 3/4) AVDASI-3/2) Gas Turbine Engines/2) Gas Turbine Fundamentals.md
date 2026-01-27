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
$$Q=(h_{2}-h_{1})+ \frac{1}{2}(C_{2}^{2}$$