Consider the simply supported beam in the following diagram:
![[Pasted image 20240226114710.png#center]]
The methodology for finding its shear force and bending moment diagrams is as follows:
- Calculate the reactions $R_A$ and $R_B$ using equations of equilibrium
- Make a cut at x, and draw the shear force F and bending moment M, using positive directions.
- Solve for F, using force equilibrium
- Solve for M, using moment equilibrium
- Make two cuts (one where x<L/2 and one where x>L/2)
- Plot the [F] and [M] diagrams
\
Using this method we get that before the load the force is equal to $\frac{P}{2}$ and the bending moment is equal to $-\frac{Px}{4}$. Making a cut x<L/2 gives us the maximum bending moment of $-\frac{PL}{4}$, and making a cut after the load gives us a force of $-\frac{P}{2}$ and a bending moment of $-\frac{LP}{2}+\frac{Px}{2}$ (Note that all of these values were calculated using [[The Sign Convention for Shear Force and Bending Moment in Beams]]). All of this together gives us the shear force and bending moment diagrams as follows:
![[Pasted image 20240226120148.png#center]]
\
It should also be noted that shear force and bending moment diagrams can be superimposed on each other to get a solution to a problem with multiple loads, much like with ODEs. So, it may be easier to solve each load separately and then combine them all at the end.
\
By taking the moments about a small section of the beam:
![[Pasted image 20240226172458.png#center]]
We can calculate that $\frac{dM}{dx}=-F$, or in other words:
$$M(x)=-\int F(x)\cdot dx$$
So the moment diagram can be found by integrating the force diagram and negating it. (Bending Moment diagram = - Area under Shear Force Diagram)
Take for example:
![[Pasted image 20240226173522.png#center]]
If the force is constant and negative (as it is at the start) then on the moment diagram there must be a linear positive bending moment. This logic can be applied to the whole of the diagram to solve it.

##### How to deal with Distributed Loads
__Uniformly Distributed Loads__
The easiest type of distributed load to deal with are uniformly distributed loads. While finding a shear force diagram it is best to start a local coordinate axis at the beginning of the distributed load and hence the force applied up until the cut will be equal to whatever the force was before the load plus q (N/m) times by x*.
In the case of moment calculations the force can be considered to act through the midpoint of the area over which the load is applied.
![[Pasted image 20240226175055.png#center]]
__Triangular Loads__
You can deal with triangular loads in the same way, however you have to use the formula $\frac{q\cdot x^*}{2}$. Similarly for moments the force can be considered to act at a point two thirds along the length of the applied load.
![[Pasted image 20240226175115.png#center]]
__General Distributed Loads__
For a generally distributed load the force applied is equal to:
$$F=\int q(x)\cdot dx$$
And is applied through:
$$\bar{x}=\frac{\int q(x)~x\cdot dx}{\int q(x)\cdot dx}$$
![[Pasted image 20240226175205.png#center]]

#####
Now that we have the Bending Moment diagram we can qualitatively draw the deflected shape of the beam:
![[Pasted image 20240226175406.png#center]]
\
When doing this remember that:
![[Pasted image 20240226175435.png]]
Whilst also consulting the bending moment diagram to determine whether the beam is sagging or hogging (See [[The Sign Convention for Shear Force and Bending Moment in Beams]])

##### Gerber's Beam (Pinned Beams)
To solve problems involving pinned beams split the beam at the point at which it is pinned and then solve each section individually (using one to then solve the other)
\
![[Pasted image 20240226175745.png#center]]
\
In the above example we first solve the right part for $F_{pin}$ and then use it to solve the left part.