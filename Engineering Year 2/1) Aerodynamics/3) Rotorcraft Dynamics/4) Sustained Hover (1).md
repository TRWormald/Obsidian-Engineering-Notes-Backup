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
### Rotor Performance Coefficients
The general thrust coefficient:
$$T_{c}=\frac{T}{\rho V^{2}D^{2}}$$
has limited value for helicopter rotors has it has infinite value at $V=0$.
A more suitable coefficient is:
$$C_{T}=\frac{T}{\rho A(\Omega R)^{2}}$$
Which gives a thrust coefficient based upon tip rotor speed $\Omega R$ and rotor disk area $A$.

Note that, whilst the above equation for $C_{T}$ has become the accepted form some textbooks might show:
$$C_{T}=\frac{T}{\frac{1}{2}\rho V^{2}_{T}A}$$
Where $V_{T}=\Omega R$, or some other variation on this theme.
#### The Torque and Power Coefficients
Similarly:
$$C_{Q}=\frac{Q}{\rho AR(\Omega R)^{2}}$$
$$C_{P}=\frac{P}{\rho A(\Omega R)^{3}}$$
Therefore $C_{P}=C_{Q}$
#### The Advance and Inflow Ratios
it is also normal to express the forward speed $V$ of the helicopter relative to the tip speed parameter $\Omega R$ - this is called the Advance Ratio $\mu$, thus:
$$\mu =\frac{V}{\Omega R}$$
In a similar way, the flow through the rotor ($v$ in hover, but $V_{V}+v$ otherwise) is non-dimensionalised by $\Omega R$ and this is called the inflow ratio $\lambda$, thus:
$$\boxed{\lambda=\frac{V_{V}+v}{\Omega R}}$$
Note that in hover $V_{V}=0$.
#### The Figure of Merit
We previously defined the figure of merit in terms of thrust, power and velocity, however we can also use the relations that we have just found above to calculate it in terms of the non-dimensionalised coefficients:
$$\text{FoM}=0.707\frac{C_{T}^\frac{2}{3}}{C_{Q}}$$
With an important intermediary step being figuring out that:
$$\lambda=\sqrt{\frac{C_{T}}{2}}$$
When the rotorcraft is in hover (i.e. when $V_{V}=0)$.
