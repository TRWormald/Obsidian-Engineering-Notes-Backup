![[Pasted image 20251020110750.png|centre]]
### Iterative Coupling with Transpiration Velocity
The goal is to have the inviscid outer flow match the viscous boundary layer. This is done iteratively, and the transpiration velocity is the key mechanism.
![[Pasted image 20251020111505.png|centre]]
A normal velocity is added at the surface of the aerofoil in the inviscid solver. This mimics the effect of the boundary layer pushing the outer flow away from the surface. (This is a new B.C. for inviscid solutions)