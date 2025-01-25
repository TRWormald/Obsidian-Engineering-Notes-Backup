So far sources, sinks, or vortices have been added to a uniform flow and then any streamline of the resulting flow patter may be taken to represent a solid surface since no flow can cross it.
But this *direct* approach is very restrictive. A more general approach is needed that will allow the potential flow solution about arbitrary aerofoils to be calculated.
### The Generalised Method
There are a number of steps to the general method:
1) We will introduce a discrete set of singularities (point sources, doublets, and/or vortices) of unknown strength at predefined locations to a freestream flow.
2) We will then apply the boundary condition that the body surface is a stream line to construct a set of equations to solve for the unknown strengths of these singularities.
3) However applying the boundary condition doesn't immediately yield a unique solution because:
	- The singularity type, number and positions can vary
	- Physical considerations need to be introduced to fix the correct level of circulation (i.e. the Kutta condition must be enforced)

Therefore the first question that we need to ask is:

>*Which point singularities are appropriate to use to model the flow?*

This depends on the flow:
- Point sources/sinks can be used to model flows over non lifting bodies
- Point doublets can be used to model flows over lifting and non-lifting bodies
- Point vortices can be used to model flows over lifting and non-lifting bodies

We can also develop combined methods using:
- Sources and Doublets
- Sources and Vortices

We will be focusing on a *generalised point source model* for non-lifting flows. This is the simplest method to implement as sources will automatically yield zero circulation and hence zero lift.
We will return to point vortex models for thin aerofoils since a means to enforce [[3) The Kutta Condition|The Kutta Condition]] arises from the simplified analytic thin aerofoil theory.
### Example - A Generalised Point Source Model
>A non-lifting flow over a body is to be modelled using point sources added to a freestream

First $N$ locations are chosen for the point sources (**singularities**). The sources have unknown strength $\Lambda_{j}$. *Note: The impact of the placement of sources will be considered later.*

Since there are $N$ unknown strengths and we don't have to worry about fixing circulation then the streamline condition can be enforced at $N$ locations on the body. 
These locations are called **control points** or **collocation points**.
The diagram below shows the method pictorially:
![[Pasted image 20250125145631.png|centre]]
*Note: The singularities must be placed within the geometry as we cannot have locations where flow tends to infinity in the flow field.*

The boundary condition at the body surface is a streamline at the control points can be applied in two ways:
1) The first way is by directly setting the flow velocity normal to the body surface at the control points to be zero. This is called a **Neumann** condition.
2) An alternative approach specifies the potential on the body surface to make it a streamline. This is called a **Dirichlet** condition.
*In this example/course we will use the **Neumann Condition***.
#### The Solution Process
First we work out the surface normal $\vec{n}_{i}$ to the body at the control points and hence the surface normal component of the velocity induced by each source at every control point. So for example, for source $j$ the normal velocity induced at control point $i$ is given by:
$$(V_{n})_{i,j}=a_{i,j}\Lambda_{j}$$
Where $a$ is the velocity influence coefficient.
The boundary condition of no normal flow is then applied at each control point by combining the surface normal velocities induced by all the sources and the freestream.
$$\sum\limits_{j=1}^{N}a_{i,j}\Lambda_{j}+\vec{V}_\infty\cdot\vec{n}_{i}=0$$
Combining these equations for all $N$ control points yields a linear set of equations to solve one of the form:
$$A\vec\Lambda=\vec{R}$$
Where:
$$\vec\Lambda=[\Lambda_1,\Lambda_{2},...,\Lambda_{n}]^T$$
$$\vec{R}=[R_{1},R_{2},...,R_{N}]^{T}$$
$$A \text{ is a matrix with entries } a_{i,j}$$
This equation is then solved for the point sources strengths and then secondary quantities such as pressures, forces, and off body velocities predicted by the model can be calculated.
### Summary of the Process of Model Generation
1) Geometry Discretisation
2) Calculation of *influence coefficients* and *influence matrix* equation
3) Solution of the linear set of equations
4) Secondary calculations: pressures, forces, off-body velocities
### Where Should We Place Point Sources and Control Points
The most common approach with point sources is to place sources on the line of symmetry. We will consider this placement first using a circular cylinder as an example.
We are doing this because we have an analytic potential solution.
In the following figures circles represent sources and crosses the control points.
![[Pasted image 20250125163753.png|centre]]
All of these look very similar to the analytical solution, however if we observe the case in the top right we can see that there are issues with having **a few sources positioned close to the edge of the body**.
The graphs below show the tangential surface velocity $V_{t}$:
![[Pasted image 20250125164103.png|centre]]
Note again how they all look good, except for the one in  the top right (which we had issues with before).
These graphs indicate that:
- If we have a small number of sources then their location impacts the accuracy of the results.
- However if we increase the number of sources then the model becomes more accurate
Again we can see this with the graphs of surface pressures:![[Pasted image 20250125164336.png]]
We can also observe the radial surface velocity - for the analytical solution we get that there is zero radial velocity, however with the numerical solutions this isn't necessarily the case:
![[Pasted image 20250125164613.png|centre]]
Here we can see that all of the control points have the correct velocities (as we have locked them to zero) but we cant control the velocity between the control points. Note how the bottom left graph shows the best solution with the error dropping to 1.5x10^-3 in error.
**Lets now observe what happens if we place the sources in a circular pattern with a reduced radius:**
![[Pasted image 20250125165041.png|centre]]
Here it is much more obvious that the position plays a much greater role in the quality of the model, the top right example is awful, with streamlines passing straight through the body.
Again looking at the tangential velocity:
![[Pasted image 20250125165301.png|centre]]
And the pressure:
![[Pasted image 20250125165325.png|centre]]
We see a similar pattern.
And again looking at the radial velcocity:
![[Pasted image 20250125165400.png|centre]]
Shows that increasing the number of points whilst they are further away from the body of the surface massively increases accuracy.
### Solution for a Symmetric Aerofoil - Centreline
Let's now look at the solution for a symmetric aerofoil when the sources are along the centreline:
![[Pasted image 20250125165647.png|centre]]
Using the control points as illustrated in the diagram above (i.e. where they are directly above the sources which are at the centre of each "panel") we get the poor plot shown below:
![[Pasted image 20250125165659.png|centre]]
However if we move the foremost and rearmost control points closer to the leading and trailing edges respectively then we get a much better plot which aligns with the analytical solution.
### Panel Methods
The 2D generalised models considered thus far have many similarities to 2D panel methods. This is particularly the case if the location of the singularities and control points is linked to modelling the geometry with panels.
However most methods referred to in literature as 2D panel methods don't use individual discrete point elements. Instead distributed elements are used where the sources, doublets, and vortices are distributed 