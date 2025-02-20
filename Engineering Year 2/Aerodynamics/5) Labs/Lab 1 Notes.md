##### What is the value of the Reynolds Number at 20$ms^{-1}$?
$$Re=\frac{\rho uL}{\mu}=\frac{\text{inertial forces}}{\text{viscous forces}}$$
Higher Reynolds numbers = Turbulence
Lower Reynolds numbers = Laminar
So:
$$Re=\frac{1.225*20*0.25}{1.82*10^{-5}}=337000$$

##### What is the value of the Mach Number at 20$ms^{-1}$?
Mach number gives us an idea about the compressibility.
$$M=\frac{u}{a}$$
Mach number is a ratio of speed against the speed of sound.
$$M=\frac{20}{340}=0.07$$
##### What do the numbers in the NACA 23015 aerofoil designation mean?
$$\text{NACA}~\underbrace{2}_{\text{Design }C_{l}= \frac{0.1*3}{2}*x}\underbrace{3}_{\begin{matrix}\text{3/20 is the}\\\text{location of max camber }\end{matrix}}\underbrace{0}_{\begin{matrix}\text{normal or }\\\text{reflex camber }\end{matrix}}\underbrace{15}_{\begin{matrix}\text{max thickness }\\\text{wrt. chord}\end{matrix}}$$
##### How does flap deflection influence the maximum $C_{l}$ (the $C_{l}$ at stall)? Why might this be useful?
We see an increase in $C_{l_{max}}$ with increasing flap deflection, however we also see:
- Stall at a lower angle
- Zero lift coefficient at a negative AoA

These are useful properties when we are landing or taking off as we can take off slower.
##### How does the flap deflection influence stall angle?
Greater flap deflection results in a lower stall angle.
##### Illustrate with a diagram the regions of adverse and favourable pressure gradient. Will separation usually occur under an adverse or favourable pressure gradient?
A favourable pressure gradient is where the pressure is decreasing in a section of the $C_{p}$ vs $\frac{x}{c}$ graph. So the velocity is increasing and the flow is being pulled along by the flow.
An adverse pressure gradient is where the pressure is increasing in a section of the same graph. So the velocity is decreasing and we are using energy to compress the fluid.

We are likely to see separation when there is an adverse pressure gradient. i.e. towards the rear of the wing.
##### Where does the flow first separate from the aerofoil? What type of stall is this? Is the stall gradual or sudden? What would happen for a thinner section?


##### How does the lift curve slope compare to the flat plate potential flow result of $2\pi$/radian? List three potential reasons for the difference.
##### Definition and usage of $C_{p}$
$$C_{p}=\frac{p-p_{\infty}}{\frac{1}{2}\rho V^{2}}$$
##### Definition and Usage of $C_{l},~C_{m},~C_{d}$
$$\begin{bmatrix}C_{x}\\C_{y}\end{bmatrix}=\oint C_{p}\mathbf{n}~d\left(\frac{s}{c}\right)$$
Where $\mathbf{n}$ is the unit normal.
$$\begin{bmatrix}C_{l}\\C_{d}\end{bmatrix}=\begin{bmatrix}\cos(\alpha)&-\sin(\alpha)\\\sin(\alpha)&\cos(\alpha)\end{bmatrix}\begin{bmatrix}C_{x}\\C_{y}\end{bmatrix}$$
$$C_{m}=\oint C_{p}\mathbf{n}\times\mathbf{d}d\left(\frac{s}{c}\right)=\oint C_{p}\begin{bmatrix}\Delta y\\-\Delta x\end{bmatrix}\times\begin{bmatrix}x_{m}-x_{ref}\\y_m-y_{ref}\end{bmatrix}~d\left(\frac{s}{c}\right)$$
Where $\mathbf{d}$ is the vector from the reference point to the location for that $C_p$ value. Please also refer to section 5 in this document for more details. How would you find $C_{l,d,m}$ numerically from the experimental data (you will do this later using the data in the spreadsheet)?
##### Sketch the influence of boundary layer transition on $C_{p}$ vs. $\frac{x}{c}$
##### Contributions to $C_{d}$ come from skin friction and normal pressure forces/ Which are measurable in this experiment? Why would it be unwise to measure $C_{d}$ by surface integration?
##### What effect to the wind tunnel walls have on $C_{l_{max}}$
##### The aerodynamic centre $x_{ac}$ is the location about which pitching moments do not change with angle of attack, $i.e.~~ \frac{dC_{m_{AC}}}{d\alpha}=0$
$$M_{LE}=M_{AC}-Lx_{AC}$$
$$\frac{dC_{m_{LE}}}{d\alpha}=-\frac{dC_{l}}{d\alpha}\frac{x_{AC}}{c}$$
Now calculate $x_{ac}$:

##### Calculate the ratio of the projected frontal area of the aerofoil to the cross sectional area of the tunnel (0.6 x 0.6m) for small to high incidences. This is termed the blockage factor - is it acceptably small? What does this imply about measurements at higher incidences? Recall the aerofoil is 15% thick, and the chord is about 25cm.
##### How will flap deployment change the handling of an aircraft?
##### What is hysteresis, what causes it and what does this imply for recovery of a stalled aircraft? Note in free air hysteretic effects will be smaller than seen in the confined space of this wind tunnel owing to wall effects.