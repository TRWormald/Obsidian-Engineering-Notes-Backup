We can check the stability of our scheme by applying Fourier stability analysis, also known as Von Neumann stability analysis.
![[Pasted image 20251030173209.png|centre]]
#### Step 1 - Write Our Numerical Solution as a Fourier Series
We know that a particular set of Fourier modes are exact solutions of our equation. Hence, a similar Fourier mode should be an exact solution of our FDA. Suppose we say, for a particular value of $k$ and $w$,
$$u(x,t)=ae^{j(kx+\omega t)}$$
Where $j=\sqrt{-1}$, and $a$ is a constant, then:
$$\frac{\partial u}{\partial t}=aj\omega e^{j(kx+\omega t)}$$
$$\frac{\partial u}{\partial x}=ajk e^{j(kx+\omega t)}$$
Hence:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=a(\omega+ck)je^{j(kx+\omega t)}$$
only if:
$$\omega=-kc$$
Of course we can superimpose an infinite number of these modes. We take:
$$k=m\pi$$
and then:
$$u(x,t)=\sum\limits^{+\infty}_{m=-\infty}a_{m}e^{j(m\pi x-m\pi ct)}$$
For our FDA we can then say:
$$u_{i}^{n}=\sum\limits^{+\infty}_{m=-\infty}a_{m}e^{j(m\pi i\Delta x-m\pi c n\Delta t)}$$
#### Step 2 - Define the Amplification Factor $\lambda$
Only one mode need be considered for a stability analysis. All other modes follow similarly. The relationship between $u_{i}^{n+1}$ and $u_{i}^{n}$ is of interest. Using the Fourier mode above:
$$u_{i}^{n}=a_{m}e^{j(m\pi i \Delta x-m\pi cn\Delta t)}=a_{m}e^{jm\pi i \Delta t}e^{-jm\pi cn\Delta t}$$
$$u_{i}^{n+1}=a_{m}e^{j(m\pi i \Delta x-m\pi c(n+1)\Delta t)}=a_{m}e^{jm\pi i \Delta t}e^{-jm\pi cn\Delta t}e^{-jm\pi cn\Delta t}$$
$$u_{i}^{n+1}=u_{i}^{n}e^{-jm\pi c\Delta t}$$
We say that:
$$u_{i}^{n+1}=\lambda^{m}u_{i}^{n}$$
Where $\lambda^{m}$ is called the **amplification factor**. Clearly this needs to be less than one or the Fourier mode will grow with time, and the FDA will be unstable.
#### Step 3 - Derive an Expression for the Amplification Factor
We then substitute the Fourier mode into our FDA relation and rearrange for $\lambda$. Inserting the Fourier mode into the FTCS update relation (drop $m$ superscript from $\lambda$ from hereon):
$$u_{i}^{n+1}=u_{i}^{n}-\frac{c\Delta t}{2\Delta x}u_{i+1}^{n}-u_{i-1}^{n}$$
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{2\Delta x}(a_{m}e^{jm\pi(i+1)\Delta x}e^{-jm\pi cn\Delta t}-a_{m}e^{jm\pi(i-1)\Delta x}e^{-jm\pi cn\Delta t})$$
Splitting the exponential terms and simplifying we obtain:
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{2\Delta x}u_{i}^{n}(e^{jm\pi \Delta x}-e^{-j m\pi \Delta x})$$
Remembering that:
$$e^{j\theta}=\cos\theta+j\sin\theta,~~~~~~~~e^{-j\theta}=\cos\theta-j\sin\theta$$
So:
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{2\Delta x}u_{i}^{n}2j\sin(m\pi\Delta x)$$
Dividing through by $u_{i}^{n}$ gives:
$$\lambda=1-\frac{c\Delta t}{\Delta x}j\sin(m\pi\Delta x)$$
#### Step 4 - Calculate the Magnitude of the Amplification Factor
$$\lambda=1-\frac{c\Delta t}{\Delta x}j\sin(m\pi\Delta x)$$
We only care about the magnitude of $\lambda$ not its phase, so we compute this as:
$$|\lambda|=\sqrt{1+\frac{c^{2}(\Delta t)^{2}}{(\Delta x)^{2}}\sin^{2}(m\pi\Delta x)}$$
Hence,
$$|\lambda|>1$$
for every mode except $m=0$, and so the FDA is unstable as disturbances are not damped, but grow exponentially. The amplification is the effective dissipation of the scheme. If $|\lambda|<1$ the dissipation coefficient can be thought of as positive, vice versa it is negative. Negative damping is clearly unstable.
#### Evaluation of the FTCS Scheme
We have therefore determined that despite the fact that the FTCS scheme is consistent, it is **always unstable**. Consistency and stability are the vital requirements. Order of accuracy is important, but not vital, it determines how small $\Delta x$ and $\Delta t$ have to be before the FDA solution $\rightarrow$ the real PDE solution.
So, can we find stable, consistent methods, even if they are of lower order accuracy?
#### Considering the Backward Spatial Difference
Lets again consider:
$$\frac{\partial u}{\partial t}+c\frac{\partial u}{\partial x}=0$$
As before we will take a first order temporal approximation:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n}=\frac{u_{i}^{n}-u_{i}^{n}}{\Delta x}+O(\Delta x)$$
but now lets consider the backwards spatial difference:
$$\left.\frac{\partial u}{\partial t}\right|_{i}^{n}=\frac{u_{i}^{n}-u_{i-1}^{n}}{\Delta x}+O(\Delta x)$$
And so:
$$\frac{u_{i}^{n+1}-u_{i}^{n} }{\Delta t}+\frac{c}{\Delta x}(u_{i}^{n}-u_{i-1}^{n})=0+O(\Delta x,\Delta t)$$
or, as $\Delta x,\Delta t\rightarrow 0$ the scheme is:
$$u_{i}^{n+1}=u_{i}^{n}-\frac{c\Delta t}{\Delta x}(u_{i}^{n}-u_{i-1}^{n})$$
Considering the truncation error it is clear that the scheme is first order accurate in both space and time, i.e. less accurate than the FTCS scheme. But is is consistent, is it stable?
We apply the same stability analysis as before:
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{\Delta x}(e^{jm\pi i\Delta x}e^{-jm\pi cn\Delta t}-e^{jm\pi (i-1)\Delta x}e^{-jm\pi cn\Delta t})$$
Which, after simplifying, give us:
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{\Delta x}u_{i}^{n}(1-e^{-jm\pi\Delta x})$$
$$\lambda u_{i}^{n}-u_{i}^{n}=-\frac{c\Delta t}{\Delta t}u_{i}^{n}(1-\cos(m\pi\Delta x)+j\sin(m\pi\Delta x))$$
We shall call:
$$\nu=\frac{c \Delta t}{\Delta x}$$
Then dividing through by $u_{i}^{n}$ leaves:
$$\lambda=1-\nu(1-\cos(m\pi \Delta x))-j\nu\sin(m\pi \Delta x)$$
Which gives:
$$|\lambda|^{2}=1-4\nu(1-\nu)\sin^{2}\left(\frac{1}{2}m\pi \Delta x\right)$$
From which we can clearly see that:
$$|\lambda|\le1$$
 for all modes (all m) so long as:
 $$0\le \frac{c\Delta t}{\Delta x}\le 1$$
 Hence, for $c<0$ the scheme is always unstable, and for $c>0$ we have the condition:
 $$\frac{c\Delta t}{\Delta x}\le 1$$
 which is a physical limit on the time step. This condition is of fundamental importance, and is known as the CFL condition.
### Things to Consider
1) Why is FTCS always unstable?
2) Why is one-sided backward difference stable for $c>0$, and unstable for $c<0$, and one sided forward difference stable for $c<0$, and unstable for $c>0$?
3) For stable one-sided difference, why is there a stability limit?
Lets consider the stencils for the three schemes considered so far, and the signal propagation in each.
![[Pasted image 20251030190703.png|centre]]
Hence, it is clearly physically incorrect to propagate information against the flow direction, and the stability analysis has shown this to be incorrect. The correct propagation of signals forms the basis of UPWIND methods. In these methods information may only propagate from "upwind" or "upstream", i.e. all information must travel with the local wave direction.
![[Pasted image 20251030191007.png|centre]]
