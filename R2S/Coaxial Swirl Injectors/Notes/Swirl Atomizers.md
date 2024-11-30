### Pros and Cons
Swirl atomisers are commonly used because they have the following **advantages** compared to other nozzles:
1) Relatively simple design
2) High reliability
3) Good spraying quality
4) Small power required
However they do have the following **disadvantages**:
1) Limited use for atomisation of very viscous fuels
2) Small range of regulation, where regulation is understood as the ratio of the maximum and minimum flow rates
### Characteristic Parametrisation
A schematic diagram of the simplest swirl atomiser is shown below:
![[Pasted image 20241127140224.png|centre|400]]![[Pasted image 20241129143310.png|centre]]
The characteristic parameters of swirl atomisers are represented by the geometric constant $K$:
$$K=\frac{Rr_{0}}{ir_{p}^{2}}=\frac{2Rd_{0}}{id_{p^2}}=\frac{\pi Rr_{0}}{iA_{p}}=\frac{2\pi Rd_{0}}{4iA_{p}}$$
Note that:
- $R$ is the swirl radius
- $r_{p}$ and $d_{p}$ are the radius and diameter of the tangential orifice, respectively
- $r_{0}$ and $d_{0}$ are the radius and diameter of the discharge orifice, respectively
- $i$ is the number of tangent inlet orifices
- $A_{p}$ is the cross section of the tangential inlet orifice with an arbitrary transverse shape
If the tangential inlet orifices are inclined to the swirl chamber axis at angle $\Theta$ then this equation assumes the form:
$$K=\frac{Rr_{0}}{ir_{p}^{2}}\sin\Theta=...$$
### Design (Of a Simplex Atomiser)
#### Volumetric and Mass Flow Rates
We can calculate the volume and mass flow rates using the following equations:
$$Q=\frac{1}{\sqrt{\frac{K^{2}}{1-\epsilon}+ \frac{1}{\epsilon^{2}}}}\cdot\pi r_{0}^{2}\sqrt{\frac{2P_{t}}{\rho}}=\boxed{\mu A_{0}\sqrt{\frac{2\Delta P}{\rho}}}$$
Where $\mu$ is the discharge coefficient, which depends on two quantities: the geometric constant $K$ and the efficiency of filling the discharge orifice $\epsilon$:
$$\mu=\frac{1}{\sqrt{\frac{K^{2}}{1-\epsilon}+ \frac{1}{\epsilon^{2}}}}$$
$\epsilon$ can be calculated using:
$$\epsilon=\frac{A}{A_{0}}=\frac{\pi(r_{0}^{2}-r_{2}^{2})}{\pi r_{0}^{2}}=1-\left(\frac{r_{r}}{r_{0}}\right)^{2}$$
Where $A_{0}=\pi r_{0}^{2}$ which is the area of the discharge orifice, and $r_{r}$ is the gas core radius.
**************
We can therefore calculate the volumetric flow rate based on the change in pressure across the atomiser, and the geometric properties of it.

We can calculate the mass flow rate by simply multiplying by density:
$$G=\rho Q=\mu A_{0}\sqrt{2\rho\Delta P}$$

#### Simple Design Method

> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=11&selection=112,20,130,38&color=yellow|DesignOfSwirlAtomiser, p.11]]
> > The aim of the design is to determine the dimensions of a simplex swirl atomizer for the following data: $Q$ or $G$, $\alpha$ , $\Delta P$ , $\rho$ , and $v$. First one calculates the basic dimensions incorporated in geometric constant K and then the other dimensions (Fig. 5-13).
> 

Firstly, for a given angle $\alpha$ we determine the geometric constant $K$ using the following diagram (curve 2):
![[Pasted image 20241129142750.png|centre]]
We then determine the discharge coefficient $\mu$ for this value of $K$.
From these we can calculate the discharge orifice diameter:
$$d_{0}=\sqrt{\frac{4G}{\pi\mu\sqrt{2\rho P_{t}}}}$$
The geometric constraint now contains three unknown quantities: $R$, $i$, and $d_{p}$:
$$K=\frac{2Rd_{0}}{id_{p}^{2}}$$
![[Pasted image 20241129144836.png|centre]]

