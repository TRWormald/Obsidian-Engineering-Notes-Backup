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
$$\gamma=\frac{\tau}{G}=\frac{q_{s}}{Gt}$$
Then the global energy balance is:
$$U_{ext}=U_{int}$$
$$\cancel{\frac{1}{2}}T\theta'\cancel{dz}=\oint \frac{1}{2}(q_{(s)}~ds)(\gamma \cancel{dz})$$
$$T\theta'=\oint\gamma\bar{q}~ds$$
$$T\theta'=\oint\frac{\bar{q}^{2}}{Gt}ds$$
Hence:
$$\boxed{\frac{d\theta}{dz}=\frac{1}{2\bar{A}}\oint\frac{\bar{q}}{Gt}ds}$$
### The Torsional Constant
If the shear modulus $G$ is constant then:
$$T=\theta'G\left(\frac{4\bar{A}}{\oint\frac{ds}{t}}\right)$$
And since:
$$\theta'=\frac{T}{GJ}$$
$$\boxed{J=\frac{4\bar{A}}{\oint \frac{ds}{t}}}$$
Or in discrete form:
$$J=\frac{4\bar{A}^{2}}{\sum\left(\frac{b_{i}}{t_{i}}\right)}$$
### Closed Sections Under Transverse Shear
Remembering the shear flow expression for open sections:
$$q_{(s)}^{open}=q_{0}-C_{x}\int_{0}^{s}x_{(s)}t_{(s)}ds-C_{y}\int_{0}^{s}y_{(s)}t_{(s)}ds$$
This equation is based on 1st moment of area relationships, so it must also hold for closed sections - i.e. it gives the correct "rate of change" of the shear flow around closed sections.
However closed sections no longer have a free edge where $q_{(s)}=0$.
Therefore, one needs to find this nonzero constant of integration, now called $\bar{q}$ which reveals the true shear flow $q_{(s)}^{closed}$:
$$\boxed{q_{(s)}^{closed}=q_{(s)}^{open}+\bar{q}}$$

The shear flow $\bar{q}$ can be interpreted in different ways:
1) A constant which must be added to the open shear flow to give the closed shear flow (as above)
2) The actual shear flow at the assumed notional cut
3) Constant shear flow required to counteract externally applied torque, effectively moving the shear centre to its correct location.
![[Pasted image 20241006144839.png|centre]]
#### Finding the Closed-cell Constant: Known Shear Centre
The torque is given by the shear centre offset $e_{x}$:
$$T=S_{y}e_{x}=\oint q_{(s)}^{open}r_{(s)}ds$$
So when loading the closed section through its shear centre we get:
$$\boxed{\bar{q}=-\frac{1}{2\bar{A}}\oint q_{(s)}^{open}r_{(s)}ds}$$
#### Finding the Closed-cell Constant: Unknown Shear Centre
If the location of the shear centre is unknown, we cannot find the 'local radius' $r_{(s)}$ directly.
Instead, we can derive an expression for $\bar{q}$ based on deformation:
$$ \frac{d\theta}{dz}=\frac{1}{2\bar{A}}\oint\frac{\bar{q}}{Gt}$$
