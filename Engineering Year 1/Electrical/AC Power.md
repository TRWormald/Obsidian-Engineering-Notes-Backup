### Explanation
Electrical power is the rate at which energy is being consumed in a circuit. It can be time-varying either as a DC quantity or as an AC quantity.
In an AC circuit the instantaneous values of the Voltage $V(t)$, current $I(t)$ and thus power $P(t)$ are constantly changing.
![[Pasted image 20240304110349.png]]
Depending on the phase difference between the voltage and the current the power wave's phase and offset will vary.
Note that the frequency of the power wave is always twice that of the current or voltage.
Also note that when the voltage leads or trails the current by 90 degrees the average power disappears and as a result there is no net power, in fact the energy is just being stored in the reactive components.
For the voltage leading the current by more than 90 degrees the load is supplying power back to the source (hence why the average power is negative)
\
This happens because AC circuits contain reactance which is created by either an capacitor, inductor or both.
Power dissipated by a resistive load is lost, whilst power dissipated by a reactive load is stored (either as an electric or magnetic field)
### Equations
#### Instantaneous Power
The amount of power in a circuit at any instant of time is the instantaneous power. It is given by:
$$p(t)=v(t)\cdot i(t)$$
In a steady state:
$$v(t)=V_Mcos(\omega t+\theta_v)$$
$$i(t)=I_Mcos(\omega t+\theta_i)$$
So:
$$p(t)=V_MI_Mcos(\omega t+\theta_v)cos(\omega t+\theta_i)$$
And as:
$$cos\phi_1cos\phi_2=\frac{1}{2}[cos(\phi_1-\phi_2)+cos(\phi_1+\phi_2)]$$
$$p(t)=\frac{V_MI_M}{2}[cos(\theta_v-\theta_i)+cos(2\omega t +\theta_v+\theta_i)]$$
With the first trigonometric component being constant as the phase of the voltage and current are constant, and the second having twice the frequency of either the voltage or the current.
#### Average Power
The average power $P_{avg}$ is the average of the instantaneous power in a circuit over one full period.
We can get this by using our knowledge of finding the mean value of a function:
$$P_{avg}=\frac{1}{T}\int_{t_0}^{t_0+T}p(t)\cdot dt,~~~~~T=\frac{2\pi}{\omega}$$
So if:
$$v(t)=V_Mcos(\omega t+\theta_v)$$$$i(t)=I_Mcos(\omega t+\theta_i)$$$$p(t)=\frac{V_MI_M}{2}[cos(\theta_v-\theta_i)+cos(2\omega t +\theta_v+\theta_i)]$$
Then:
$$P_{avg}=\frac{V_MI_M}{2}cos(\theta_v-\theta_i)$$

### RMS Power
We can also define the power in a circuit using the Root Mean Square, it is defined as:
$$V_{rms}=\sqrt{\frac{1}{T}\int_{t_0}^{t_0+T}[V(t)]^2\cdot dt}$$$$I_{rms}=\sqrt{\frac{1}{T}\int_{t_0}^{t_0+T}[I(t)]^2\cdot dt}$$
For a purely sinusoidal signal:
$$\boxed{V_{rms}=\frac{V_{peak}}{\sqrt{2}},~~~I_{rms}=\frac{I_{peak}}{\sqrt{2}}}$$
**These equations are boxed because this is the only way that we will be asked to calculate the RMS values, the derivations above will not be used.**
It is the closest approximation to DC equivalent for AC signals, and it is useful for simplifying calculations. For example the power for a resistor in an AC circuit:
$$P_{rms}=V_{rms}I_{rms}=\frac{V_{peak}}{\sqrt{2}}\cdot \frac{I_{peak}}{\sqrt{2}}=\frac{I_{peak}V_{peak}}{2}$$
### RMS Power Triangle
If we consider power supplied from an AC voltage source $V_S$ in a series complex impedance, $Z=R+j(X_L-X_C)$, we note that power will also be a complex quantity.
The total complex power is apparent power, $S$ and can be calculated as:
$$S_{rms}=I_{rms}\cdot V_{rms},~~~~~V_{rms}=I_{rms}\cdot Z$$
$$S_{rms}=I^2_{rms}\cdot Z=I^2_{rms}(R+j(X_L-X_C))$$
The real component is the **Real Power** [W], dissipated in the resistor:
$$P_{rms}=I^2_{rms}\cdot R$$
The imaginary component is the **Reactive Power** [VAr], stored in the reactive elements:
$$Q_{rms}=I_{rms}^2(X_L-X_C)$$
**Note that the Reactive Power is the power which is transferred between the source and the load per second. It is not useful but your AC system must be rated to be able to carry that power.**
\
The power factor is the cosine angle formed between the apparent power and the real power, it is the ratio of the real power absorbed by an impedance to the total apparent power.
$$Power~Factor = cos(\theta)=\frac{P_{rms}}{S_{rms}}$$
\
**If the power factor is 1 the load is purely resistive**
**If the power factor is 0 the load is purely reactive**

