We will be looking at:
- Dynamic Aeroelasticity of an Elastically Supported Pitching-Heaving Aerofoil model
	- Generalised loads and quasi-steady aerodynamics
	- Aeroelastic matrices
- Dynamic Aeroelasticity Analysis
	- Aeroelastic eigenvalue problem
	- Eigenvalue loci in the complex plane and stability
	- Binary flutter and its mechanism
- Other considerations
### 2DOF Aeroelastic Model
We have previously seen the 2DOF model of a rigid wing:
![[Pasted image 20250311110743.png|centre]]
Which has equations of motion:
$$\begin{align*}&
\begin{bmatrix} m&mx_{CM} \\ mx_{CM}&I_{CM}+mx^{2}_{CM}\end{bmatrix}\begin{bmatrix}\ddot{q}_{1}\\\ddot{q}_{2}\end{bmatrix}+\begin{bmatrix}k_{y}&0\\0&k_t\end{bmatrix}\begin{bmatrix}q_{1}\\q_{2}\end{bmatrix}\\\\
&= \boxed{\begin{bmatrix}L\\M_{AC}+Lx_{AC}\end{bmatrix}}
\end{align*}$$
### Quasi-Steady Aerodynamics
**Quasi-Steady Aerodynamics**: At any instant in time, the aerodynamic characteristics are assumed to be the same as if the aerofoils were moving with constant heave or pitch velocities (c.f. steady aerodynamics = no motion)
![[Pasted image 20250311111447.png|centre]]
Therefore the moment change due to the pitching velocity:
$$C_{M_{ac}}=C_{M_{ac},\dot{\theta}}\frac{\dot\theta c}{U},~~~C_{M_{ac},\dot{\theta}}<0$$
Where $C_{M_{ac},\dot{\theta}}$ is the rate of change of moment with respect to the non-dimensionalised pitching velocity and is typically negative.

Therefore the **Generalised Loads with Quasi-Steady Modifications**:
$$Q_{1}=L=qSC_{L}=qSC_{L,\alpha}(\theta-\dot{y}/U)$$
$$\begin{align*}
Q_{2}&= M_{AC}+Lx_{AC}\\
&= qSc\cdot C_{M_{ac},\dot{\theta}}(\dot\theta c/U)+qSC_{L,\alpha}(\theta-\dot{y}/U)ec
\end{align*}$$
Where $S=sc$ and $S$ is the planform area, $s$ is the wing span, and $c$ is the chord length.
### The Aeroelastic Model in Matrix Form
![[Pasted image 20250311112313.png|centre]]
### Aeroelastic Eigenvalue Analysis
![[Pasted image 20250311112359.png|centre]]
### Eigenvalue Analysis
![[Pasted image 20250311112419.png|centre]]
### Flutter Diagram and Flutter Mechanism
![[Pasted image 20250311112501.png|centre]]
### Other Considerations
![[Pasted image 20250311112549.png|centre]]
## Summary
![[Pasted image 20250311112605.png|centre]]
