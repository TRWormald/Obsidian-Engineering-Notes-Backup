### Lifting Line Theory for General Lift Distributions
In the general case circulation distribution can be modelled using a Fourier Sine Series:
$$\boxed{\Gamma(\theta)=4sV_{\infty}\sum\limits_{n=1}^{N}A_{n}\sin n\theta}$$
Where $y=-s\cos\theta$.
Note that for the elliptic case only the first term $A_1$ is non zero:
$$\Gamma(\theta)=\Gamma_{0}\sin\theta$$
Where:
$$A_{1}=\frac{\Gamma_{0}}{4sV_{\infty}}=\alpha_{i}$$
The corresponding induced incidence distribution is:
$$\alpha_{i}(\theta_{0})=\frac{-w(\theta_{0})}{V_{\infty}}=\sum\limits_{n=1}^{N}nA_{n}\frac{\sin n\theta_{0}}{\sin\theta_{0}}$$
So lift depends on $A_1$ only:
$$C_{L}=A_{1}\pi~AR$$
And induced drag becomes:
$$C_{D_{i}}=\frac{C_{L}^{2}}{\pi~AR}[1+\delta]$$
For an untwisted wing the lift coefficient is given by:
$$C_{L}=a(\alpha-\alpha_{L=0})$$
Where $\alpha_{L=0}$ is the zero lift incidence of the wing and the 3D lift curve slope is given by:
$$a=\frac{a_{0}}{1+\frac{a_{0}}{\pi~AR}(1+\tau)}$$
### Drag and Lift Slope Distributions
![[Pasted image 20250408160158.png|centre]]![[Pasted image 20250408160226.png|centre]]
![[Pasted image 20250408160238.png|centre]]
### Effect of AR on Lift Distribution
![[Pasted image 20250408160311.png|centre]]
For a rectangular wing, $\lambda=1$ and shape is the same as plotting lift coefficient since the chord is the same for all sections of the wing. 
### Effect of $\lambda$ on Lift Distribution
![[Pasted image 20250408160550.png|centre]]
We want a **high AR** wing for **low drag**.
### Wing Planforms
Consider untwisted wings with the same aerofoil section which have the same span and are:
- Rectangular
- Elliptical
- Tapered
Then the chord and downwash vary across the span and hence the effective incidence and lift vary across the span.
![[Pasted image 20250408160751.png]]In the image above we see the various ways in which the wings stall.
Planform section is based on compromises:
- Elliptical is favoured for induced drag considerations, but it is too expensive to produce.
- Rectangular would be the cheapest to produce, since all aerofoil sections are the same, and thus all ribs are identical and can be made from the same pattern (it also has a favourable stall pattern)
	- However then the wings end up heavier than necessary in the outboard region.
- The tapered wing can be designed to have induced drag levels close to that of the elliptical wing. However, stall pattern is not favourable. This can be overcome using twist, but this can increase parasitic drag.
### Wake Modelling
To get the correct lift from a 3D panel method we need to model the wake in a physically responsible way. This has two aspects:
1) The way the wake is shed from the trailing edge
2) The way the wake develops downstream of the wing
#### Wake Modelling - TE
Applying the Kutta condition as equal pressure top and bottom of the aerofoil at the trailing edge implies an equal velocity magnitude, but not direction. This ensures that the wake leaves the trailing edge smoothly.
This does allow for a jump in velocity direction in the wake, which is more physically correct for wing flows. (remember the 2D Kutta implies either zero velocity or identical velocities at the trailing edge, but this is the 2D manifestation of equal pressure.)
### Wake Modelling Downstream
The other issue is that the angle the wake leaves the trailing edge of the wing is linked to the geometry, but far downstream the wake should be aligned with the free stream. Thus, a fixed flat wake will not satisfy both requirements.
Despite this issue, planar wakes are often used. Alternatively, a fixed curved wake shape is prescribed.
![[Pasted image 20250408164157.png|centre]]
Prescribed wakes lead to quick calculations.
A more physically correct approach used for steady flows is to allow the wake shape to evolve (“relax”) either from an original prescribed wake or over time from the trailing edge until there is no pressure difference across the wake. This allows the wake edges to roll up and the downstream shape to evolve.
### The Vortex Lattice Method
The VLM combines two of the methods we have already met to provide a quick method that is used in the early stages of aircraft design. 
These are the Lifting Line Method, and the Lumped Vortex Method.
![[Pasted image 20250408170222.png|centre]]
![[Pasted image 20250408170309.png|centre]]
##### Vortex Lattice For Rectangular Uncambered Wings
Combining these ideas for a thin, rectangular, uncambered (or symmetric wing):
- Divide the wing into a finite number of panels and put a horseshoe vortex and control point on each panel.
	- Bound vortex at 0.25c
	- Control point at 0.75c
When the wing is fully covered it should look like this:
![[Pasted image 20250408170506.png]]
And then this is a problem which can be solved very quickly numerically.
##### Vortex Lattice For Swept Uncambered Wings
We can even extend this method to uncambered swept wings, but we may need to be careful as a control point could be in line with a bound vortex.
![[Pasted image 20250408170624.png|centre]]
![[Pasted image 20250408170749.png|centre]]
#### Implementing the Vortex Lattice Method
1) Represent the wing as a flat plate
2) Split the plate into cells or panels
3) Give each panel a horseshoe vortex of strength $\Gamma_{j}$
4) Use this to calculate the normal induced velocity, caused by vortex $j$ at control point $i$ using the **Biot Savart Law** to give:
$$a_{i,j}\Gamma_{j}$$
5) Apply no normal flow b.c. and as with the 2D panel method this results in a matrix equation of the form:
![[Pasted image 20250408171019.png|centre]]
This can be solved for each vortex strength in a similar way to the 2D panel methods seen before.
### How Can We Make This Work For Cambered Wings?
The method that we have just defined would not work for cambered wings, the image below illustrates why that is the case:
![[Pasted image 20250408180537.png|centre]]
Up to this point we have used the discrete horseshoe vortex case, which could be visualised in two different ways:
![[Pasted image 20250408180651.png|centre]]
We could think about the model in a third way however, representing the wing as a series of ring vortex elements, with only a single trailing vortex:
![[Pasted image 20250408180754.png|centre]]
This vortex ring representation can then be extended to cambered wings:
![[Pasted image 20250408180828.png|centre]]
The wake shown here leaves the trailing edge smoothly, but far downstream it really should be aligned with the free stream direction, leading to inaccuracy.
Ideally the wake itself should be represented in more detail so that its behaviour is closer to the real flow (this is achieved via wake relaxation, an iterative process see earlier).
- It should leave the trailing at the mid point of the trailing edge angle
- It should be aligned with the free stream in the far field
**PROS AND CONS:**
- Quicker and simpler than full 3D panel method. 
- Easy to do multi-element aerofoil sections (i.e. Flaps) 
- But has similar limitations to thin aerofoil theory – thin shapes – not very good at stagnation 
-  Also limitations of a potential method
	-  Can extend applicability by using compressibility correction and coupling to a boundary layer code 
	- Can also be corrected using experimental data 
-  These problems are not too important if the vehicle to be analysed is an aircraft dominated (aerodynamically) by the wing.
#### Aeroelastic Analysis
- Perhaps biggest advantage/widest application is for aeroelastic work: 
	- Structural representation of a wing is often as flat panels 
	- can be coupled directly to vortex lattice method
	- Fast solution of linear aerodynamic equations
	- Available in commercial FE solution packages such as NASTRAN and ZAERO
## Revision
![[Pasted image 20250408181117.png|centre]]
