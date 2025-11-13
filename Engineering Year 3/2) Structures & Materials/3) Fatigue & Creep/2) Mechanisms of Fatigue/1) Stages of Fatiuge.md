Fatigue failure stress is much lower than the static strength, the fracture initiates at the surface; the stress concentrations form due to stress raisers.
Damage accumulation stages:
- Stage 1 - Crack Initiation
Safe life design of safety critical or less inspectable structures - crack free life assuming no initial micro crack
- Stage 2 - Slow Propagation of Crack
Fail safe design of easily inspectable structures (e.g. fuselage skin/empennage) - assuming initial micro-crack
- Stage 3 - Fast Propagation of Crack

Fatigue life:
$$N=N_{stage~1}+N_{stage~2}+N_{stage~3}$$
$$N=N_{initiation}+N_{Slow~propagation}+N_{Fast~propagation}$$
$$N=N_{i}+N_{p}$$
### Stage 1 - Crack Initiation
![[Pasted image 20251113110254.png|centre|400]]
Stress raisers result in local plastic deformation and shear based slip (in slip planes along slip directions). There is then a reversal of cycle (a change in direction of the slip planes) and this leads to the formation of extrusions and intrusions.
The intrusions act as small cracks, which grow, cutting through the gain boundaries to slip planes of adjacent grains, resulting in macroscopic surface cracks.

Repeated Loading > Plastic Deformation > Shear Based Slip > Reversal > Extrusions & Intrusions > More Loading > Formation of Macroscopic Cracks

This occurs if $S_{max}$ or $S_{local}>$ Yield Strength

So to reduce the chance of crack initiation we use a material with a higher Yield Strength or use different strengthening mechanisms, or we lower $S_{local}$ by reducing stress concentrations - e.g. with good surface finish, proper component design (no abrupt changes in cross section, no sharp corners or edges) and making sure there are no microscopic defects (porosity, cavities, non-metallic inclusions.)

We can also minimise gaps and use structural shims.

### Stage 2 - Slow Propagation of Crack
Now the crack is open it goes through several processes:
- Tensile cycle
- Cycle reversal
This results in: net advancement in each cycle = crack advancement in tensile cycle - crack closure in compression cycle.
If the net advancement = 0 the component has infinite fatigue life. Else the crack growth rate $da/dN$ as per Paris Law/Paris Erdogan equation.

**But how do we slow the propagation of the crack?**
$da/dN$ gives us the crack advancement rate (crack advancement-crack closure/N). 
To reduce crack advancement we use a material with a higher Yield Strength
To increase crack closure we use a material with a higher plastic deformation (i.e. lower Yield Strength).

This is contradictory and requires optimisation, we can strike a balance by using surface/case hardening, or residual compressive stresses - i.e. attempting to have a negative compressive mean stress this can be cone with shot peening/sand blasting (which can increase fatigue life by 10x) amazingly overloads can also increase fatigue life but this is not capable to be designed for.

### Stage 3 - Fast Propagation of Crack
The crack progresses quickly, lowering the load of the bearing area.
$$S_{local}>UTS$$
Finally we have the fracture of the material
![[Pasted image 20251113113837.png|centre|400]]
![[Pasted image 20251113113853.png|centre|500]]
### Safeguards for Composite Structures
**Ply drop protocols**
For primary structures:
Ply drop length = $20\times CPT\times n$
For secondary structures
Ply drop length = $10\times CPT\times n$


