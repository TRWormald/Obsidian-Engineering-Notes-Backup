![[Pasted image 20240920105202.png|centre]]
The above image shows an arbitrary thin-walled section subjected to a transverse (downward) shear force. The resultant shear stresses are parallel to the wall, as if they were "flowing" along the cross-section.

### Coordinates in Open Thin-Walled Sections
When analysing thin-walled sections we define two new coordinates:
- The arc length "$s$", tangent to the local mid-surface of the section.
- The through-thickness coordinate $n$, normal to the local mid-surface of the section.
These can be seen in the diagram below:
![[Pasted image 20240920105504.png|centre]]
### Solving the Problem
#### Step One
Is to write our section coordinates as a function of $s$. This is called 'section parametrisation' and it is often the trickiest bit.
1) Choose a convenient origin for (X,Y), considering symmetries and any radii
2) Define the origin of "s" at a free edge, progressing CCW if possible
3) Split the section into straight lines and circular arcs, $i=1,..., n$
4) Use A-Level trigonometry and algebra to derive functions $^{i}X_{(s)}$, $^{i}Y_{(s)}$, $^{i}t_{(s)}$ (variable thickness) for each wall $i$, resetting the arc-length $s$ at the start of each wall.
##### Examples
![[Pasted image 20240920110018.png]]
![[Pasted image 20240920110026.png]]
We complete a similar process for Radii, except we use $\phi$ to denote angle:
![[Pasted image 20240920110124.png]]
And we integrate counter clockwise due to our sign convention. 
#### Step Two
Thin-walled sections must be integrated using line integrals. The arc-length coordinate $s$ defines a continuous path along the section, starting from a free edge.
The wall thickness may be variable, so we define it as a function of the arc-length $s$, writing $t_{(s)}$.
The area integral then becomes:
$$A=\int_{A}dA=\int_{s}t_{(s)}~ds$$
Arcs of Radius R are integrated in terms of the angle $\phi$ instead and:
$$\boxed{ds=R~d\phi}$$
Hence:
$$\boxed{\underbrace{A=\int_{s}t_{(s)}~ds}_{\text{For Lines}}~~~~~~~~~~~~~~~~~\underbrace{A=\int_{\phi}t_{(\phi)}(R~d\phi)}_{\text{For Arcs}}}$$
From this we can generate the first moments of area calculations, along with the centroid-based coordinates, and the second moments of area equations:

**First Moments of Area:**
For lines we get:
$$\begin{align*}
Q_{XX}&= \int_{s}Y_{(s)}t_{(s)}~ds\\
Q_{YY}&= \int_{s}X_{(s)}t_{(s)}~ds
\end{align*}$$
While for arcs:
$$\begin{align*}
Q_{XX}&= \int_{\phi}Y_{(\phi)}t_{(\phi)}~(R~d\phi)\\
Q_{YY}&= \int_{\phi}X_{(\phi)}t_{(\phi)}~(R~d\phi)
\end{align*}$$
**Centroid-based Coordinates:**
As before we know that:
$$\bar{X}=\frac{Q_{YY}}{A} ~~~~~~~~\text{and}~~~~~~~~\bar{Y}=\frac{Q_{XX}}{A}$$
Then, for lines:
$$\begin{align*}
x_{(s)}&= X_{(s)}-\bar{X}\\
y_{(s)}&=Y_{(s)}-\bar{Y} 
\end{align*}$$
And for arcs:
$$\begin{align*}
x_{(\phi)}&= X_{(\phi)}-\bar{X}\\
y_{(\phi)}&=Y_{(\phi)}-\bar{Y} 
\end{align*}$$
**Second Moments of Area**
Simply, for lines:
$$I_{xx}=\int_{s} {y_{(s)}}^{2}~t_{(s)}~ds$$

$$I_{yy}=\int_{s} {x_{(s)}}^{2}~t_{(s)}~ds$$

$$I_{xx}=\int_{s} x_{(s)}~y_{(s)}~t_{(s)}~ds$$
And for arcs:

$$I_{xx}=\int_{\phi} {y_{(\phi)}}^{2}~t_{(\phi)}~(R~d\phi)$$

$$I_{yy}=\int_{\phi} {x_{(\phi)}}^{2}~t_{(\phi)}~(R~d\phi)$$

$$I_{xx}=\int_{\phi} x_{(\phi)}~y_{(\phi)}~t_{(\phi)}~(R~d\phi)$$
