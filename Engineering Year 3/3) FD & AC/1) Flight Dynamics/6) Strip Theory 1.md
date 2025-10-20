Advised to read:
[[Chapter 13 - Aerodynamic Stability and Control Derivatives.pdf#page=1|Chapter 13 - Aerodynamic Stability and Control Derivatives, p.371 - Section 13.1]]
[[Chapter 13 - Aerodynamic Stability and Control Derivatives.pdf#page=34|Chapter 13 - Aerodynamic Stability and Control Derivatives, p.404 - Section 13.4]]

From the Equations of Motion we have seen:
$$\begin{align*}
\text{Fore/Aft:}~~~m(\dot{U}-rV+qW)&=X-mg\sin\theta\\
\text{Lateral:}~~~m(\dot{V}-pW+rU)&=Y-mg\cos\theta\sin\phi\\
\text{Transverse:}~~~m(\dot{W}-qU+pV)&=Z-mg\cos\theta\cos\phi\\
\end{align*}$$
From which we are interested in the $X,~Y,\text{and}~Z$ terms.

>It is more difficult to calculate overall basic lift distribution than to calculate additional lift components. These can be due to control surface deflections, due to aircraft movements away from steady level flight, or due to gusts. 
  **It is in these cases that strip theory is most useful.**

### Strip Theory Aerodynamics
![[Pasted image 20251003102035.png|centre]]
Above we can see a simple diagram of a wing with chord $c$, onset flow velocity $U$, and is split into infinitesimal strips of width $dy$.
The equation below defines the lift coefficient of this wing:
$$\huge{C_{L}\equiv \frac{L}{qS}=\frac{L}{\frac{1}{2}\rho u^2S}}$$
The essence of strip theory is to describe the differential element of lift that is generated on a single differential strip of a lifting surface. The underlying assumption of this method is that:

>"The lift on any strip is independent of the aerodynamics of all neighbouring strips"

Every strip is treated independently and its contribution to lift is expressed accordingly.
![[Pasted image 20251003102613.png|centre]]
Note how in the diagram above the strips are defined by the positions of the control surfaces. This is one possible way of applying strip theory.
#### The First Equation
For a single strip of an aerofoil (which for the moment has no camber so $a_{0}=0$) we can write:
$$\underbrace{dL}_\text{differential lift}=\underbrace{\frac{1}{2}\rho U^{2}}_\text{dynamic pressure}\cdot \underbrace{c~dy}_\text{differential area}\cdot \underbrace{C_{1}}_\text{coefficient of proportionality}$$
We can use a sectional lift coefficient, as opposed to a wing lift coefficient.
We can use the variation (with span) of this coefficient to generate expressions for the change in overall lift generated.
The graph below shows how the local lift coefficient changes with AoA, for a cambered and symmetric local section.
![[Pasted image 20251003103044.png|centre]]
#### Summation of Lift Producing Mechanisms
In practice we can allow for all normal lift-producing mechanisms, including a trim tab by summing their contributions to the local lift coefficient.
$$\huge{C_{l}=a_{0}+a_{1}\alpha+a_{2}\delta+a_{3}\beta}$$
(Note that in the equation above $\beta$ is the control tab deflection)