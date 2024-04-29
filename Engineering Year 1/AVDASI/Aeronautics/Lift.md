### The Definitions of Lift and Drag
![[Pasted image 20240429134127.png|center]]
**Lift (L)** is the component of the aerodynamic force *perpendicular* to the relative wind.
**Drag (D)** is the component of the aerodynamic force *parallel* to the relative wind.
\
**Note that the lift is not always up! It is perpendicular to the plane of the wings.**
### Aerodynamic Forces
![[Pasted image 20240429134332.png|center]]
The Aerodynamic forces generated depend on:
- The shape and size of the body
- The free-stream velocity ($V_{\infty}$)
- The **incidence angle** or **angle of attack ($\alpha$)**, which is the angle between the chord line and the free stream velocity.
### The Aerodynamic Moment
There is also a **Pitching Moment** acting about a defined axis (usually the leading edge or quarter-chord point):
![[Pasted image 20240429134632.png|center]]
This is caused by the distribution of pressure over the wing.
### The Generation of Lift
The easiest way to explain how lift is generated is via **Redirection**. This is effectively just leveraging Newton's Second Law (that the force is proportional to the rate of change of momentum) and therefore the momentum of the air directed/deflected downwards is equal and opposite to the momentum imparted to the aircraft.
So:
$$\text{Lift}[kg~m/s^{2}]=\text{Diverted Air}[kg/s]\times\text{Vertical Velocity}[m/s]$$
The diverted air is proportional to the **speed** as well as the **air density**:
$$\frac{m}{t}\propto V_{\infty},\rho$$
The vertical velocity is proportional to the **speed** as well as the **angle of attack**:
$$V_{v}\propto V_\infty,\alpha$$
Hence lift is a function of the speed squared, the angle of attack, and the air density.
This is what allows us to derive the equation for the coefficient of lift:
$$L=\frac{1}{2}\rho V^{2}SC_{L}$$
$$C_{L}=\frac{L}{\frac{1}{2}\rho_{\infty} V_{\infty}^{2}S}$$