### Balance vs Stability
> In steady non-accelerating flight the aircraft is in equilibrium and the forces and moments acting on the airframe are in balance and sum to zero. This initial condition is usually referred to as **trimmed equilibrium**.

The **static stability** of an aircraft is commonly interpreted to describe its tendency to converge on the initial equilibrium condition following a small disturbance from trim. **Dynamic stability** on the other hand, describes the transient motion involved in the process of recovering equilibrium following the disturbance.
### Longitudinal Balance
The simplest version of the longitudinal model (which assumes axial forces - thrust and drag - are in balance):
- We need enough lift to support the aircraft in the trimmed condition
- We need to distribute the aerodynamic forces such that the overall pitching moment is zero
The challenge is that:
- We need to arrange for both of these to be achieved simultaneously
- We need to establish and maintain this balance throughout the flight (through adjustments to throttle and elevator)
>We will be considering straight and level flight, however we could easily extend the analysis to include steady climbing flight, i.e. non-zero, constant flight path angle $\gamma$, and even turning flight.

Let's consider the free body diagram below (it's important to always draw one):
![[Pasted image 20251023150241.png|centre]]
It shows the aerodynamic forces from the two primary lifting surfaces (the wings and the tailplane) and the moments they generate, along with the weight originating from the centre of gravity. So we can construct equations such that:
$$\sum F_{vertical}=0$$
(Which ensures that the lift is equal to the weight)
And:
$$\sum M_{pitch}=0$$
(Which ensures that there is no change in the pitch of the aircraft)

For this configuration we need to have:
$$L_{W}=\bar{q} S C_{L_{W}}$$
$$L_{T }=\bar{q}S_{T}C_{L_{T}}$$
And we must retain:
$$(L_W +L_{T})=nW$$
The simple expression $L=\bar{q}Sa_{1}\alpha$ suggests that is speed (or $\bar{q}$) drops, we must simply increase the $\alpha$ to keep $L$ constant, but the two separate lift coefficients will be seen later to be separately related to $\alpha$ and we cannot simply alter the aircraft incidence and expect both to be altered by the same factor.
Therefore we must expect the relative values of $L_{W}$ and $L_{T}$ to change even if their sum remains at $nW$ (i.e. the need to trim/balance an aircraft for a given airspeed). This typically requires adjustment of both elevator (or stabiliser) and throttle.
#### Aerodynamic Centre
The centre of pressure for an aerofoil can move quite noticeably over the chord as the incidence varies. However, for a reasonable range of $\alpha$, we can find a point (the aerodynamic centre) on the aerofoil about which the moment generated will be constant. i.e:
$$\text{lift force}\times\text{arm about a.c.}=\text{constant}$$
From this we define the pitching moment $M_{0}$ that is taken to be constant for a range of $\alpha$ and is not altered when there is a $\Delta$Lift.
As the incidence changes, the value of lift changes and the centre of its action also changes (moment arm from c.p. to any chosen point). Clearly, for most values of $\alpha$ there must be a positive moment about the T.E. and a negative moment about the L.E.
What also becomes evident is that for some position near $\frac{1}{4}\bar{c}$ the pitching moment can be independent of $\alpha$ though not necessarily of zero value.
![[Pasted image 20251023152345.png|centre]]

### Lift Lumping
For ease of use we can "lump together" all lift contributions other than those due to the tail and thus refer to the primary lift as $L_{WFP}$ which means lift on the wing, fuselage, and pods (engine nacelles).
There would still be a moment that is independent of lift, but it would act about an aerodynamic centre which is not now at the wing quarter chord (due to the contribution of the fuselage).
### Simple Model for Longitudinal Balance
![[Pasted image 20251023153137.png|centre]]
**Assumptions:**
- The pitching moments due to thrust $F$ and all drag components $D$ are often considered to be quite small, compared with other moments.
- i.e. we initially ignore the pitching effect of $F$ and $D$
- The two lift forces act normal to the horizontal wind vector, which itself is aligned with $F$ and $D$. Clearly this is true for $D$, but the thrust line is fixed by engine installation and will not in general be aligned with the wind vector. The difference in alignment will not be large, and hence the assumption given above.
- The weight factor $nW$ acts vertically, normal to the body $x$ axis. In other words, we are confining the analysis to the fuselage being horizontal.
- Note that whilst we might choose to neglect $L_{T}$ in the transverse equation, if $L_{T}<<L_{W}$ we cannot ignore its major contribution to pitching moment because of its long moment arm.
- The tail is not shown to have an elevator: for now we include such effects in any expression for $C_{L_{T}}$

The three equations valid in the plane of symmetry are:
$$\text{Transverse:}~~~~~~ L_{W}+L_{T}=nW$$
$$\text{Axial:}~~~~F=D$$
Pitch: for the moment we shall choose to take moments about the a.c. of the wing, leading to:
$$\begin{align*}
M_{ac}&= M_{0} + nWx\bar{c}-L_{T} l_{T} \\
&= 0~~~\text{for equilibrium}
\end{align*}$$
We can non-dimensionalise the equations using $\bar{q}S$ for forces and $\bar{q}S\bar{c}$ for moments.
![[Pasted image 20251023154951.png|centre]]
![[Pasted image 20251023155004.png|centre]]
![[Pasted image 20251023155026.png|centre]]
### CG/Balance Diagram
[[Flight Dynamics Lecture 9 - Longitudinal Balance.pdf#page=27|Flight Dynamics Lecture 9 - Longitudinal Balance, p.27]]
