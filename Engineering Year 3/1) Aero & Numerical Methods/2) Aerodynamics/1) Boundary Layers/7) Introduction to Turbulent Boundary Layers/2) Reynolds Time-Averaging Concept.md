### The Turbulent Boundary Layer Equations
As with laminar boundary layers we have:
$$\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}=0$$
$$u\frac{\partial u}{\partial x}+v\frac{\partial u}{\partial y}=-\frac{1}{\rho} \frac{dp}{dx}+\nu\frac{\partial^{2}u}{\partial y^{2}}$$
But now we represent the flow properties as a sum of the mean plus the turbulent fluctuation:
$$u=\hat{u}+u'$$
#### Mean and Fluctuating Components
![[Pasted image 20251030015440.png|centre]]
### The Continuity Equation
Substituting these Reynolds decomposed variables into the continuity equation gives:
$$\frac{\partial u}{\partial x}+\frac{\partial v}{\partial y}=\frac{\partial(\hat{u}+u')}{\partial x}+\frac{\partial()\hat{v}+v'}{\partial y}=0$$
We now would like to perform Reynolds averaging. If we average over the timescale of fluctuation but less than that of anything we are interested in, then:
### Properties of Time Averaged Variables
![[Pasted image 20251030015742.png|centre|400]]
![[Pasted image 20251030015754.png|centre|400]]
### Reynolds Averaged Navier Stokes
From this we can see that:
$$\frac{\bar{\partial \hat{q}}}{\partial x}=\frac{\partial\bar{\hat{q}}}{\partial x}=\frac{\partial \hat{q}}{\partial x}$$
As the mean of a gradient is the gradient of a mean.
And also,
$$\frac{\bar{\partial q'}}{\partial x}=\frac{\partial \bar{q'}}{\partial x}=0$$
As time averaging and differentiation are commutative.
So returning to the continuity equation and time averaging:
$$\frac{\overline{\partial(\hat{u}+u')}}{\partial x}+\frac{\overline{\partial(\hat{v}+v')}}{\partial y}=0$$
So:
$$\frac{\overline{\partial \hat{u}}}{\partial x}+\frac{\overline{\partial u'}}{\partial x}+\frac{\overline{\partial\hat{v}}}{\partial y}+\frac{\overline{\partial v'}}{\partial y}=0$$
But, using our rules from earlier, the time average of the fluctuating differentials are zero so:
$$\frac{{\partial \hat{x}}}{\partial x}+\frac{{\partial \hat{v}}}{\partial y}=0$$
Similarly we can show that the x-momentum equation becomes:
$$\hat{u}\frac{\partial \hat{u}}{\partial x}+\hat{v}\frac{\partial\hat{v}}{\partial y}=- \frac{1}{\rho}\frac{d\hat{p}}{dx}+\frac{\partial}{\partial y}\left(\nu \frac{\partial \hat{u}}{\partial y}-\overline{u'v'}\right)-\frac{\overline{\partial u'^{2}}}{\partial x}$$
Where the last two terms are called the Reynolds Stresses. We sometimes ignore the final one due to the thin layer assumption. Overall the continuity and momentum equations are the same in turbulent flow as laminar, as long as we use time averaged values.
### The Boussinesq Hypothesis
The extra stress acts just like a viscous stress, but is a function of local flow variables. This is in analogy with how the momentum transfer caused by the molecular motion in a gas can be described by a molecular velocity.
In turn this means that the boundary layer equations become:
![[Pasted image 20251030021130.png|centre]]
### Finally
The problem now is that we have more unknowns than equations. Finding additional equations that give good results is the field of turbulence modelling. The additional equations often mimic physical ones and are largely empirical. Sometimes further unknowns are introduced to model more complicated effects.
