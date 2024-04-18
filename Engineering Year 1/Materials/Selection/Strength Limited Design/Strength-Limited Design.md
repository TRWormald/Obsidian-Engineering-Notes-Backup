In many cases our design is limited by the load carrying capacity of a component without it failing. In this case the material is limited by it's strength - although this might be the yield, tensile, or compressive strength or any other suitable limitation on the maximum stress depending on the application.
### Example: Strong, Light Tie

|                    | Translation Table                                        |
| ------------------ | -------------------------------------------------------- |
| **Function**       | Support a tensile force                                  |
| **Constraints**    | Support a force $F$ without yielding<br>Length specified |
| **Objectives**     | Minimise mass                                            |
| **Free Variables** | Choice of material<br>Cross-sectional area $A$           |
The objective (mass) equation is the same as for the light, stiff tie, and is independent of cross-sectional shape:
$$m=\rho AL_{0}$$
Given some minimum force the component must take without failing, the area must be big enough to keep the stress below the failure stress, this results in our constraint equation:
$$\sigma_{f}\ge \frac{F}{A}$$
Combining the two gives:
$$\begin{align*}
A&= \frac{F}{\sigma_f}\\
m&= \rho AL_{0}
\end{align*}
\Rightarrow m=FL_{0}\left(\frac{\rho}{\sigma_{f}}\right)
$$
And as a result the material index is therefore:
$$M=\frac{\rho}{\sigma_{f}} ~\text{or } M=\frac{\sigma_{f}}{\rho} =\text{Reciprocal merit index (to minimise m)}$$
Note that the reciprocal merit index is the specific strength of the material.
### Example: Strong Light Beams

|                    | Translation Table                                                                      |
| ------------------ | -------------------------------------------------------------------------------------- |
| **Function**       | Beam in bending                                                                        |
| **Constraints**    | Support moment $M$ without any yield<br>Length specified<br>Square cross-section (b=h) |
| **Objectives**     | Minimise mass                                                                          |
| **Free Variables** | Choice of material<br>Cross-sectional area $A$                                         |
Just like with the tie the mass objective equation is the same:
$$m=\rho AL_{0}$$
However we have to now consider the yield strength of the beam. This is related to [[Longitudinal Stresses in Beams#The Euler-Bernoulli Beam Theory|Euler-Bernoulli Beam Theory]]:
$$\frac{M}{I}=\frac{\sigma}{y}=\frac{E}{R}$$
In this instance we only want to compare the bending moment $M$ and the yield strength:
$$\sigma_{max}=\frac{M\cdot y_{max}}{I}$$
As we know $y_{max}$ is the maximum distance from the neutral axis of the beam (typically the centre as it passes through the centroid of the cross section) and $I$ is the [[Second Moment of Area]].
We can rewrite this equation as:
$$\sigma_{max}=\frac{C_{2}FL}{Z_{e}}$$
Where $C_{2}$ is a constant reflecting the type of loading, $F$ is the load applied, and $L$ is the length of the beam, whilst $Z_e$ is the **elastic section modulus** and is equal to $\frac{y_{m}}{I}$ as can be seen by observation.
\
**Note that if the stress exceeds $\sigma_{y}$ then the beam progresses into plasticity until the entire beam is plastic and we get sudden plastic collapse.**
This is modelled by the plastic section modulus $Z_{p}$.
Below are the Elastic, and Plastic Section Moduli of several common shapes:
![[Pasted image 20240418160427.png|center|450]]
\
As we are considering a square beam we know that:
$$\sigma_{y}\ge \frac{M}{Z_{e}}=\frac{6M}{bh^{2}}=\frac{6M}{h^{3}}$$
The objective and constraint equations are coupled by the area so we can eliminate this free variable:
$$h=\left(\frac{6M}{\sigma_{y}}\right)^\frac{1}{3}$$
$$A=h^{2}=$$