*Note what these unknown quantities are, $R$ and $d_{p}$ are shown in the diagram above, whilst $i$ is the number of inlets.*
**We will need to assume two of these.** 
> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=12&selection=14,32,24,4&color=yellow|DesignOfSwirlAtomiser, p.12]]
> >  It is most convenient to assume the number of orifices and radius of swirling. Most commonly, $i$ = 2 to 4 and $R$ = $(2-5)r_{0}$ are used.  

Therefore we can calculate the diameter of the tangential inlet orifices to be:
$$d_{p}=\sqrt{\frac{2Rd_{0}}{iK}}$$
**We can now begin the second phase of calculations.**
> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=12&selection=57,0,62,6&color=yellow|DesignOfSwirlAtomiser, p.12]]
> > The second phase of calculations refers to the assessment of the viscosity effect

The Reynolds number at the inlet to the atomisers is:
$$Re=\frac{v_{p}d}{\nu}$$
Where $d$ is the diameter of the equivalent orifice, which can be determined as:
$$d=\sqrt{i}d_{p}$$
Velocity $v_{p}$ is given by:
$$v_{p}=\frac{4G}{\rho i \pi d_{p}^{2}}$$
And obviously $\nu$ is the viscosity of the fluid being swirled.

We can find the friction coefficient from:
$$\lg \lambda =\frac{25.8}{(\lg Re)^{2.58}}-2$$
Which has been established as a result of extensive investigations of atomisers in the range $Re=10^{3} - 10^{5}$.

> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=13&selection=25,0,52,9&color=yellow|DesignOfSwirlAtomiser, p.13]]
> > Considering the selection of the value of radius R , remember that R should be small and simultaneously the area of the inlet orifices should be small in order to overcome the viscosity barrier. The higher K is, i.e., the larger angle a is required, the smaller radius R should be. Also, the smaller the flow rate and the higher the liquid viscosity, the smaller radius R should be

**We can now begin the third phase of calculations.**
> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=14&selection=2,0,7,38&color=yellow|DesignOfSwirlAtomiser, p.14]]
> > The third phase o f calculations concerns the determination of the remaining dimensions of the atomizer (Fig. 5-13)

The diameter of the swirl chamber $D_{s}$ is:
$$D_{s}=2R+d_{p}'$$
The length of the swirl chamber $l_{s}$ should be larger than the length of the inlet - which itself should have proper length so that jets entering the swirl chamber are not deflected from the tangential direction - it is recommended that this length is in the range:
$$l_{s}=(1.5 \text{ to } 3.0)d_{p}'$$
> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=14&selection=61,0,71,1&color=yellow|DesignOfSwirlAtomiser, p.14]]
> > The angle of the transient cone most commonly equals $\beta$ = 60-120°; smaller angles $\beta$  cause an increase of the discharge coefficient p and decrease of angle $\alpha$ 
> 

> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=14&selection=44,0,60,0&color=yellow|DesignOfSwirlAtomiser, p.14]]
> > The discharge orifice should not be too long in order not to decrease an gle a. For K$_\lambda$  < 4-5 we recommend $l$ = (0.5-1.0)$d_0$; for K$_\lambda$ > 4 -5 , $l$ = (0.25- 0.5)$d_0$.

### Specifics on Two-Nozzle Atomizers
In two-nozzle atomizers, liquid flow through both systems proceeds independently:
![[Pasted image 20241130163405.png|centre]]
A two-orifice atomizer consists of two simplex atomizers connected in parallel. (**Also sometimes called co-axial swirl injectors**)

> [!PDF|yellow] [[DesignOfSwirlAtomiser.pdf#page=19&selection=35,6,37,79&color=yellow|DesignOfSwirlAtomiser, p.19]]
> > The design of a two-nozzle atomizer consists of separate calculations for two systems following the method described for simplex atomizers. The relative position of the two nozzles (discharge orifices) affects the shape of the spray.
> 
