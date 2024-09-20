Stiffness-limited design is constrained by the elastic **deflection** of the component, which must be restricted to some **acceptable** value (a constraint).
We typically consider three different types of scenarios: uniaxial tension (a), beam bending (c), and panel bending (b).
![[Pasted image 20240321100442.png|center]]
Usually we want to minimise the mass or the cost of the component (the [[Constraints vs Objectives|objective]]). Both of these need equations to describe them. Typically constraint and objective equations will interact with each other (for example if the objective is to minimise mass but you have a constraint based on loading and a more massive beam will likely have greater load bearing capacity). Dealing with these *coupled variables* follows a regular pattern:
1) Define an objective and constraint equations
2) Identify the coupled free variable (i.e. can change and appears in both equations)
3) Solve the constraint equation for the free variable
4) Substitute into the objective to eliminate the free variable
5) Separate variables to identify the material properties ([[Selecting for Physical Properties#The Material Index (M)|The Material Index]])
\
The material index may appear in the form:
$$M=\frac{P_{y}^{\alpha}}{P_{x}}~~~~~~\text{or}~~~~~~M=\frac{P_{x}}{P_{y}^{\alpha}}$$
The latter being the reciprocal of the first. When placing a line on a selection diagram with these axes the selection line gradient is equal to $\frac{1}{\alpha}$.  
#### The Impact of Shape on Stiffness (Shape Factor)
The deflection of a beam is a function of the shape as reflected in the [[Second Moment of Area]], which gets bigger if more material is far from the neutral axis. Tubes and I-beams can be lighter than solid sections for the same stiffness constraint.
We can describe this via a *shape factor*:
$$\Phi^{e}_{B}=\frac{I}{I_{square}}=\frac{12I}{A^{2}}$$
Where $I_{square}$ is the second moment of area of a solid square beam of the same area as the shaped beam. The superscript on the $\Phi$ denotes elastic and the subscript denotes bending.
As a result we can represent the fact that we are using a tube or I-beam by multiplying the young's modulus by the shape factor.
Note that if we have $E^\frac{1}{2}$ in an equation and we apply a shape factor, we end up with $(\Phi E)^\frac{1}{2}$ as the shape factor is a component of the [[Young's Modulus]].