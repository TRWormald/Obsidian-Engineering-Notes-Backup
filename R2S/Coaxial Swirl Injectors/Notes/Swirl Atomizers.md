### Pros and Cons
Swirl atomisers are commonly used because they have the following **advantages** compared to other nozzles:
1) Relatively simple design
2) High reliability
3) Good spraying quality
4) Small power required
However they do have the following **disadvantages**:
1) Limited use for atomisation of very viscous fuels
2) Small range of regulation, where regulation is understood as the ratio of the maximum and minimum flow rates
### Characteristic Parametrisation
A schematic diagram of the simplest swirl atomiser is shown below:
![[Pasted image 20241127140224.png|centre|400]]
The characteristic parameters of swirl atomisers are represented by the geometric constant $K$:
$$K=\frac{Rr_{0}}{ir_{p}^{2}}=\frac{2Rd_{0}}{id_{p^2}}=\frac{\pi Rr_{0}}{iA_{p}}=\frac{2\pi Rd_{0}}{4iA_{p}}$$
Note that:
- $R$ is the swirl radius
- $r_{p}$ and $d_{p}$ are the radius and diameter of the tangential orifice, respectively
- $r_{0}$ and $d_{0}$ are the radius and diameter of the discharge orifice, respectively
- $i$ is the number of tangent inlet orifices
- $A_{p}$ is the cross section of the tangential inlet orifice with an arbitrary transverse shape
If the tangential inlet orifices are inclined to the swirl chamber axis at angle $\Theta$ then this equation assumes the form:
$$K=\frac{Rr_{0}}{ir_{p}^{2}}\sin\Theta=...$$
### Design
#### Volumetric and Mass Flow Rates
We can calculate the volume and mass flow rates using the following equations:
$$Q=\frac{1}{\sqrt{\frac{K^{2}}{1-\epsilon}+ \frac{1}{\epsilon^{2}}}}\cdot\pi r_{0}^{2}\sqrt{\frac{2P_{t}}{\rho}}=\boxed{\mu A_{0}\sqrt{\frac{2\Delta P}{\rho}}}$$
Where $\mu$ is the discharge coefficient, which depends on two quantities: the geometric constant $K$ and the efficiency of filling the discharge orifice $\epsilon$.
This can be calculated using:
$$\epsilon=\frac{A}{A_{0}}=\frac{\pi(r_{0}^{2}-r_{2}^{2})}{\pi r_{0}^{2}}=1-\left(\frac{r_{r}}{r_{0}}\right)^{2}$$
Where $A_{0}=\pi r_{0}^{2}$ which is the area of the discharge orifice, and $r_{r}$ is the gas core 