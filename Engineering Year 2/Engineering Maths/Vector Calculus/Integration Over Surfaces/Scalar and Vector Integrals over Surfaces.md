**Motivation:**
Consider a steady fluid motion (e.g. airflow); what is the flux (volume of fluid per unit time) flowing through a given surface? E.g. what is the air intake rate into the orifice of a jet engine? How much blood flows through a given membrane etc?

Consider fluid flowing across a surface $S$ with velocity $\mathbf{v}$. In unit time a small piece of area $\Delta A$ moves to $\Delta A'$.
![[Pasted image 20241031172520.png]]
The volume of the fluid flowing through $\Delta A$ in unit time is given by the volume of the column in the above figure.
$$\begin{align*}
\text{area}\times\text{flow/unit time}&= \Delta A|\mathbf{v}|\cos\theta\\
&= \Delta A(\mathbf{v}\cdot\mathbf{\hat{n}})
\end{align*}$$
Where $\mathbf{\hat{n}}$ is the normal vector to the surface $S$ at this point. We need the component of the vector field $\mathbf{v}(\mathbf{r})$ that is normal to the surface.
Summing up all the small contributions from $\Delta A$'s across the surface $S$, the integral we require is:
#### The Flux Integral
The flux integral of a vector field through a surface $S$ is:
$$\int\int_{S}\mathbf{v}\cdot \mathbf{dA}:=\int\int_{S}\mathbf{v\cdot \hat{n}}~dA$$
Where $dA$ is an infinitesimal piece of area of the surface and $\mathbf{\hat{n}}$ is the unit normal.
##### Applications of the Flux Integral
In fluid dynamics the flow through a surface $S$ is given by:
$$\Phi=\int\int_{S}\mathbf{v}\cdot\mathbf{\hat{n}}~dA$$
In thermodynamics the heat flow through a surface $S$ is given by:
$$\Phi=\int\int_{S}\mathbf{H}\cdot\mathbf{\hat{n}} ~dA$$
##### Example 6.1
![[Pasted image 20241031181310.png|centre]]
### The Scalar Surface Integral
This is the integral over a surface of scalar field $f$:
$$\int\int_{S}f~dA:=\int\int_{S}f|\mathbf{dA}|$$
Examples include mass, surface area, and moment of inertia of plates, shells, etc.
![[Pasted image 20241103154917.png|centre]]
##### Example 6.2
![[Pasted image 20241103154941.png]]
