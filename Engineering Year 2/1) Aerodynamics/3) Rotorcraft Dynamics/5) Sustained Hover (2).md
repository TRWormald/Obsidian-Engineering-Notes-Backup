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
$$C_{Q}=\frac{Q}{\rho AR(\Omega R)^{2}}$$
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
![[Pasted image 20250211103134.png|centre]]
### Ideal Blade Twist
Ideal Blade Twist results in a constant induced velocity across the rotor disk.
It has been seen that for this to be the case, then $\alpha_{r}\propto \frac{1}{r}$.
For this to be the case:
$$\alpha_{r}=(\theta-\phi)=\frac{R}{r}(\theta_{t}-\phi_{t})$$
So $\phi=\phi_{t} \frac{R}{r}$, where $\phi_{t}$ is the inflow angle at the tip.
Similarly the blade pitch angle:
$$\theta=\theta_{t} \frac{R}{r},\text{where }\theta_{t}\text{ is the pitch angle at the tip}$$
Thus by careful design the ideal inflow can be achieved by blade twist, or blade planform taper, or a combination of the two.
Unfortunately the other requirements for ideal conditions (zero profile drag, tip losses and swirl in the wake) are not so easily met and must, at best, be minimised.
![[Pasted image 20250223160225.png|centre]]
Returning briefly to the diagram above, note how inflow angle $\phi$ can be calculated using the following formula:
$$\phi=\arctan\left(\frac{v}{\Omega R}\right)$$
As it is the angle subtended by the line drawn from the induced velocity vector when it is perpendicular to the tip of the velocity component due to blade rotation.
### Thrust Coefficient for a Rotor with Ideally Twisted Blades
![[Pasted image 20250211102603.png|centre|centre]]
For the diagram above (with $a$ being the section lift curve slope):
$$dL=\frac{1}{2}\rho (\Omega r)^{2}a \frac{R}{r}(\theta_{t}-\phi_{t})c~dr$$
So:
$$\begin{align*}
L&= \int_{0}^{R}\frac{N}{2}\rho \Omega^{2}rRa(\theta_{t}-\phi_{t})c~dr\\
&= \frac{N}{4}\rho\Omega^{2}R^{3}a(\theta_{t}-\phi_{t})c~~~~~~~(\approx T)
\end{align*}$$
So:
$$\begin{align*}
C_{T}&= \frac{T}{\rho A (\Omega R)^{2}}=\frac{N}{4}\frac{\rho\Omega^{2}a R^{3}(\theta_t-\phi_{t})c}{\rho\pi\Omega^{2}R^{4}}\\\\

&= \frac{Na(\theta_t-\phi_{t})c}{4\pi R}
\end{align*}$$
Or:
$$C_{T}=\frac{\sigma}{4}a(\theta_{t}-\phi_{t}),~~~~\text{where}~~\sigma=\frac{Nc}{\pi R}$$
### The Effect of Blade Profile Drag and Rotor Solidity
The rotor blade element of drag is composed of two components; the profile drag and the induced drag. The resultant drag in the plane of the rotor is:
$$dD\cos\phi+dL\sin\phi$$
Since $\phi$ is small this can be written as:
$$dD+dL\phi$$
Or in coefficient form as:
$$C_{d_{0}}+\phi C_{l}$$
Thus the in plane drag torque due to this element is:
$$dQ=\frac{N}{2}\rho(\Omega r)^{2}c(C_{d_{0}}+\phi C_{l})r~dr$$
Assuming that $C_{d_{0}}=\delta$ is relatively constant over the range of $\alpha$ then we can assume that $C_{d_{0}}$ is a constant.
Using our previous assumptions and plugging them into the torque equation we can eventually derive that:
$$\boxed{\boxed{FoM=0.707\frac{C_{T}^{\frac{3}{2}}}{\frac{C_{T}^{\frac{3}{2}}}{\sqrt{2}}+\frac{\sigma\delta}{8}}}}$$
![[Pasted image 20250211105007.png|centre]]
In hover, we can again use SAA, so $L=T=W$, so the weight is the summation of all the blade elemental lift force, therefore:
$$\boxed{\bar{C}_{L}=6\frac{C_{T}}{\sigma}}$$
But to derive this we've also obtained:
$$L=T=C_{T}\pi R^{2}\rho(\Omega R)^{2}$$
Where $\bar{C_{L}}$ is the mean lift coefficient, and $\sigma=\frac{N c}{\pi R}$. *Note that sometimes the mean lift coefficient is called the equivalent lift.*
When plotted against the FoM, the effect of solidity becomes apparent:
![[Pasted image 20250218124212.png|centre]]
Reducing rotor solidity increases the FoM, but with diminishing effect at higher $C_{T}/\sigma$.
### Rotor Blade Tip Loss Factors
![[Pasted image 20250218124304.png|centre]]
Unlike the actuator disk, a real rotor blade cannot support lift right out to the blade tip. A tip loss factor B (usually 0.95 -0.97) can be used in analysis whereby it is assumed that blade drag exists over the entire blade length but no lift is generated outboard of radius BR.
### Blade Loading and Blade Coning
![[Pasted image 20250218124404.png|centre]]
Generally the rotor blade has the facility to freely flap about a hinge at the rotor hub. To prevent the blade drooping too much in the static case, droop stops are usually employed.
![[Pasted image 20250218124458.png|centre]]
As the rotor starts to turn, the C.F. lifts the blades off the droop stop. With increasing rotor speeds the droop stops are automatically withdrawn.
