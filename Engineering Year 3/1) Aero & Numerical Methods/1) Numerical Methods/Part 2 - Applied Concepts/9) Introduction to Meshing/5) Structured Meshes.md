### Simple Cartesian
The image below shows a simple cartesian mesh:
![[Pasted image 20251021132703.png|centre|400]]
It is not body-fitted, meaning that we have poor surface representation or need special parameterisation methods at the surface (immersed boundary).
These are rarely used on their own - we need body-fitted grids.
Although they are often used for a background grid in Chimera/Overset methods.
### Body-fitted
There are three main mesh topologies when considering body-fitted structured grids.
Each topology maps a regular cartesian grid around a boundary such that the body forms a boundary of the grid.
O-type meshes are used for inviscid flows, while C- and H-Type are used for RANS.
![[Pasted image 20251021132943.png|centre|300]]
![[Pasted image 20251021133000.png|centre|400]]
![[Pasted image 20251021133013.png|centre|300]]
### Multiblock Meshes
For real configurations we most-often need multiple structured blocks to mesh our domain: a complex mesh is generated from many simple meshes. For example this aerofoil and flap combination:
![[Pasted image 20251021133130.png|centre|400]]
However it is important that the mesh point distributions at each block boundary must match exactly: therefore no interpolation of the solution is required.
![[Pasted image 20251021133231.png|centre]]
For complex configurations, placing and matching structured blocks is a skilled and time consuming process.
![[Pasted image 20251021133311.png|centre]]


