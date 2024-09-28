### Stress-Resultant Torque $M_{z}$
The shear flow field always follows the contour of a section, this field represents stress-resultant forces acting over the section.
Taking an arbitrary point as the origin of the $X-Y$ plane, these forces are seen to generate a stress-resultant torque $M_{z}$.
We define a new function, $r_{(s)}$ representing the orthogonal distance between vector $q_{(s)}$ and this arbitrary reference point.
![[Screenshot 2024-09-28 130945.png|centre|300]]
The total torque is then:
$$M_{z}=\int_{s}q_{(s)}r_{(s)}~ds$$
### The Local Moment Arm
The local moment arm function $r_{(s)}$ can be positive or negative, following the right-hand rule about axis $Z$.
The function depends on the chosen reference point, i.e. the origin of the $X-Y$ plane.
- A convenient reference point must be chosen for each particular case
- If the section contains a radius then the centre of this radius must be taken as the reference point.

### Shear Centre - Point of Zero Stress-Resultant Torque
There is a point within the $X-Y$ plane where the stress-resultant torque for a section will always be zero, for any combination of orthogonal shear forces $S_{X}$ and $S_{Y}$.
This point is called the **shear centre**, and is an intrinsic property of the section.
The coordinate system with origin at the shear centre is $(\hat{X},\hat{Y},\hat{Z})$ and the new moment arm function is $\hat{r}_{(s)}$, and the stress-resultant torque becomes:
$$^{q_{(s)}}M_{\hat{Z}}=\int_{s}q_{(s)}\hat{r}_{(s)}~ds=0$$
### External Torque about $\hat{Z}$
If two orthogonal shear forces $S_{X}$ and $S_{Y}$ are applied along lines that do not cross the shear centre, then the section will not only deflect but also twist.
This is because the shear forces will generate a torque about $\hat{Z}$, proportional to the orthogonal distances between the loading axes and the shear centre, $e_{x}$ and $e_{y}$:
$$M_{\hat{Z}}=S_{x}e_{Y}-S_{Y}e_{X}$$
![[Screenshot 2024-09-28 133813.png|centre|250]]
### External Torque that cancels out $M_{Z}$
To find the shear centre coordinates we find the external torque about the shear centre, $M_{\hat{Z}}$, required to cancel out the stress-resultant torque about the loading point, $M_{Z}$:
$$M_\hat{Z}=-M_{Z}$$
This is finally written as:
$$\underbrace{S_{Y}e_{X}-S_{X}e_{Y}}_{-M_{\hat{Z}}}=\underbrace{\int_{s}q_{(s)}r_{(s)}~ds}_{M_Z}$$
### Torsion Centre
The shear centre also provides a favourable axis for torsion.
Torsion about axis $\hat{Z}$ that passes through the shear centre will generate minimum stresses over the section for any given applied torque, hence providing a configuration of lowest potential energy.
Therefore the shear centre is also sometimes called the torsion centre.