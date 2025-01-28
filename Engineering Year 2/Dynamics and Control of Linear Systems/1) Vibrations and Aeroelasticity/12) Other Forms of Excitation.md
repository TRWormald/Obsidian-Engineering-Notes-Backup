We have [[10) Harmonic Excitation|previously]] looked at Force, Unbalance, and Base Excitation, and the [[11) Transfer Functions#Frequency Response Function|FRF]] and its equivalents.
We're now going to look at:
- Multi-harmonic excitation
- Impulse excitation
### An overview of Vibrations (so far)
![[Pasted image 20250128111830.png|centre]]
### Multi-Harmonic Excitation
![[Pasted image 20250128112331.png|centre]]
>We know about the principle of superposition - where the total solution is the sum of all partial solutions resulting for individual components of excitation. We can apply this to harmonic excitation by forming multiple differential equations describing the motion of a system and simply adding the resulting functions describing displacement.

The partial steady state solutions are:
$$m\ddot{x}_{1}+x\dot{x}_{1}+kx_{1}=F_{C,1}e^{i\omega_{1} t}~\Rightarrow~x_{1}=(H(\omega_{1})F_{C,1})e^{i\omega_{1}t}$$
$$m\ddot{x}_{2}+x\dot{x}_{2}+kx_{2}=F_{C,2}e^{i\omega_{2} t}~\Rightarrow~x_{2}=(H(\omega_{2})F_{C,2})e^{i\omega_{2}t}$$
Meaning that the total steady state solution is:
$$\begin{align*}
x(t)&= x_{1}(t)+x_{2}(t)\\
&= H(\omega_{1})F_{C,1}e^{i\omega_{1}t}+H(\omega_{2})F_{C,2}e^{i\omega_{2}t}
\end{align*}$$
**However**... it should be noted that this method only allows us to predict the steady state response of the system - not the transient response:
![[Pasted image 20250128113028.png]]
The red dotted lines is our solution from the method above, whilst the blue line is the full solution from integrating the ODE with $F(t)$. As we can see initially these plots are dissimilar, but once the system is allowed to settle down they match up.
### Impulse Excitation
![[Pasted image 20250128113158.png|centre]]
![[Pasted image 20250128113221.png|centre|250]]
In **Impulse Excitation** the force applied to a system is only for a finite period of time for which the following applies:
$$T_{P}<<T_{D}=\frac{2\pi}{\omega_{D}}$$
We also have to assume that:
$$x(T_{P})\approx 0$$
Whilst:
$$\frac{dx}{dt}T_{P}\ne 0$$
This means that up to $T_{P}$ there is no 