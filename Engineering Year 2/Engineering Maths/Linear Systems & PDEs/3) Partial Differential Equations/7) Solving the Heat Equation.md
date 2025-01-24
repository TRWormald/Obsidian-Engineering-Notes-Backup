#### Defining the Problem
Find the solution $u(x,t)$ of the [[1) Introduction to PDEs#The Heat Equation|Heat Equation]]
on a finite domain:
$$u_{t}=\alpha ^{2}u_{xx}$$
$$0\le x\le L,~~~~ t>0$$
Subject to boundary conditions (perfect insulator/no heat flux):
$$u_{x}(0,t)=u_x(L,t)=0$$
For all $t>0$.
And an initial temperature distribution:
$$u(x,0)=h(x)$$
For all $0\le x\le L$.
#### Step 1 - Separate the Variables
We assume that the solution is separable so:
$$\frac{\partial u}{\partial t}=\alpha ^{2}\frac{\partial^{2}u}{\partial x}$$
Becomes:
$$T'(t)X(x)=\alpha^{2}T(t)X''(x)$$
Allowing us to separate the variables:
$$\frac{1}{\alpha^{2}} \frac{T'(t)}{T(t)}=\frac{X''(x)}{X(x)}$$
And since time is not dependant on space, or vice versa the above must be equal to a constant $\mu$ ([[5) Solving the Wave Equation#What Sign Should the Separation Constant Be?|The Separation Constant]]) allowing us to generate 2 ODEs with the above equation:
$$T'(t)=\alpha^{2}\mu T(t)$$
$$X''(x)=\mu X(x)$$
