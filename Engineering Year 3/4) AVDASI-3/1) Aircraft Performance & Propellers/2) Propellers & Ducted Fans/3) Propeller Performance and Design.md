### Propeller Pitch
>The **Geometric Pitch (P)** of a propeller is the theoretical axial displacement of the propeller prescribed by the geometric chord in one revolution.

>The **Effective Pitch (E)** is the actual axial displacement of the propeller (due to inflow)

The difference between these two lengths is called the **Propeller Slip**.
If the propeller blade has a radial twist such that all stations have the same Geometric Pitch the propeller is described as a **Constant Pitch Propeller**, as shown below:
![[Pasted image 20260216110932.png|centre|600]]

In this case $\beta$ is the angle to the horizontal (pitch angle) and $\phi$ is the inflow angle. We can see that $P$ is described by $\beta$ and $E$ is described by $\phi$.

By combining *Momentum Theory* and *Blade Element Analysis* we can determine some basic design parameters:

For a Constant Pitch propeller:
$$\tan{\beta}=\frac{P}{2\pi r}$$
Since all blade radial locations must have the same value of $E$, then:
$$\tan{\phi}=\frac{E}{2\pi r}$$
But since this is not a static condition, it is more convenient to replace $E$ with $V$ and modify the rotational displacement accordingly, then:
$$\tan\phi=\frac{V}{2\pi rn}~\left(=\frac{V}{2\pi rn}\frac{D}{D}=\frac{JD}{2\pi r}\right)$$
Since the angle of incidence $\alpha=\beta-\phi$, then:
$$\alpha=\arctan\frac{P}{2\pi r}-\arctan\frac{JD}{2\pi r}$$
When $P=JD$ (i.e. when $J=P/D$) the incidence along the entire blade is zero and the blade produces zero lift. (In practice it is unusual for all the radial locations of a blade to have the same pitch)
*(Note that P is Geometric Pitch, D is the Diameter of the Rotor, J is the Advance Ratio ($J=V/nD$), and r is the radius from the centre of the Rotor)*

**This means that as you increase speed your thrust will reduce, and when your thrust becomes zero you reach your maximum speed.**

### Design for Optimum Incidence
In practice it is unusual for all the radial locations of a blade to have the same pitch. In theory the radial twist of the blade can be such that the angle of incidence is constant along it's length (for a particular $J$) so that the entire blade can operate at it's best $L/D$.
For the incidence to remain constant along the length of the blade, the Geometric Blade Pitch Angle ($\beta$) for each radial station can be determined as follows:
$$\beta=\alpha+\phi$$
Thus:
$$\tan\beta=\tan(\alpha+\phi)=\frac{\tan\alpha+\tan\phi}{1-\tan\alpha\tan\phi}$$
But:
$$\tan\beta=\frac{P}{2\pi r}$$
So:
$$P=2\pi r\frac{\tan\alpha+ JD/ 2\pi r}{1-(JD /2\pi r)\tan\alpha}$$
Using the dimensionless quantities:
$$y=\frac{P}{D}~~~and~~~x=\frac{2r}{D}$$
$$y=\pi x\frac{\tan\alpha+(J/ \pi x)}{1-J\tan\alpha/\pi x}=J\frac{1+\pi x\tan\alpha /J}{1-J\tan\alpha/\pi x}$$
### Propeller Performance
General Aviation (GA) propellers are purchased “off the shelf” to best match the engine and airframe characteristics. Such proprietary propellers are tested in controlled conditions over a range of advance ratios (J).

These performance charts have a number of uses:
- Comparing the performance of commercially available propellers
- Choosing a propeller to suit a particular engine's power output characteristics
- Establishing the best blade pitch setting for a flight mission
- Determining the take-off or climb performance of an aircraft
- Providing a measure in the development of a new propeller design

Recalling the Coefficients used in the analysis of propeller performance:
$$J=\frac{V}{nD}$$
$$C_{P}=\frac{P}{\rho n^{3} D^{5}}$$
$$C_{T}=\frac{T}{\rho n^{2} D^4}$$
$$\eta_{P}=\frac{TV}{P}=\frac{C_{T}\rho n^{2}D^{4}V}{C_{P}\rho n^{4}D^{5}}=\frac{C_{T}J}{C_{P}}$$
