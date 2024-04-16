### Thermal System
#### Intro to Concepts
All materials have a [[Thermal Conductivity]] which defines the rate at which heat will pass through the material.
\
Heat conduction will always be driven by a temperature gradient - heat energy cannot move against a temperature gradient. Heat conduction rate is a function of:
- Temperature Gradient
- Distance of Conduction
- Surface area of plane normal to the direction of heat transfer
- Thermal Conductivity
Such that:
$$\dot{Q}=\frac{k\cdot A\cdot\Delta T}{\Delta x}$$
We will assume that properties are constants for a given material sample, so the only thing that can affect $\dot{Q}$ is $\Delta T$.
### Thermal System
As all of our properties are constant we can combine them to get a new property, the thermal resistance $R_{t}$:
$$R_{t}=\frac{\Delta x}{k\cdot A}$$
This equation comes from the fact that:
- Increased $\Delta x$ results in a reduction in $\dot{Q}$
- Increased $A$ results in an increase in $\dot{Q}$
- Increased $k$ results in an increase in $\dot{Q}$
And ultimately we are attempting to get the equation to look as similar to $I=\frac{V}{R}$ as possible.
So:
$$\dot{Q}=\frac{\Delta T}{R_{t}}$$
### Electrical Equivalence
If we consider the following equivalent circuit:
![[Pasted image 20240416105651.png|center|300]]
We can see that:
- There is a potential difference between $V_{1}$ and $V_{2}$ of $\Delta V=V_{1}-V_{2}$.
- The current flow is always driven by a potential difference.
- Electrical Resistance limits current flow.
\
It shouldn't be too hard to see the equivalence:
$$I= \frac{{\Delta V}}{R_{e}}\Leftarrow\Rightarrow\dot{Q}=\frac{{\Delta T}}{R_{t}}$$
Hence we can create a table comparing the two systems:
![[Pasted image 20240416110052.png|center]]
### Using Series Circuits to model Complex Thermal Systems
What happens if we have two materials with different thermal conductivities in series?