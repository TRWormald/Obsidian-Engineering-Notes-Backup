'Let us consider the equation of motion for a 1DOF system:
$$m\ddot{x}+c\dot{x}+kx=F(t)$$
To solve this we:
1) Solve the homogeneous ODE (the component due to free response)
2) Solve the RHS - a component due to the applied force $F(t)$
This relates to the **Complementary** and **Particular** solutions that we have previously seen in [[Solution Structure for Nonhomogeneous ODEs]].
**The Complementary Solution** - where RHS=0
$$\begin{align*}
x_{H}&= Xe^{-\zeta\omega_{0}t}\sin(\omega_{D}t+\varphi)\\
&= e^{-\zeta\omega_{0}t}(X_{1}\sin(\omega_{D}t)+X_{2}\cos(\omega_Dt))
\end{align*}$$
**The Particular Solution** - where RHS=f(t)
- For constant force: $F(t)=F_{0}=const.$
- For harmonic force: $F(t)=F_{0}\sin(\omega t)$

The **Total Solution** is obtained through the superposition of the complementary and particular solutions:
$$\begin{align*}
x&= x_{H}+x_{P}\\
&= e^{-\zeta\omega_{0}t}(X_1\sin(\omega_{D}t)+X_{2}\cos(\omega_{D}t))+x_{forced}
\end{align*}$$
### Total Vibration Response
![[Pasted image 20250120161544.png|centre]]
![[Pasted image 20250120161608.png]]
**Note: Constant force produces a steady-state static deflection (a new equilibrium position)**
