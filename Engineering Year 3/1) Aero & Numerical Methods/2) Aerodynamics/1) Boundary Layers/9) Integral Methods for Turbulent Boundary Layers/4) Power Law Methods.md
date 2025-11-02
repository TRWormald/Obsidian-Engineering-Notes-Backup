The simplest approximation is to assume a velocity profile.
From empirical data, it has been found that a power law gives a good approximation to a turbulent boundary later under zero pressure gradient.
I.e. we can scale the boundary layer with respect to local height $\delta$ through the boundary layer variable $\eta=\frac{y}{\delta}$.
The velocity ratio $U/U_{e}$ is a power of $\eta$.

Power Law Methods were developed from pipe flow results:
- Implicitly assumes velocity profile is similar
- Hence only really applicable to zero pressure gradient flows
- Has no theoretical underpinnings, i.e. is entirely empirical
The most common form is:
$$\frac{u}{u_{e}}=\eta ^{\frac{1}{n}}$$
Where n is characterised by the Reynolds number:
- $5\times10^{5}<Re<10^{7},~~n=7$
- $10^{6}<Re<10^{8},~~n=9$
### Power Law Methods - Thickness
![[Pasted image 20251020112310.png|centre]]
However, we have a problem with skin friction:
![[Pasted image 20251020112338.png|centre]]
For any value of n>1, the second term on the RHS above tends to 1/$\eta$, and hence as $\eta$ is zero at the wall, the skin friction is infinite!

Obviously this is a problem with our analysis, not real, and hence skin friction is approximated through empirical relations (both of type $c_{f}=K_{\delta}Re_{\delta}^{\frac{-2}{n+1}}$):
$$c_{f}=\frac{0.0468}{Re_{\delta}^{0.25}}~~for~n=7,~~~~~c_{f}=\frac{0.0290}{Re_{\delta}^{0.2}}~~for~n=9$$
### Use of the Momentum Integral Equation
The derivation of the MIE made no assumptions about the nature of the flow, so the MIE can be used for turbulent flows:
$$\frac{d\theta}{dx}+\frac{\theta}{u_{e}}\cancel{\frac{du_{e}}{dx}}(H+2)=\frac{c_{f}}{2}$$
So if we consider zero pressure gradient (i.e. no velocity gradients) the MIE becomes:
$$\frac{d\theta}{dx}=\frac{c_{f}}{2}$$
We can then solve for integral properties in the following manner:
![[Pasted image 20251020112850.png|centre]]
![[Pasted image 20251020112900.png|centre]]
