The Navier-Stokes equations in a fixed Cartesian coordinate system describe unsteady, viscous, compressible flow with body forces. The equations are:
- Continuity, conservation of mass (1 eqn)
- Conservation of Momentum in each coordinate direction (3 eqns)
- Conservation of total Energy (1 eqn)
- Two equations of state - i.e. the fundamental properties of the fluid. (We will typically use the Gas Law and a law related to Viscosity.)
### Calculating N-S Solutions
Numerically resolving all the detail of a N-S solution is not possible at Reynolds numbers typically found in aerodynamics - because of small eddies/turbulence. 
N-S solutions are not routinely calculated, even today - typically reserved for very specialist circumstances.

As a result we cant get analytical solutions, so we make series' of assumptions to simplify the equations. The first three are:
1) Viscous effects are negligible (this is typically valid - because they are confined to below the boundary layer)
2) Steady flow
3) No body forces (this is typically valid for aerodynamic flows because of the low density of air)
These assumptions result in some rather complex equations:![[Pasted image 20250110184047.png]]
**Which we don't need to memorise!**
Now are these equations any good?
**Yes**, we can still have rotational flow (i.e. lift generation) and nonlinear features like shocks are modelled. However we cannot model separated or turbulent flow (as then our assumption about viscous effects is no longer true).
Many CFD programmes solve the Euler equations - however it is important to note that when you get drag results from these CFD programmes it is excluding viscous effects.