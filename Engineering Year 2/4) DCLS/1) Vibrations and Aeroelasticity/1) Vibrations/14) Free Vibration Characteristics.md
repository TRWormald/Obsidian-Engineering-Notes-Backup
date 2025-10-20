We saw in the previous lecture that the equation of motion for a NDOF system with no damping was:
$$\mathbf{M\ddot{x}}+\mathbf{Kx}=\mathbf{f}(t)$$
![[Pasted image 20250204115743.png|centre]]
Here we'll be looking at:
- [[14) Free Vibration Characteristics#Free Vibration Response|Free Vibration Response]]
- [[14) Free Vibration Characteristics#The Eigenvalue Problem|The Eigenvalue Problem]]
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
\mathbf{\dot{x}}&= \omega\mathbf{a}\cos(\omega t +\varphi)\\
\mathbf{\ddot{x}}&= -\omega^{2}\mathbf{a}\sin(\omega t +\varphi)
\end{align*}$$
We substitute the vector of displacements and accelerations to the EOM:
$$-\omega^{2}\mathbf{M~a}\sin(\omega t +\varphi)+\mathbf{K~a}\sin(\omega t +\varphi)=\mathbf{0}$$
So:
$$(\mathbf{K}-\omega^{2}\mathbf{M})\mathbf{a}\sin(\omega t+\varphi)=\mathbf{0}$$
This equation is valid for all time instants, therefore:
$$(\mathbf{K}-\omega^{2}\mathbf{M})\mathbf{a}=\mathbf{0}$$
Hence we have obtained a linear (matrix) equation with the unknown vector of amplitudes $\mathbf{a}$ and unknown frequency $\omega$. This problem is called the *Eigenvalue Problem*.
### The Eigenvalue Problem
The eigenvalue problem is:
$$(\mathbf{K}-\omega^{2}\mathbf{M})\mathbf{a}=\mathbf{0}
$$
For 2DOF system, this problem has two solutions: $\omega_{1}^{2}, \mathbf{a_{1}}$ and $\omega^{2}_{2},\mathbf{a}_{2}$. The values $\omega_{i}^{2}$ are called eigenvalues and the vectors $\mathbf{a_{i}}$ are called eigenvectors or mode shapes.
Eigenvalues are squares of the undamped natural frequencies $\omega_{i}$.

We will consider two different ways of solving the eigenvalue problem:
- For *small* systems (e.g. 2DOF) we can use the analytical method
- While for larger problems, or where larger calculations are needed, we use the *numerical* method which is available in MATLAB
![[Pasted image 20250204121528.png|centre]]
#### Solving the Eigenvalue Problem
 The eigenvalue problem:
$$(\mathbf{K}-\omega^{2}\mathbf{M})\mathbf{a}=\mathbf{0}$$
For this system of linear equations there are two types of solutions:
- *One trivial solution*, where $\mathbf{a}=0$ (zero amplitude of vibration = no vibration)
- *Non-trivial solutions*, where $\mathbf{a}\ne 0$ (non-zero vibration amplitudes)
##### The Analytical Solution
We are interested in the non-trivial solutions. Assuming that $\mathbf{a}\ne 0$, the condition for the non-trivial solutions is that the determinant of the system matrix is zero. Therefore:
$$\boxed{\det(\mathbf{K}-\omega^{2}\mathbf{M})=0}$$
##### The Numerical Solution
An alternative approach to solving this problem uses numerical methods. MATLAB can determine all eigenvalues and eigenvectors of the standard problem:
$$(\mathbf{K}-\omega_{i}^{2}\mathbf{M})\mathbf{a_{i}}=\mathbf{0}~~~\Rightarrow~~~\mathbf{Ka_i}=\lambda_{i}\mathbf{Ma_{i}},~~~ \lambda_i=\omega_{i}^{2}$$
So:
>K=...      % stiffness matrix
>M=...     % mass matrix
>$[$Evec,Eval$]$=eig(K,M);

### Example
![[Pasted image 20250204122327.png|centre]]
![[Pasted image 20250204122340.png|centre]]
![[Pasted image 20250204122406.png|centre]]
![[Pasted image 20250204122421.png|centre]]
