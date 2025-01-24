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
We know that for the heat equation the separation constant must be negative so:
$$\mu=-k^{2}$$
#### Step 2 - Solve the Separated ODEs
Knowing that $\mu=-k^{2}$:
$$\frac{1}{\alpha^{2}} \frac{T'(t)}{T(t)}=\frac{X''(x)}{X(x)}=-k^{2}<0$$
So we get the two ODEs:
$$T'(t)=-(\alpha k)^{2} T(t)$$
$$X''(x)=-k^{2} X(x)$$
Both of which are easy to solve:
$$T(t)=Ae^{-(\alpha k)^{2}t}$$
$$X(x)=B\cos(kx)+C\sin(kx)$$
#### Step 3 - Separate and Apply the Homogeneous Boundary Conditions
The homogeneous boundary conditions are:
$$u_{x}(0,t)=u_x(L,t)=0$$
Which we can separate to obtain:
$$X'(0)T(t)=0$$
and
$$X'(L)T(t)=0$$
From which it is obvious that:
$$X'(0)=X'(L)=0$$
Applying these to $X(x)$ gives us:
$$X'(x)=-Bk\sin(kx)+Ck\cos(kx)$$
So:
$$Ck=0$$
$$-Bk\sin(kL)=0$$
Hence:
$$k=\frac{n\pi}{L}$$
#### Step 4 - Put the Pieces Together and Find the General Solution
So substituting this back into the ODEs gives:
$$X(x)=B\cos\left(\frac{n\pi x }{L}\right)$$
$$T(t)=Ae^{-\left(\frac{n\pi\alpha}{L}\right)^{2}t}$$
Which we can multiply together to obtain the PDE:
$$u_{n}(x,t)=a_{n}\cos\left(\frac{n\pi x}{L}\right)e^{-\left(\frac{n\pi\alpha}{L}\right)^{2}t}$$
Which we can turn into the general solution by summing all the values, getting:
$$u(x,t)=\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos\left(\frac{n\pi x}{L}\right)e^{-\left(\frac{n\pi\alpha}{L}\right)^{2}t}$$
#### Step 5 - Apply the Non-Homogeneous Initial Conditions
Our final step is to satisfy the initial condition:
$$u(x,0)=h(x)$$
Setting $t=0$ in the general solution we get:
$$h(x)=u(x,0)=\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos\left(\frac{n\pi x}{L}\right)$$
Which is just the Fourier half-range cosine series expansion of $h(x)$:
$$a_{n}=\frac{2}{L}\int_{0}^{L}h(x)\cos\left(\frac{n\pi x}{L}\right)~dx$$
So the general solution is:
$$u(x,t)=\frac{a_{0}}{2}+\sum\limits_{n=1}^{\infty}a_{n}\cos\left(\frac{n\pi x}{L}\right)e^{-\left(\frac{n\pi\alpha}{L}\right)^{2}t}$$
With the $a_n$ coefficients being given by the equation above.
