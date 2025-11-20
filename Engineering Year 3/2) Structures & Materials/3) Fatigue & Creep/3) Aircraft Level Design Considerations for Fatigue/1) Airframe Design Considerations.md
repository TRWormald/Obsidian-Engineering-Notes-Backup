### Airframe Design Philosophies
**Safe Lift, Fail Safe & Damage Tolerant**
These are the primary design philosophies in aircraft design.
They can sometimes be called "Safety By Retirement", "Safety By Design", and "Safety By Inspection".
#### Safe Life Design
The safe life is the number of flights/landings/flight hours, during which there is a low probability that the strength will degrade below design strength.
The design criteria are:
- Safety by retirement
- Fatigue failure not likely to occur during the design life
- Safe-life interval = projected lifespan of the aircraft = crack free service life.
#### Fail Safe Design
Designed NOT to fail
There are three cases:
1) Infinite life
2) Redundant load paths
3) Residual strength-based design
Design criteria:
- Max stress < FEL (fatigue crack propagation stage)
- Multiple redundant spars in the wing
- Compression after impact (CAI) as design allowable for very conservative design

This is generally economical and safe than safe life.

#### Damage Tolerant Design
Designed with maintenance (detection capability & inspection schedule) in the loop (current). The aircraft are designed assuming the presence of damage, and that they can sustain loads until a critical size of the damage. It is assumed that defects can be detected until they attain the critical design through inspection protocol, and repairs should restore the original strength.

#### The Safety Design Approach
![[Pasted image 20251120111507.png|centre]]
#### FHA/FMEA/FMECA
These are structured engineering practice to analyse potential causes of operational failure.
### Materials & Manufacturing
### Operational Environments
Apply knock down factors repeatedly to obtain the actual strength of the material you can use in your design calculations.

### Detail Designs
#### Stress Levels
We use high fidelity stress analysis to capture stress gradients and concentrations from holes, cut-outs, notches etc.
We use actual loads if possible (from FTI or SHM)
We use allowable strength values only
We limit fuselage hoop stress (quilting or pillowing)
Avoid initial buckling of webs (no buckling up to 1g & 1.5g for civilian and fighter aircraft respectively). Use the design ratio:
$$\frac{\tau_{crit}}{\tau_{ult}}>20\%$$

#### Detail Engineering
- Use large cut-out radii & corner/bend radii (min 2$\times$thickness)
- Avoid sudden discontinuities in sections
- Avoid interacting stress concentrations
- Avoid change in sections at the same location
- Composite lay-up ply drops
#### Joint & Edge Design
- Use sufficient pitch between fastener holes & edge distance to prevent stress concentration interactions
- Limit coutersink depth - increase edge distance to cater for CSKs
- Use thickening / pad-up to reduce stress levels
- Use cold worked holes - for residual compressive stress
- Use correct fastener & installation
- Avoid blind areas
- Avoid eccentriciti