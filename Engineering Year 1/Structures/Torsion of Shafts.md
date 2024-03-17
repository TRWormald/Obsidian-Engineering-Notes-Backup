When calculating the torsion in shafts we make several assumptions:

1) The Shaft is in Pure Torsion (i.e. there are no other loads applied to the Shaft)
2) The rotations applied to the shaft are small (This is important so that we can use small angle approximations later
\
To derive the equation relating load to angle of deformation we need to work backwards:
\
Define Deformation ($\phi$) -> Define Strains ($\gamma$) -> Define Stress ($\tau$)-> Define Load ($T$)

## Defining the Deformation
Consider a shaft which is clamped at one end with length $L$ and radius $R$. Now consider a point/particle at the end of the shaft (at the radius) and its motion as Torsion is applied.
The point's motion can be defined by the equation:
\
$$s=\phi R$$
Where:
$s$ is the distance around the centre of the shaft that the particle has traversed
$\phi$ is the angle that the shaft has been rotated by (in radians)
$R$ is the radius of the shaft
\
Now consider: 
1) The fact that $s$ decreases as we move closer to the clamp
2) The fact that $s$ decreases as we move closer to the centre of the shaft
\
From this we can deduce that $s$ must be a function of the distance from the clamp and the distance from the centre of the shaft, hence:
\
$$s(x,r)=\phi (x)r$$
\
Where:
$r$ is the distance from the centre of the shaft
$\phi$ is the angle of rotation (which is a function of the distance from the clamp ($x$)- and is maximum when $x=L$)

## Defining the Strain
From the definition of [[Shear Strain]] ($\gamma$) we can deduce that it is equal to $arctan(\frac{s}{L})$, however as we are assuming that the angle of twist is small $arctan(\frac{s}{L}) \approx\frac{s}{L}$ so:
\
$$ s=\gamma L=\gamma x$$ \
From before we know that $s=\phi r$ and as such $\phi r=\gamma x$ leading to:
\
$$s(x,r)=\gamma x$$
\
As when we are at distance L from the clamp $\phi$ is constant but $s$ decreases as we move towards the centre we can deduce that:
\
$$\gamma (r)=\frac{\phi r}{L}$$
\
So $\gamma_{max}$ occurs at $r=R$ hence:
\
$$\gamma_{max}=\frac{QR}{L}$$
Leading to:
$$\gamma (r)=\frac{r\cdot\gamma_{max}}{R}$$
## Defining the Stress
From the definition of [[Shear Stress]] ($\tau$) we know that to calculate it all we need to do is multiply the [[Shear Strain]] by the [[Shear Modulus]]:
\
$$\tau (r)=G\cdot\gamma(r)=G\cdot\frac{r\cdot\gamma_{max}}{R}$$
\
## Defining the Load/Torque
Consider the cross section of the shaft and an infinitesimal area of that area ($dA$). That area has some shear stress applied to it and the sum of all of these should equal the total torque:
So considering the small area:
$$dT=\tau (r)~r\cdot dA$$
Where:
$dT$ is some small torque applied by the shear stress at that point
$\tau$ is the shear stress
$r$ is distance from the centre of the shaft
\
Integrating that gives:
\
$$T=\int r~\tau(r)\cdot dA$$
Where:
$$\tau (r)=\frac{r}{R}\cdot\tau_{max}$$
So:
$$T=\frac{\tau_{max}}{R}\cdot\int r^2\cdot dA$$
\
By observation $\int r^2\cdot dA$ is the [[Polar Second Moment of Area]] ($J$) resulting in:
\
$$\tau_{max}=\frac{TR}{J}$$
\
However we can also form a different equation by leaving the shear stress in terms of the strain:
\
$$T=\int r~G~\gamma(r)\cdot dA=\int r~G~\frac{\phi(r)~r}{L}\cdot dA=\frac{G~\phi(L)}{L}\int r^2\cdot dA$$
\
Which is:
$$T=\frac{G~J}{L}\cdot\phi(L)$$
\
We can compare this equation to the traditional Hooke's law equation $F=ku$ (where $F$ is the force applied $k$ is the stiffness and $u$ is the change in displacement) and see that $\frac{G~J}{L}$ is similar to the stiffness term. As a result we call it the "Shaft Torsional Stiffness"