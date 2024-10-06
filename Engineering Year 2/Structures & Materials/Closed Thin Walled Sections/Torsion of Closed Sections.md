Consider the closed section in the following diagram to be in pure torsion:
![[Pasted image 20241006140604.png|centre|400]]
Pure torsion means that there are no shear or axial forces, i.e. no direct stresses:
$$\sigma_{z}=0$$
If we recall the differential shear flow equation for thin walled members:
$$t\cancel{\frac{d\sigma_{z}}{dz}}+\frac{dq_{(s)}}{ds}=0$$
So:
$$\frac{dq_{(s)}}{ds}=0$$
Therefore, the shear flow is constant throughout the section; we call it the **closed-cell shear flow** $\bar{q}$.
### Applied Torque vs Shear Flow
Writing the stress-resultant torque about an arbitrary point $O$ we get:
$$\begin{align*}
M_{z}=T&= \oint q_{{(s)}}r_{(s)}~ds\\
&= \bar{q}\oint r_{(s)}~ds
\end{align*}$$
The cross section of the closed section looks as follows:
![[Pasted image 20241006141126.png|centre|300]]
The area of a small triangle is given to be:
$$\frac{r_{(s)}~ds}{2}=d\bar{A}$$
And when integrating we get:
$$\oint r_{(s)}~ds=2\bar{A}$$
So:
$$T=\bar{q}(2\bar{A})~~~~~~~~\Rightarrow~~~~~~~~\bar{q}=\frac{T}{2\bar{A}}$$
Therefore for a constant torque $T$ the shear flow $\bar{q}$ is inversely proportional to the cell area $\bar{A}$.
### Angle of Twist and Torsional Stiffness
In pure torsion the deformation is given in terms of the **twist rate**, i.e. the angle of twist per unit shaft length:
$$\frac{\theta}{L}= \frac{d\theta}{dz}=\theta'$$
To find torsional stiffness - i.e. the relationship between applied torque $T$ and the angle of twist $\theta$, we must conduct an **energy balance**:
$$\text{applied external work}=\text{internal strain energy}$$
The **external work** done by the applied torque over the small 'slice' of depth $dz$ seen below is:
![[Pasted image 20241006141908.png|centre|250]]
$$U_{ext}=\frac{1}{2}\times\text{torque}\times{twist}$$
$$U_{ext}=\frac{1}{2}T~d\theta=\frac{1}{2}T\theta'~dz$$
The **internal strain energy** for the small element of depth $dz$ and arclength $ds$ seen below is:
![[Screenshot 2024-10-06 142018.png|centre|300]]
$$dU_{int}=\frac{1}{2}\times\text{force}\times\text{displacement}$$
$$dU_{int}=\frac{1}{2}(q_{(s)}~ds)(\gamma~dz)$$
If we assume linear elasticity, i.e:
$$\gamma=\frac{\tau}{G}=\frac{q_{s}}{GT}$$
Then the global energy balance is:
$$U_{ext}=U_{int}$$
$$\cancel{}$$