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
$$M=$$