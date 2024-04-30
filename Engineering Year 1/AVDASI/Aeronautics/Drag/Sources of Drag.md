### Drag Breakdown
There are two underlying sources of drag:
1) **Skin friction drag**
	- Sometimes called **surface friction drag**
	- It is the streamwise component of the tangential stresses acting at the surface
	- It is a direct result of the fluid viscosity
2) **Pressure Drag**
	- The streamwise component of pressure forces acting **normal** to the surface
	- It consists of:
	a) **Form Drag** due to **Boundary Layer** growth
	b) **Induced Drag** due to the formation of trailing vortex systems at the wingtips
	c) **Wave drag** due to shock formation at high speeds
![[Screenshot 2024-04-29 143450.png|center]]
### Skin Friction Drag
This occurs when the aerofoil drags air along with it:
![[Pasted image 20240429144513.png|center|400]]
Tangential shear stress on the surface opposes the aircraft's motion.
Friction causes the flow very close to the surface to slow down, forming a boundary layer which grows downstream. This results in the shape of the body changing as the flow is displaced outwards, and also leads to flow separation and the formation of a turbulent wake.
The friction drag coefficient reduces with Reynolds number and is greater for turbulent flow than laminar flow.
### Form Drag
Front to rear asymmetry in surface pressure distribution generates **Form Drag**; it is sometimes referred to as pressure drag. The form drag coefficient increases with increasing wake size.
![[Pasted image 20240429144843.png|center|300]]
![[Pasted image 20240429144859.png|center|300]]
### Profile Drag
Profile drag is the combination of Skin Friction and Form Drag:
$$\text{Profile Drag = Skin Friction Drag + Form Drag}$$
Low form drag and low skin friction drag tend not to go together:
- Form drag can be reduced by fairing off the aft part of the body
- But this increases the surface area and hence the skin friction drag.
\
As a result the minimum profile drag is often a compromise:
![[Pasted image 20240430100123.png|center]]
### Induced Drag
In 2D flow we only have profile drag, however in 3D flow we have an additional drag component that appears which is proportional to $\text{lift}^{2}$.
This is driven by pressure differences between the upper and lower surface of the wing - creating vortices.
The Wake Roll-Up diagram below shows how these vortices are formed:
![[Screenshot 2024-04-30 100509.png|center]]
#### Downwash
Tip vortices induce **downwash**, a downward flow component ($w$) over the wing span. This rotates the local velocity vector downwards by a small angle ($\varepsilon$) which reduces the AoA to $\alpha_{\text{eff}}$ and hence reduces lift to $L_{\text{eff}}$.
This means that the lift vector now has an induced drag component:
![[Screenshot 2024-04-30 101147.png|center]]
#### Span Efficiency
Induced incidence $\varepsilon$ is proportional to $C_{L}$ and therefore tip vortex strength is related directly to lift:
$$D_{i}=L\sin\varepsilon\approx L\varepsilon \Rightarrow C_{D_{i}}\approx C_{L}\varepsilon$$
Induced incidence also depends on wing aspect ratio (AR):
$$\varepsilon=\frac{C_{L}}{\pi AR}$$
So the closer the tips are together the greater the downwash.
Using this equation along with the approximation we get:
$$C_{D_{i}}=\frac{C_{L}^{2}}{\pi e AR}$$
Where $e\le 1$ and is equal to the **span efficiency factor**.
### The Drag Polar $C_D$ vs $C_L$
![[Pasted image 20240430102519.png|center]]
Before stall (in the 'well behaved region) $C_{D}\propto C_{L}^{2}$, so:
$$C_{D}=\underbrace{C_{D_{0}}}_{\text{Profile Drag}}+\underbrace{KC_{L}^{2}}_{\text{Indu}}$$