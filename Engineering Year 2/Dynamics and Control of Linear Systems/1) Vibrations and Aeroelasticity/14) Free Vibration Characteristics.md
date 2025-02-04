We saw in the previous lecture that the equation of motion for a NDOF system with no damping was:
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{f}(t)$$
![[Pasted image 20250204115743.png|centre]]
Here we'll be looking at:
- Free response
- Eigenvalue problem
- The characteristic equation
- Numerical solutions using MATLAB
### Free Vibrations
Lets consider a linear, forced, undamped system:
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{f}(t)$$
We will study the free vibrations of this system (i.e. when $\mathbf{f}(t)=0$):
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{0}$$
We assume that this system can vibrate freely at a **single** frequency:
$$\begin{align*}
\mathbf{x}&= \begin{bmatrix}x_{1} \\ x_{2}\end{bmatrix}=\begin{bmatrix}a_{1}\sin(\omega t+\varphi) \\ a_{2}\sin(\omega t +\varphi)\end{bmatrix}\\
&= \begin{bmatrix}a_{1} \\ a_{2}\end{bmatrix}\sin(\omega t +\varphi)=\mathbf{a}\sin(\omega t +\varphi)
\end{align*}$$
Where $\mathbf{x}$ is the vector of displacements, $\mathbf{a}$ is the vector of displacement amplitudes, $\omega$ is the frequency of vibration, and $\varphi$ is the phase angle.
#### Free Vibration Response
We use the assumed motion function to find the free response of the system:
$$\begin{align*}
\mathbf{x}&= \mathbf{a}\sin(\omega t +\varphi)\\
\mathbf{\dot{x}}&= \omega\mathbf{a}\sin(\omega t +\varphi)\\
\mathbf{\fdot{x}}&= \omega\mathbf{a}\sin(\omega t +\varphi)
\end{align*}$$