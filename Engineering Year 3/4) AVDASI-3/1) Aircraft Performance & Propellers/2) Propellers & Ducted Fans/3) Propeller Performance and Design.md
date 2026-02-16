### Propeller Pitch
>The **Geometric Pitch (P)** of a propeller is the theoretical axial displacement of the propeller prescribed by the geometric chord in one revolution.

>The **Effective Pitch (E)** is the actual axial displacement of the propeller (due to inflow)

The difference between these two lengths is called the **Propeller Slip**.
If the propeller blade has a radial twist such that all stations have the same Geometric Pitch the propeller is described as a **Constant Pitch Propeller**, as shown below:
![[Pasted image 20260216110932.png|centre|600]]

In this case $\beta$ is the angle to the horizontal and $\phi$ is the inflow angle. We can see that $P$ is described by $\beta$ and $E$ is described by $\phi$.

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

