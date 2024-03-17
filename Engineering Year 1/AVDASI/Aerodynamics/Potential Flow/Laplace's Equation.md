Kelvin's Theorem:
"*In the absence of viscous forces and discontinuities the flow till remain irrotational*"
\
We know how [[Irrotational Flow]] is defined, and discontinuities come from free surfaces (multi-phase flows) or shock waves (only present in compressible flows). Inviscid incompressible flows are always irrotational.
\
For incompressible flows the mass conservation equation becomes:
\
$$\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}+\frac{\partial w}{\partial z}=0 $$
\
As the density of the fluid cancels out.
\
\
Irrotationality guarantees the existence of a scalar 'velocity potential function' $\phi$.
Where (if the flow is irrotational):
$$ u=\frac{\partial\phi}{\partial x},v=\frac{\partial\phi}{\partial y},w=\frac{\partial\phi}{\partial z}$$
\
Substituting the second equation into the first we get:
$$\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}+\frac{\partial w}{\partial z}= \frac{\partial}{\partial x} \frac{\partial\phi}{\partial x}+\frac{\partial}{\partial y} \frac{\partial\phi}{\partial y}+\frac{\partial}{\partial z} \frac{\partial\phi}{\partial z}=0$$
Or:
$$\frac{\partial^2\phi}{\partial x^2}+\frac{\partial^2\phi}{\partial y^2}+\frac{\partial^2\phi}{\partial z^2}$$
Which is the Laplace Equation.
Note that it is a **linear** 2nd order partial differential equation - this means that solutions can be superimposed on each other (flow models built up from 'elementary' flow solutions)