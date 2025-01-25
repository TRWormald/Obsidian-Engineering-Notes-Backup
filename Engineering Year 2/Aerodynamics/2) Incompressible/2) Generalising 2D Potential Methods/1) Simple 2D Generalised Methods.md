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
