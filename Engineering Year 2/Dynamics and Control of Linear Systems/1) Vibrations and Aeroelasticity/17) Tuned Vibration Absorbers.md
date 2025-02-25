### Amplitude-Frequency Characteristics for 1 and 2 DOF Systems
![[Pasted image 20250225150039.png|centre]]
### Generic Tuned Vibration Absorber Model
![[Pasted image 20250225150153.png|centre|250]]
In the general tuned vibration absorber model we have a 2DOF system. The equation of motion are:
$$m_{1}\ddot{x}_{1}+k_{1}x_{1}-k_{2}(x_{2}-x_{1})=f_{0,1}\cos(\omega t)$$
$$m_{2}\ddot{x}_{2}+k_{2}(x_{2}-x_{1})=0$$
$$x_{i}(t)=x_{0,i}\cos(\omega t),~i=1,2$$
With the harmonic response being given by:
$$\begin{bmatrix}k_{1}+k_{2}-\omega^{2}m_{1}&-k_{2}\\-k_{2}&k_{2}-\omega^{2}m_{2}\end{bmatrix}\begin{bmatrix}x_{0,1}\\x_{0,2}\end{bmatrix}=\begin{bmatrix}f_{0,1}\\0\end{bmatrix}$$
We want to find the amplitudes, $x_{0,1}$ and $x_{0,2}$ which can be done using the matrix inverse or Gaussian Elimination.
Resulting in the following:
![[Pasted image 20250225150654.png|centre]]
With the amplitude of the harmonic response of block one being zero if:
![[Pasted image 20250225150725.png|centre]]
i.e. If the secondary system is tuned (designed) such that it's own natural frequency is equal to the frequency of excitation (which might be the resonant frequency) then the secondary system is called a Tuned Vibration Absorber.
### Controlling Resonant Vibrations
TVAs are useful for passive control of resonant vibrations. Assuming an undamped problem, the harmonic excitation at the undamped natural frequency $\omega=\omega_{0}$, causes resonance. TVA can be designed such that $\omega_{a}=\omega=\omega_{0}$ and the steady-state amplitude $x_0,1$ will change from $x_{0,1}\rightarrow \pm\infty$ to $x_{0,1}=0$.

The TVA tuning condition applied to the system with resonant excitation is:
$$\omega_{0}^ 2=\frac{k_{1}}{m_{1}}=\frac{k_{2}}{m_{2}}=\omega_{a}^{2}$$
Which is illustrated in the following graph:
![[Pasted image 20250225151208.png|centre]]
### Further TVA Considerations
The properties of 2DOF systems with TVA:
- 1DOF primary system changes to a 2DOF system (primary + TVA)
- The primary system has one anti-resonance frequency (no-motion)
- The tuning condition represents one equation with two unknowns $k_{2}$ and $m_{2}$
	- So we nee