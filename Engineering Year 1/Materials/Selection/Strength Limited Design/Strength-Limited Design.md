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
