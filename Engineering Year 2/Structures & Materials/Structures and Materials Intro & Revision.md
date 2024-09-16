## Important Axial Definitions
### Global Axes
We use the uppercase roman letters (X,Y,Z) to describe the *global coordinate system* (global CS)
This is also sometimes called the *structural coordinate system*.
The origin and orientation of the global CS are somewhat arbitrary.
![[Screenshot 2024-09-16 160707.png|center]]
In the diagram above we have made the $Z$ the longitudinal (span-wise) direction, so that any cross sectional plane will be parallel to the $XY$ plane.
We will also use the terms 'horizontal' and 'vertical' for the $X$ and $Y$ directions respectively.
### Centroid-based Axes
This is a local coordinate system which is defined with the origin **at the centroid** of the cross section, but parallel to the global CS.
We will use the lowercase roman letters ($x,y,z$) for this coordinate system.
![[Screenshot 2024-09-16 161101.png|center]]
### Rotations and Moments
Rotations and moments are defined with respect to centroid-based axes ($x,y,z$) or global axes ($X,Y,Z$) by application of the **right hand rule** about each orthogonal axis.
Moments are vectoral quantities represented by arrows with double arrowheads.
To find the positive direction of rotation, apply the RHR about each vector.
![[Screenshot 2024-09-16 161356.png|center]]
### Loading Axis (angle $\theta_{L}$)
We will be considering loads along or about any arbitrary loading axis, oriented in the ($x,y$) plane by the angle $\theta_{L}$.
- Shear loads are applied along the loading axis
- Moments are applied about the loading axis
Moment vectors can be operated on just like force vectors:
- Resultant can be decomposed into orthogonal components and vice versa.
![[Screenshot 2024-09-16 161656.png|centre]]
### Neutral Axis (angle $\alpha$)
We define the **neutral axis** as the axis along which bending stresses are **zero** (and change sign above/below the axis).
We name $\alpha$ the angle of this neutral axis with respect to the centroid-based coordinate system ($x,y$)
The orientation of the neutral axis depends on a combination of geometry **and** loading conditions, and therefore it is **not** and intrinsic property of the cross-section.
![[Screenshot 2024-09-16 163857.png|centre]]
### Principal Axes (1,2) (angle $\theta_{P}$)
We use indicies (1,2) to indicate the **principal axes**, i.e. axes about which the [[Second Moment of Area]] is maximum or minimum.
The principal aces are rotated by an angle we call $\theta_{P}$ and:
- Have their origin at the centroid of the section
- Coincide with any axes of symmetry that the section may have.
![[Pasted image 20240916162250.png|centre]]
## Cross-Section Properties
### Cross-sectional Area
The area of a cross-section can be written as an **area integral**:
$$A=\int_{A}dA$$
For compound cross-sections we split the section into geometrical primitives indexed by the subscripts $i=1...n$ and write the integral as a summation:
$$A=\sum\limits^{n}_{i=1}A_{i}$$
### First Moments of Area
The first moments of area are used twice in the course: when finding the centroid of a section and when deriving shear stresses.
**Definition**:
The first moments of area about an arbitrary coordinate system ($X,Y$) are:
$$Q_{XX}=\int_{A}YdA$$
$$Q_{YY}=\int_{A}XdA$$
For compound sections we again re-write these as summations:
$$Q_{XX}=\sum\limits^{n}_{i=1}\bar{Y}_{i}A_{i}$$
$$Q_{YY}=\sum\limits^{n}_{i=1}\bar{X}_{i}A_{i}$$
Where $\bar{X}_{i}$ and $\bar{Y}_{i}$ are the coordinates of the centroid of each component making the compound section.
