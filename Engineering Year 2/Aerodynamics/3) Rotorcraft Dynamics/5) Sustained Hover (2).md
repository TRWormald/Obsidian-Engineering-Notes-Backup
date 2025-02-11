Today we will be looking at:
- Maximising the Figure of Merit
- The Coning Angle
### Recap on Rotor Efficiency
We have previously looked at the efficiency of a rotor, we defined this as:
$$\eta_{rotor}=\frac{\text{Output Power}}{\text{Input Power}}$$
This is the same as the "Figure of Merit" that we explored [[4) Sustained Hover (1)|last time]].
$$\eta_{r}=FoM=\frac{P_{i}}{P}=\frac{Tv}{P}$$
We also previously saw that the "Figure of Merit" was equal to the [[4) Sustained Hover (1)#Rotor Performance Coefficients|Thrust Coefficient]] ($C_{T}$) divided by the [[4) Sustained Hover (1)#The Torque and Power Coefficients|Power Coefficient]] ($C_{P}$) multiplied by $\lambda$:
$$FoM=\frac{C_{T}}{C_{P}}\lambda~~~~~~~~\text{where, }\lambda=\sqrt{\frac{C_{T}}{2}}$$
Hence:
$$FoM=0.707\cdot\frac{C_{T}^\frac{2}{3}}{C_{Q}}$$
Where $C_{Q}$ is the Torque Coefficient:
$$C_{Q}=\frac{Q}{\rho A(\Omega R)^{2}}$$
### Maximising the Figure of Merit (1)
![[Pasted image 20250211101328.png|centre]]
So increasing the velocity results in a proportional increase to the third power to the Power.
![[Pasted image 20250211101446.png|centre]]
### Forces Acting on the Rotor Blade
![[Pasted image 20250211101600.png|centre]]
The diagram above shows the forces acting on a rotor blade.
A singular infinitesimal element (In the hover case) has the following forces acting on it:
![[Pasted image 20250211101650.png|centre]]
### Maximising the Figure of Merit (2)
For a helicopter rotor, which has a finite number of blades, the blade element theory can be used to equate the lift on a <font color="#f79646">blade element</font> to the induced velocity in the <font color="#00b0f0">swept annulus</font> of that element:
![[Pasted image 20250211102603.png|centre]]
$$L=\frac{1}{2}\rho V^{2}SC_{L}$$
$$dL =\frac{1}{2}\rho \Omega^{2}r^{2}c ~dr ~a\alpha_{r}=dT$$
With:
$$\begin{align*}
v&= \sqrt{\frac{T}{2\rho A}},\\
dv&= \sqrt{\frac{dT}{4\rho \pi r~dr}}\\
&= \sqrt{\frac{\rho\Omega^{2}r^{2}c~dr~a~\alpha_{r}}{8\rho\pi r~dr}}
\end{align*}$$
So $dv$ is proportional to:
$$\sqrt{\frac{r^{2}\alpha_{r}}{r}}=\sqrt{r\alpha_{r}}$$
So for constant $v$, $\alpha_r$ is proportional to $\frac{1}{r}$.
