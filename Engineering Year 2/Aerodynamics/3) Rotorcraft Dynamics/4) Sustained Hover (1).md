### Ground Effects
![[Pasted image 20250202202944.png]]
Ground effect is a special kind of condition that really only effects rotorcraft. It occurs when the rotorcraft is close to the ground, and results in the induced power requirement being lower due to a greater generation of lift.
Below we can see the graph of Thrust Enhancement in comparison to Height off the Ground:
![[Pasted image 20250202203116.png|centre]]
As we can see, the lower the craft the greater the thrust enhancement factor - with thrust increasing buy up to 1.3x when close to the ground.
### Rotor Efficiency
How do we calculate the efficiency of a rotorcraft, in many ways it is similar to how we calculate the efficiency of any other system:
$$\text{Efficiency}=\eta=\frac{\text{Output Power}}{\text{Input Power}}$$
For a rotor:
![[Pasted image 20250202203315.png|centre]]
However the measure of propeller efficiency,
$$\eta_{p}=\frac{TV}{P}$$
Is not suitable for the helicopter, so we use a "Figure of Merit":
$$\eta_r=\text{FoM}=\frac{P_{i}}{P}=\frac{Tv}{P}$$
Where $P_{i}$ is the induced power and $P$ is the rotor shaft power (note that this makes $v$ the induced velocity).
Therefore we can substitute in the equation for induced velocity to obtain:
$$\begin{align*}
\eta_{r}&=\frac{T}{P}\sqrt{\frac{T}{2\rho A}}\\
&= \frac{T^{\frac{3}{2}}}{P}\sqrt{\frac{1}{2\rho\pi R^2}}
\end{align*}$$
So therefore the $FoM$ is inversely proportional to the rotor diameter, and therefore comparative studies should be limited to rotors of the same diameter.
### Rotor Efficiency In Hover
We previously ascertained that:;
$$\eta_r=\text{FoM}=\frac{Tv}{P}=\frac{T}{P}\sqrt{\frac{T}{2\rho A}}$$
If $\frac{T}{P}=PL$ (known as power loading) and $\frac{T}{A}=DL$ (known as disk loading) then:
$$PL=1.565*\text{FoM}*\frac{1}{\sqrt{DL}}$$
This relationship can be plotted if the Figure of Merit is known, then for a given disk loading the power loading may be found from the graph:
![[Pasted image 20250202204043.png|centre]]
