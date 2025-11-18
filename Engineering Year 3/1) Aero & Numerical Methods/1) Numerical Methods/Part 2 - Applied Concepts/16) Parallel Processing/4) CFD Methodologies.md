The inter-processor communication depends on the flow solver.
**Near-Neighbour Communication**
- Explicit finite-difference schemes
- Explicit finite-volume schemes
For these solvers only halo cell data has to be transferred between neighbouring processors.
**Global Data Dependency**
- Implicit finite-volume or finite-difference schemes
- Panel methods
- Spectral methods
- Point vortex models
In these cases every processor has to communicate with every other one