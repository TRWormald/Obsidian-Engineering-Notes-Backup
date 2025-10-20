The Helmholtz theorems together with our knowledge of the flow structure over aerofoils and finite wings leads to a first simple model of 3D wing flow based on a 2D single "lumped vortex" model where the Kutta condition was applied by matching to thin aerofoil theory.
![[Pasted image 20250310182306.png|centre]]
We begin this process by starting with a "bound vortex"
![[Pasted image 20250310182320.png|centre]]

The "bound vortex" cannot end at wing tips.
We then have trailing or tip vortices which are perpendicular to the bound vortex, and the circuit is completed by the starting vortex:
![[Pasted image 20250310182703.png|centre]]
The starting vortex convects downstream, which gives a "horseshoe vortex" in steady state flow when the effect of the starting vortex can be neglected:
![[Pasted image 20250310182758.png|centre|350]]
This is the simplest solution that satisfies the requirement for the shed wake to be force free and leave the thin wing smoothly.
### Lift Distribution in the Horseshoe Vortex Model
The circulation distribution of the Horseshoe Vortex Model is:
![[Pasted image 20250310183109.png|centre]]
And hence the lift distribution is:
![[Pasted image 20250310183232.png|centre]]
Which we can compare to the representative loading:
![[Pasted image 20250310183324.png|centre]]
And see that it is uniform in comparison to the latter where it is greater towards the centre of the aerofoil.
### Downwash
The Bound (lifting) wing vortex does not induce a velocity on itself. However the trailing or tip vortices induce a velocity on the bound vortex:
![[Pasted image 20250310183446.png|centre]]
Velocity induced by tip vortices along the wing bound vortex is a pure downwash, which is proportional to $\Gamma$.
### The Effects of Trailing or Tip Vortices
Consider the local flow over an element of the bound vortex in more detail:
**With No Tip Vortices:**
![[Pasted image 20250310183648.png]]
**With Tip Vortices:**
Now the downwash effects can be superposed:
![[Pasted image 20250310183733.png|centre]]
NB vertical velocity in the $z$ direction is $w$. The downwash is the velocity in the downwards direction. So a downwash corresponds to a negative value for $w$ or in other words a positive value for $-w$.
### Lift-Dependent Drag
The presence of tip vortices results in drag.
Note that the downwash velocity $-w$ is directly proportional to the tip vortex strength $\Gamma$, so:
$$-w\propto\Gamma\rightarrow -w\propto l$$
$$d_{i}\propto \Gamma^{2}\rightarrow d_{i}\propto l^{2}$$
Where the subscript $i$ has been introduced because this is induced drag.
### Alternate Interpretation of Tip Vortices
We can also interpret tip vortices in the following way:
![[Pasted image 20250310184055.png|centre]]
Consider the above, the flow over a section can be though of as being due to a rotated free stream velocity:
![[Pasted image 20250310184131.png|centre|250]]
### Uses of the Horseshoe Vortex Model
It is a simple demonstration of the fundamental reason for the existence of induced drag.
It provides first order estimates of interactions between lifting surfaces.
	Usually used in a modified form where the total lift and hence circulation associated with the horseshoe vortex is the same as that for the actual wing.
![[Pasted image 20250310184338.png|centre]]
However the horseshoe vortex model does not lead to good quantitative prediction of lift and drag for 3D wings.
### Deficiencies of the Horseshoe Vortex Model
The model predicts non-physical flow in the vicinity of the wing, in reality the top vortices do not originate just at the wing tips.
Also, bound circulation $\Gamma$ should vary with span:
	- For a horseshoe vortex all bound $\Gamma$ is shed at the tips
	- For a real wing, bound $\Gamma$ is progressively shed along the span, from the centreline to the tips
### The Lifting Line Theory
The variation of the circulation along the span is modelled by superimposing horseshoe vortices of varying strength. In the original version of this method the bound vortices are coincident along the lifting line, which is usually located at the local quarter chord.
![[Pasted image 20250310190524.png|centre]]
#### Circulation Distribution
The result is a lifting line with bound circulation $\Gamma(y)$ varying with span $y$:
![[Pasted image 20250310190609.png|centre]]
Note that each time the circulation jumps, another vortex is shed into the wake with circulation equal to the jump, i.e. there are multiple vortex pairs shed into the wake across the span.
#### Limiting Case-Circulation Distribution
In the limit, use an infinite number of horseshoe vortices, each of strength $d\Gamma$. This gives a continuous bound circulation distribution $\Gamma(y)$ on the lifting line, together with a continuous vortex sheet shed from the wing trailing edge of strength $\gamma_{x}(y)$.
![[Pasted image 20250310190838.png|centre]]
## Revision
![[Pasted image 20250316172802.png|centre]]
