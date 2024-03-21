The method for numerically solving systems of equations is similar to solving a single equation (obviously) however it requires many more steps.
Given a general set of differential equations:
$$\frac{dx}{dt}=-\lambda xy$$
$$\frac{dy}{dt}=\lambda xy-\gamma y$$
$$\frac{dz}{dt}=\gamma y$$
Where $x(0)=x_{0}$, $y(0)=y_{0}$, and $z(0)=z_{0}$.
We can calculate that:
$$\begin{align*}
x(t+h)=x_{n+1}&= x(t)+h\times-\lambda~x(t)~y(t)\\
&= x_{n}+h\times-\lambda ~x_{n}~y_{n}
\end{align*}$$
$$\begin{align*}
y(t+h)=y_{n+1}&= y(t)+h\times(\lambda ~x(t)~y(t)-\gamma~ y(t))\\
&= y_{n}+h\times(\lambda x_{n}~y_{n}-\gamma~y_{n})
\end{align*}$$
$$\begin{align*}
z(t+h)=z_{n+1}&= z(t)+h\times\gamma ~y(t)\\
&= z_{n}+h\times\gamma~y_{n}
\end{align*}$$
We therefore need to iterate through each of these equations to solve the system.

