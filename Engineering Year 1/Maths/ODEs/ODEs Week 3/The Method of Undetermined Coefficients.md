From the [[Solution Structure for Nonhomogeneous ODEs]] we know that, for a nonhomogeneous ODE, the general solution takes the form:
$$x=x_c+x_p$$
Where $x_c$ is the complementary function (found by solving the ODE as if it were homogenous) and $x_p$ is the particular integral.
\
Finding $x_p$ can be difficult, especially if we are working on pure guesswork so we use [[The Method of Undetermined Coefficients]] to help us.
The method is as follows:
1) Use homogeneous techniques to find the complementary function $x_c(t)$
2) Guess the particular integral $x_p(t)$ in terms of unknown coefficients (Ansatz)
3) Substitute the guess into the ODE and solve for the coefficients
4) The general solution is $x_c(t)+x_p(t)$
\
The theorem for this method is as follows, consider a nonhomogeneous linear ODE with **constant coefficients**:
$$a_n\frac{d^nx}{dt^n}+a_{n-1}\frac{d^{n-1}x}{dt^{n-1}}+\cdot\cdot\cdot+a_1\frac{dx}{dt}+a_0x=f(t)$$
If $f(t)$ has a finite chain of derivatives then we can use the **method of undetermined coefficients** to find a particular integral. In most cases $x_p=\alpha f_1(t)+\beta f_2(t)+...$ where $f_1,~f_2,...$ are chosen so that $f$ and all its derivatives can also be written as $C_1f_1(t)+C_2f_2(t)+...$
\
Note that a function has a finite chain of derivative if and only it it can be constructed by adding and multiplying exponential, cos, sin, and polynomial functions.
So:
$$x=e^{2t} \Rightarrow x'=2e^{2t}\Rightarrow x''=4e^{2t}\Rightarrow ~...$$
Is a chain of derivatives, note that all of the derivatives are in the form $C_1e^{2t}$ (this is what you would use in the method of undetermined coefficients)
\
The following table can be useful for choosing the correct function to solve using [[The Method of Undetermined Coefficients]]:
![[Pasted image 20240303131810.png]]
**Note that the above table is NOT GIVEN on the formula sheet and therefore must be revised!**



