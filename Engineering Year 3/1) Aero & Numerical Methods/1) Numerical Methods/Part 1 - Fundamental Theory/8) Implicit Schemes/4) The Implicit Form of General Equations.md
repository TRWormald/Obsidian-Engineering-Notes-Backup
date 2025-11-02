General equations are written in the form:
$$\frac{\partial u}{\partial t}+\frac{\partial F(u)}{\partial x}=0$$
This is then approximated implicitly by:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n+1}+\left.\frac{\partial F(u)}{\partial x}\right|_{i}^{n+1}=0$$
Consider the implicit BTCS scheme for the general equation:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{2\Delta x}(F(u_{i+1}^{n+1})-F(u_{i-1}^{n+1}))$$
Which is normally written as:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{2\Delta x}(F_{i+1}^{n+1}-F_{i-1}^{n+1})$$
So the problem now is, how do we approximate the flux function $F^{n+1}$? The most common method is to use a Taylor series expansion for $F$ about the $n-th$ time level:
$$F_{i}^{n+1}=F_{i}^{n}+\Delta t\left.\frac{\partial F}{\partial t}\right|_{i}^{n}+O(\Delta t^{2})$$
But to make this more useful we use:
$$\left.\frac{\partial F}{\partial t}\right|_{i}^{n}=\left.\frac{\partial F}{\partial u}\right|_{i}^{n}\left.\frac{\partial u}{\partial t}\right|_{i}^{n}$$
Using the standard approximation:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n}=\frac{u_{i}^{n+1}-u_{i}^{n}}{\Delta t}$$
and
$$\Delta u_{i}^{n}=u_{i}^{n+1}-u_{i}^{n}$$
we have:
$$F_{i}^{n+1}=F_{i}^{n}+\Delta t\left.\frac{\partial F}{\partial u}\right|_{i}^{n}\frac{\Delta u_{i}^{n}}{\Delta t}+O(\Delta t^{2})$$
or:
$$F_{i}^{n+1}=F_{i}^{n}+\Delta u_{i}^{n}\left.\frac{\partial F}{\partial u}\right|_{i}^{n}+O(\Delta t^{2})$$
Replacing this in the scheme gives $\Delta u_{i}^{n}$ as the unknowns in a tri-diagonal matrix equation. The term \frac{\partial F}{\partial u} is the Jacobian.
$$J_{i}^{n}=\left.\frac{\partial F}{\partial u}\right|_{i}^{n}$$
The scheme for each point is:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{2\Delta x}(F_{i+1}^{n+1}-F_{i-1}^{n+1})$$
Which becomes:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{\Delta t}{2\Delta x}(F_{i+1}^{n+1}+J_{i+1}^{n}\Delta u_{i+1}^{n}-F_{i-1}^{n+1}-J_{i-1}^{n}\Delta u_{i-1}^{n})$$
