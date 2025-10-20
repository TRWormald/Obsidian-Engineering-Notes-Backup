In this we will look at:
- Free response via mode superposition
- Initial Conditions
- A 2 DOF Example

### Mode Superposition
Consider a MDOF system without applied load (i.e. in free vibration) and with non-zero initial conditions:
$$\mathbf{M\ddot{x}+Kx=0}$$
The free response of this system can be expressed as a superposition of all the modes of the system:
$$\mathbf{x=a_{1}}(C_{1}\cos(\omega_{1}t +\varphi_{1}))+\mathbf{a_{2}}(C_{2}\cos(\omega_{2}t +\varphi_{2}))+...$$
Where $C_{1},C_{2},...;~~~\varphi_{1},\varphi_{2},...$ are 2M unknown constants.
Unknown constants $C_{i}$ and $\varphi_{i}$ depend on the initial conditions (ICs):
- Initial displacements
- Initial velocities
$$t=0:~~~\mathbf{x}(0)=\mathbf{x}_{0},~~~\mathbf{\dot{x}}(0)=\mathbf{\dot{x}}_{0}$$
We use the free response and initial conditions to set up 2M equations to solve for 2M unknown constants:
$$\mathbf{x}_{0}=C_{1}\mathbf{a}_{1}\cos(\varphi_{1})+C_{2}\mathbf{a}_{2}\cos(\varphi_{2})+...$$
$$\mathbf{\dot{x}}_{0}=-\omega_{1}C_{1}\mathbf{a_{1}}\sin(\varphi_{1})-\omega_{2}C_{2}\mathbf{a}_{2}\sin(\varphi_{2})-...$$
![[Pasted image 20250204123945.png|centre]]
### 2DOF Example
![[Pasted image 20250204124015.png|centre]]
![[Pasted image 20250204124046.png|centre]]
![[Pasted image 20250204124100.png|centre]]
![[Pasted image 20250204124116.png|centre]]
![[Pasted image 20250204124134.png|centre]]
![[Pasted image 20250204124149.png|centre]]
