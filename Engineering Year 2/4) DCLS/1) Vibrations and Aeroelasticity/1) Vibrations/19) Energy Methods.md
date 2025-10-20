We are primarily going to look at:
1) Lagrange's Equations of the second kind used to derive equations of motion for multi-DOF systems
	- E.g. Pitching-heaving wing section
	- E.g. Two Coupled Pendulums
2) Energy balancing to determine the natural frequency of 1DOF systems
	- E.g. Rudder control mechanism
### Overview of Basic Energy Concepts
![[Pasted image 20250301174924.png|centre]]
### Method 1: Lagrange's Equations
**Lagrange's Equations** (of the second kind) for $N$ DOF systems:
$$\frac{d}{dt}\left(\frac{\partial\mathcal{L}}{\partial\dot{q}_{j}}\right)-\frac{\partial\mathcal{L}}{\partial\dot{q}_{j}}=Q_{j},~~~~~j=1,~2,...,~N$$
Where:
$$\mathcal{L}=E_{K}-E_{P}$$
$\mathcal{L}$ is the **Lagrangian Function**
$E_{K}$ is the total Kinetic Energy
$E_{P}$ is the total Potential Energy
$q_{j}$ are the generalised coordinates (angle, deformation, deflection)
$Q_{j}$ are the generalised loads (forces or moments)

Properties and advantages of the Lagrangian:
- Using scalar (energy functions) instead of vectors = "safer" derivations (fewer signs)
- Consistent approach wen working with rectilinear and angular DOFs and loads
- Minimum number of equations (EOMs) for multi-body and multi-DOF systems
- Useful for automatic EoM derivation using symbolic maths tools
#### Example: Pitching-Heaving Wing Section
![[Pasted image 20250301180108.png|centre]]
![[Pasted image 20250301180122.png|centre]]
![[Pasted image 20250301180148.png|centre]]
![[Pasted image 20250301180202.png|centre]]
![[Pasted image 20250301180215.png|centre]]
![[Pasted image 20250301180243.png|centre]]
#### Example: Two Coupled Pendulums
![[Pasted image 20250301180312.png|centre]]
![[Pasted image 20250301180322.png|centre]]
![[Pasted image 20250301180339.png|centre]]
![[Pasted image 20250301180351.png|centre]]
### Method 2: The Energy Balancing Method
We can use this method to derive the natural frequencies of 1DOF systems with low or no damping. This method is particularly useful when the system consists of multiple rigid bodies interacting.
There are serval assumptions that need to be made first:
- Low damping (e.g. $\zeta<0.005$) or undamped system
- Linear system vibrating at the frequency $\omega$ 
- Single degree of freedom system
- No excitation = free vibrations

Energy conservation is considered between the two extreme states:
- Maximum displacement and zero velocity
- Maximum velocity and zero displacement
In other words the maximum and minimum points for the potential and kinetic energies respectively.
$$E_{Tot}(t)=E_{P,tot}(q_{max})=E_{K,tot}(\dot{q}_{max})$$
Energy is conserved between these two states during harmonic vibrations at the natural frequency.
$$\sum\limits_{(i)}E_{P,i}(q_{max})=\sum\limits_{(j)}E_{K,j}(\dot{q}_{max})\Rightarrow\omega_{0}$$
This balancing equation offers a means of quick calculation of the natural frequency without the need to derive the EoM.
#### Example: Rudder Control Mechanism
![[Pasted image 20250301181112.png|centre]]
![[Pasted image 20250301181133.png|centre]]
![[Pasted image 20250301181147.png|centre]]
![[Pasted image 20250301181201.png|centre]]
## Summary
![[Pasted image 20250301181255.png|centre]]


