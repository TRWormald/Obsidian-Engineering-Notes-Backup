We can use the integrating factor to solve first-order linear nonhomogeneous differential equations without constant coefficients.
This is done by leveraging the product rule, take for example the general ODE below:
$$a_1(t)\frac{dx}{dt}+a_0(t)x=f(t)$$
We can solve this by multiplying by a function of t so that the LHS looks like the product rule:
$$a_1(t)g(t)\frac{dx}{dt}+a_0(t)g(t)x=f(t)g(t)$$
Where $a_0(t)g(t)=\frac{d}{dt}a_1(t)g(t)$, meaning that by applying the product rule ($\frac{d}{dx}uv=u\frac{dv}{dx}+v\frac{du}{dx}$):
$$a_1(t)g(t)\cdot x =\frac{d}{dt}f(t)g(t)$$
We would then integrate this after rearranging both sides and then solve for $x$.
## The Theorem
A general 1st order ODE can be written in the form:
$$\frac{dx}{dt}+p(t)x=q(t)$$
for some functions $p(t)$ and $q(t)$. The function $I(t)=e^{\int p(t)\cdot dt}$ is an integrating factor. The integrating factor satisfies $I'(t)=p(t)I(t)$ $ since:
$$I'(t)=(e^{\int p(t)\cdot dt})'=\left(\int p(t)\cdot dt\right)'\cdot e^{\int p(t)\cdot dt}=I(t)p(t)$$
Multiplying the ODE by $I(t)$ leads to the general solution:
$$I(t)\frac{dx}{dt}+p(t)I(t)x=I(t)q(t)\Rightarrow \frac{d}{dt}(I(t)x)=I(t)q(t)$$
$$I(t)x=\int I(t)q(t)dt+C\Rightarrow x=\frac{1}{e^{\int p(t)dt}}\left(\int e^{\int p(t)dt}q(t)dt+C\right)$$
