### What Will We Cover?
Now we've looked at the basics of aerofoils in supersonic flows we are going to:
- Explain transonic 2D aerofoil behaviour
- Introduce the concept of the Critical Mach Number and how to calculate it.
### Why do we fly at transonic speeds?
When maximising for range, we know from the [[Breguet Range - Jet|Breguet Range Equation]] that it is proportional to speed times lift over drag. The optimum point for this maximisation comes out at just below Mach 1 (i.e. transonic speeds).
### 2D Transonic Aerofoils - Critical Mach Number
Transonic behaviour begins when sonic flow first appears on the aerofoil surface.
Identification of the sonic point is important in aerofoil design.
At low free stream Mach number the flow over an aerofoil is entirely subsonic, but as the free stream Mach number increases it will reach a critical value at which the local Mach number will become one at some point on the aerofoil, with the rest of the flow subsonic.
The flow is entirely isentropic (i.e. $p_0$ is constant) up to the sonic point.
(The above leads to the interesting point that on our compressible flow tables for subsonic flow, the $p_{0}/p$ ratio increases as we increase $M$ however once $M=1$ it reaches a maximum. This means that the static pressure $p$ is at a minimum.)
#### Calculating the Critical Mach Number
If we take the standard definition for the pressure coefficient:
$$C_{p}=\frac{2}{\gamma M_{\infty}^{2}}\left(\frac{p}{p_{\infty}}-1\right)$$
And set local $M=1$ to get the critical pressure coefficient:
$$\begin{align*}
C_{p}^{*}&= \frac{2}{\gamma M_{\infty}^{2}}\left(\frac{p}{p_{\infty}}\frac{p_{M=1}}{p_{0}}-1\right)\\
&= \frac{2}{\gamma M_{\infty}^{2}}\left(\frac{p}{p_{\infty}}\frac{1}{1.895}-1\right)
\end{align*}$$
This is the most useful for calculations of critical Mach numbers using the compressible flow tables.

We also need to know for a particular aerofoil geometry how the critical or min pressure coefficient varies with Mach number in order to have sufficient information to find the critical Mach number since $M_{\infty}=M_{cr}$ when the minimum pressure coefficient on the aerofoil is $C_{p_{min}}=C_{p}^{*}$.
We could use an experimental or numerical method to find $C_{p_{min}}$ but we can also find it approximately by using the minimum pressure coefficient from an incompressible section ($C_{p_{min_{0}}}$) for an aerofoil and using a compressibility correction to get $C_{p_{min}}$. This can be achieved using the Prandtl-Glauert correction.
If you then plot $C_{p}^{*}$ and $C_{p_{min}}$ you can find the intersection to see where the conditions for critical Mach number are exactly met by the particular aerofoil.
![[Pasted image 20250405191111.png|centre]]
The highest local velocities correspond to minimum $C_p$ (suction peak), this:
- Depends on AoA
- Generally scales directly with t/c
- Does not necessarily occur at maximum thickness
**FINDING THE CRITICAL MACH NUMBER**
![[Pasted image 20250405191415.png|centre]]
**TEST CASE**
We can use XFoil to obtain the $C_{p_{min_{0}}}$ for a given aerofoil at a given (small) AoA:
![[Pasted image 20250406101234.png|centre]]
Which we can then use in the first equation above, we need to initially make a first guess of the Critical Mach Number - lets say 0.7:
$$C_{p}^{*}=\frac{2}{1.403\times0.7^{2}}\left(\frac{1}{1.895}\times 1.388-1\right)=-0.7783$$
$$C_{p_{min}}=\frac{-0.88}{\sqrt{1-0.7^{2}}}=-1.2325$$
As these values are different our guess for the Critical Mach Number is incorrect.
We can't just make random guesses to find the correct value, so we need to create an iterative method that converges to the answer.
**CREATING THE ITERATIVE METHOD**
We can assume that the CMN lies between 0.6 and 0.8, so we can use the method of bisection to find it.
We can set up a table to record the iterative process:
![[Pasted image 20250406101748.png|centre]]
We then repeat the process until converged:
![[Pasted image 20250406101820.png|centre]]
#### Why is the CMN so important?
Above the Critical Mach Number we see "drag divergence" - i.e. a rapid increase in drag just above $M_{cr}$. 
We also see "shock stall" where $M_{cr}$ decreases with $\alpha$, and above $M_{cr}$ shocks form and you get separation induced stall at the shock attachment point.
The Aerodynamic centre also moves aft (towards the half chord point) which affects stability.
![[Pasted image 20250406102102.png|centre]]
### Transonic 2D Aerodynamic Characteristics
![[Pasted image 20250407114730.png|centre]]
When we observe the Transonic vs Linearised lift behaviour, we see that there is a drag peak near M=1 and the centre of pressure and the aerodynamic centre shift rearwards.
**In Subsonic Flow**:
![[Pasted image 20250407114914.png|centre]]
l![[Pasted image 20250407114945.png]]
**But when we reach the CMR:**
![[Pasted image 20250407115025.png|centre]]
**And then as we pass through the transonic regime:**
![[Pasted image 20250407115113.png|centre]]
**Finally when the flow itself is supersonic:**
![[Pasted image 20250407115142.png|centre]]
