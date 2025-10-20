When we were looking at [[5) The Horseshoe Vortex|horseshoe vortices]] we modelled the variation of the circulation along the span by superimposing them and varying the strength. In the original version of this method the bound vortices are coincident along the "lifting line" which is usually located at the quarter chord:
![[Pasted image 20250310190524.png|centre|centre]]
The result is a lifting line with bound circulation $\Gamma(y)$, varying with span.
![[Pasted image 20250310190609.png|centre]]
We can then superimpose an infinite number of vortices of infinitesimally different strengths to generate a continuous bound circulation with a semi-circular vorticity distribution.

### The Lifting Line Method
What is the purpose of the lifting line method?
>To obtain the values for the lift and drag on a 3D wing.

#### Step 1 - Determine the Downwash
Obtain an expression for the downwash velocity induced by the shed wake on the "bound vortex".
We can do this by extrapolating from the finite number of vortices, the shed wake vortex strength equals the change in the bound vortex strength.

In this limiting case, when the wake becomes a vortex sheet:
$$d\Gamma_{wake}=d\Gamma_{bound}=\left(\frac{d\Gamma_{bound}}{dy}\right)dy=\gamma_{x}(y)dy$$
Where $\gamma_{x}(y)$ is the wake vortex sheet strength.
*Note that the subscripts $wake$ and $bound$ are usually dropped.*
**Now we need to find the downwash velocity induced by the wake element at an arbitrary point on the bound vortex:**
![[Pasted image 20250316173549.png|centre]]
The Biot-Savart Law for a point level with the end of a semi-infinite vortex is used i.e. the magnitude of velocity $V$ is given by $V=\Gamma/(4\pi h)$
*Note:*
*The simple form of Biot-Savart for a line vortex filament tells us the magnitude of velocity induced, but not the direction.*
**We will have to work this out.**

In this case the velocity induced at $y_{0}$ by a filament at y with positive circulation will have magnitude:
$$V=\frac{d\Gamma}{4\pi(y_{0}-y)}$$
But it will be in a downwards direction (i.e. a downwash).
So the velocity in the $z$ direction, $dw$, is given by:
$$dw=\frac{-d\Gamma}{4\pi(y_{0}-y)}=\frac{-(d\Gamma/dy)dy}{4\pi(y_{0}-y)}$$
Integrating this gives the downwash induced by the entire vortex sheet - we will do this from tip to tip (so $y=-s$ to $s$):
$$\boxed{w(y_{0})=-\frac{1}{4\pi}\int_{-s}^{s}\frac{(d\Gamma/dy)dy}{(y_{0}-y)}}$$
Note that the velocity $w$ is positive upwards in the $z$ direction and so usually has a negative value (i.e. it acts downwards) for simple wing geometry where the whole of the wing experiences downwash.
#### The Relationship Between Downwash and Circulation
If the circulation distribution $\Gamma(y)$ were known then the corresponding downwash, lift $l(y)$ and drag $d(y)$ distributions could be worked out.

