### Harmonic Excitation
Consider a forced MDOF system:
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{f}(t)$$
and assume that the harmonic load is defined as follows:
$$\mathbf{f}(t)=\begin{bmatrix}f_{0,1}\cos(\omega t)\\...\\f_{0,M}\cos(\omega t)\end{bmatrix}=\begin{bmatrix}f_{0,1}\\ ...\\f_{0,M}\end{bmatrix}\cos(\omega t)=\mathbf{f}_{0}\cos(\omega t)$$
Where $\mathbf{f}_{0}$ is the vector of excitation amplitudes and $\omega$ is the excitation frequency.
The 2DOF example of this would be:
![[Pasted image 20250225142654.png|centre]]
### Steady-State Harmonic Response
We can study the steady state response of the system:
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{f}_{0}\cos(\omega t)$$
The response is assumed in the following form:
$$\mathbf{x}=\mathbf{x}_{0}\cos(\omega t)+\mathbf{K x}_{0}\cos(\omega t)=\mathbf{f}_{0}\cos(\omega t)$$
Where $\mathbf{x}_{0}$ is the vector of unknown response amplitudes, $\omega$ is the known excitation frequency. The phase angle is 0 or 90 degrees. This information is captured by the signs of the components of $\mathbf{x}_{0}$.

The vector of the response amplitudes is found after the following substitutions:
$$-\omega^{2}\mathbf{M x}_{0}\cos(\omega t )+\mathbf{K x}_{0}\cos(\omega t)=\mathbf{f}_{0}\cos(\omega t)$$
$$(\mathbf{K}-\omega^{2}\mathbf{M})\mathbf{x}_{0}=\mathbf{f}_{0}$$
So:
$$\boxed{\mathbf{x}_{0}=(\mathbf{K}-\omega^{2}\mathbf{M})^{-1}\mathbf{f}_{0}}$$
Where $(...)^{-1}$ denotes an inverse matrix.
### 2DOF Example
![[Pasted image 20250225143700.png|centre]]
![[Pasted image 20250225143710.png|centre]]
![[Pasted image 20250225143723.png|centre]]
![[Pasted image 20250225143738.png|centre]]
![[Pasted image 20250225143758.png|centre]]
