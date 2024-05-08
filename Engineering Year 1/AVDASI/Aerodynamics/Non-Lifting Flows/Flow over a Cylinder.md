The flow over a cylinder is modelled as a [[Uniform Horizontal Flow]] and a [[Doublet]]:
\
![[Pasted image 20240220170420.png]]
\
#### Step 1 - Obtain the Velocity Field
By combining the potential functions from [[Uniform Horizontal Flow]] and a [[Doublet]] we can calculate:
\
$$ u=U_\infty + \frac{-\kappa}{2\pi}\frac{(x^2-y^2)}{(x^2+y^2)^2}~~~,~~~~ v=\frac{-\kappa}{2\pi}\frac{2xy}{(x^2+y^2)^2}$$
#### Step 2 - Find the Stagnation Points
The stagnation points occur when $u$ and $v$ are both equal to zero, hence:
\
$$ v=\frac{-\kappa}{2\pi}\frac{2~x_{stag}y_{stag}}{(x_{stag}^2+y_{stag}^2)^2}=0$$
\
So $v=0$ when $x_{stag}$ or $y_{stag}$ is equal to zero
\
Following on from that, if $y=0$:
\
$$ u=U_\infty - \frac{\kappa}{2\pi}\frac{1}{x^2} $$
\
So if $u=0$:
\
$$ x=\pm\sqrt{\frac{\kappa}{2\pi U_\infty}}$$
\
Which gives the cylinder $R= x=\pm\sqrt{\frac{\kappa}{2\pi U_\infty}}$ (as the dividing streamline is equidistant from the doublet at all points).
\
For a circle $x^2+y^2=R^2$ while $x=Rcos(\theta)$ and $y=Rsin(\theta$) so the velocities are:
\
$$u=U_\infty+\frac{-\kappa}{2\pi}\frac{cos^2\theta-sin^2\theta}{R^2}=U_\infty-U_\infty(cos^2\theta-sin^2\theta)=2U_\infty sin^2(\theta)$$
\
$$v=\frac{\kappa}{2\pi}\frac{2cos\theta sin\theta}{R^2}=-2U_\infty ~cos\theta~sin\theta$$