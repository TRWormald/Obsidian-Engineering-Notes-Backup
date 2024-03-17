From what we've learnt about [[The Moment of Inertia]], we can convert a system of linear forces applied to a rigid body into a single resultant force (and hence resultant acceleration) and [[Angular Acceleration]]:
![[Pasted image 20240301201127.png|center]]
\
We can use this to analyse complex systems:
##### Rolling Cylinder
Consider the following problem:
![[Pasted image 20240301201536.png]]
Where the slope is angled to the horizontal at angle $\beta$ and the cylinder has radius $R$ and the coefficient of friction between the cylinder and the surface is $\mu$.
We know that:
$$ \sum F_y=N-mg~cos\beta=m\ddot{y}$$
$$\sum F_x = F-mg~sin\beta=m\ddot{x}$$
The contact force between the cylinder and the surface can be calculated to be:
$$N=mg~cos\beta$$
So we now have two equations and three unknowns $F$, $\ddot{x}$ and, $\ddot{\theta}$
If we assume that $|F|\le\mu R$ (i.e. no slip conditions)
$$x=-\theta R$$
(i.e. the cylinder is purely rolling down the slope and the motion is completely described by the rolling of the cylinder)
So:
$$\ddot{x}=-\ddot{\theta}R$$
And some rearrangement gives:
$$\ddot{x}=-\frac{g~sin\beta}{1+(k_G/R)^2}$$
Note that we now have the traditional form for a mass sliding down a frictionless slope $\ddot{x}=-g~sin\beta$ and a rolling slow-down factor $1+(k_G/R)^2$.
Note that this explains why a hollow cylinder rolls slower down a slope compared with a solid cylinder of equal radius as the centre of gyration (see [[The Moment of Inertia]]) is lower for the solid cylinder resulting in a lower slow-down factor.
It is therefore possible to slow down acceleration by a lot when $k_G>R$, as seen in the diagram below (where the mass is concentrated further out from the radius):
![[Pasted image 20240301203201.png|center|400]]
##### Slipping and Rolling Cylinder
But what happens if the cylinder also slips as well as rolling.
So at the point of slipping:
$$\frac{F}{N}=\frac{tan\beta}{1+(R/k_G)^2}=\mu_s$$
With the same formulation as before:
![[Pasted image 20240301201536.png|center]]
$$\sum F_y = N-mg~cos\beta=m\ddot{y}=0$$
$$\sum F_x=\mu N-mg~sin\beta=m\ddot{x}$$
$$\sum M_G = \mu NR=I_G\ddot{\theta}$$
Where $M_G$ are the moments about the centre of mass.
If we combine these equations we get the following equations of motion:
$$\ddot{x}=g(\mu~cos\beta-sin\beta)$$
$$\ddot{\theta}=\frac{R~\mu~mg~cos\beta}{I_G}$$
Note that on a frictionless slope $\mu$ will be zero and therefore the cylinder will not rotate.