BUT in the equation both the circulation and downwash are unknowns so need more to determine circulation, downwash and hence lift and induced drag distributions i.e. a 3D equivalent of the Kutta condition.
#### Determining Circulation
The two simplest methods to determine circulation are:
1) Method 1 - Treat each chordwise wing section as if it were a 2D aerofoil (however this is limited to straight wings and high aspect ratio)
2) Method 2 - Apply the flow tangency condition at a control or collocation point on the chord line at each spanwise station - i.e. a 3D equivalent of the lumped vortex model (applicable to swept wings and low AR)
##### METHOD 1
Let us model a basic 2D aerofoil:
$$l=\rho_{\infty}V_{\infty}\Gamma, ~d=0$$
$$C_{L}=a_{0}(\alpha-\alpha_{l=0})$$
![[Pasted image 20250316175645.png|centre]]
For a section of a 3D wing the effective incidence is reduced by $\alpha_i$ due to the downwash velocity induced by the shed vortices, so the lift vector is rotated clockwise by $\alpha_{i}$ to give a resultant force $l_{eff}$.
![[Pasted image 20250316175811.png|centre]]
Thus there is reduced lift and also a drag component in 3D:
![[Pasted image 20250316175904.png|centre]]
Resolving the perpendicular and parallel to the actual rather than the free stream direction for small induced incidence the lift and drag forces are:
$$l=l_{eff}\cos\alpha_{i}\approx l_{eff}$$
$$d=l_{eff}\sin\alpha_{i}\approx l\alpha_{i}$$
Looking in more detail, for the wing the downwash velocity $w$ reduces the effective incidence by $\alpha_{i}$:
![[Pasted image 20250316180106.png|cenre]]
With the above being obtained when we make the usual small angle approximations.
Substituting the expressions for downwash velocity the local induced incidence at $y=y_0$ is:
$$a_{i}(y_{0})=\frac{-w(y_0)}{V_{\infty}}=\frac{1}{4\pi V_\infty}\int_{-s}^{s}\frac{(d\Gamma/dy)}{y_0-y}dy$$
And then using the 2D flow approximations for thin wings, the local lift coefficient is:
![[Pasted image 20250316180327.png|centre]]
And the Kutta-Joukowski theorem gives us another expression for the local lift coefficient:
![[Pasted image 20250316180407.png|centre]]
##### Spanwise Incidence Distribution
Equating the two expressions and substituting for the induced incidence gives the **Fundamental Lifting Line Equation**
$$\boxed{\boxed{\alpha(y_{0})=\frac{2\Gamma(y_{0})}{a_{0}(y_{0})V_{\infty}c(y_{0})}+\alpha_{l=0}(y_{0})+\frac{1}{4\pi V_{\infty}}\int_{-s}^{s}\frac{d\Gamma/dy}{y_{0}-y}dy}}$$
Noting that for thin aerofoil sections $a_0=2\pi$
For a known incidence and aerofoil shape the only unknown to be solved for is the circulation distribution.
##### Spanwise Lift Distribution
Assuming that we can solve this intergro-differential equation for $\Gamma(y_{0})$, the spanwise lift per unit span distribution is:
$$l(y_{0})=\rho_{\infty}V_{\infty}\Gamma(y_{0})$$
And hence the total lift is:
$$L=\rho_{\infty}V_{\infty}\int_{-s}^{s}\Gamma(y)~dy$$
With:
$$C_{L}=\frac{2}{V_{\infty} S}\int_{-s}^{s}\Gamma(y)~dy$$
#### Spanwise Drag Distribution
The corresponding spanwise drag per unit span distribution is:
$$d(y_{0})\approx l(y_{0}) \alpha_{i}(y_{0})$$
And hence the total induced drag is:
$$D=\rho V_{\infty}\int_{-s}^{s}\Gamma(y)\alpha_{i}(y)~dy$$
With:
$$C_{D_{i}}=\frac{2}{V_{\infty} S}\int_{-s}^{s}\Gamma(y)\alpha_{i}(y)~dy$$
#### Elliptical Circulation Distribution
An important special case is:
$$\Gamma(y)=\Gamma_{0}\sqrt{1-\left(\frac{y}{s}\right)^{2}}$$
The induced downwash is then:
![[Pasted image 20250316183608.png|centre]]
![[Pasted image 20250316183622.png|centre]]
So the downwash is constant and equal to:
$$\boxed{\boxed{w(\theta_{0})=\frac{-\Gamma_{0}}{4s}}}$$
If downwash is constant, then so is the induced incidence:
$$\alpha_i(\theta_{0})=-\frac{w(\theta_{0})}{V_{\infty}}=\frac{\Gamma_{0}}{4V_{\infty}s}$$
##### Total Lift for an Elliptical Distribution
![[Pasted image 20250316185200.png|centre]]
##### Total Induced Drag for an Elliptical Distribution
![[Pasted image 20250316185237.png|centre]]
#### What's so Special About an Elliptical Distribution?
A wing with an elliptical circulation or lift distribution has the minimum induced drag for a given lift coefficient and aspect ratio (see next week’s lecture for details). 
Designers try to achieve a lift distribution that is close to elliptic to minimise the induced drag via adjustments to the chord distribution, the twist distribution, and/or the angle of zero lift distribution.
#### Special Case Elliptical Lift Distribution on an Untwisted Wing
![[Pasted image 20250316185452.png|centre]]
![[Pasted image 20250316185509.png|centre]]
## Revision
![[Pasted image 20250316185525.png|centre]]
