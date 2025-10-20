### Types of Failure
- Composite Failure
- Brittle Fracture Failure
- Fatigue Failure
	- Fracture by slow crack growth
	- Happens when the part is subjected to many repetitions of a stress below that for static crack growth
- Corrosion fatigue failure
	- Combined action of a cyclic stress and a corrosive environment
	- Fatigue resistance will decrease in the presence of an aggressive chemical environment
- Stress corrosion cracking
	- Similar to corrosion fatigue - combines mechanical and chemical failure processes
	- However in this case the stress is not cyclic
- Creep and stress rupture failure
	- A result of a static load applied over long periods of time

### Defining Fracture Terminology
#### [[Fracture Mechanics Lecture1 - Failure Of Materials.pdf#page=14|Elastic Strain Energy]]
Consider the bar in tension:
![[Pasted image 20250925112210.png|centre|250]]
When the bar is loaded you are putting energy into the system; this is the elastic strain energy ($U$).
This can be done through doing work, and is effectively energy conservation.
$$W-U=0$$
![[Pasted image 20250925112318.png|centre|250]]
$$U=\frac{1}{2}P\delta$$
#### Elastic Strain Energy Density
This is elastic strain energy per unit volume of material. On a stress strain plot, strain energy density is the area under the curve:
![[Pasted image 20250925112430.png|centre]]
$$U^{*}=\frac{1}{2}\sigma\varepsilon$$
The relationship between the input energy U and the strain energy density is:
![[Pasted image 20250925112538.png|centre]]
$$U=\frac{1}{2}P\delta =\frac{\sigma^{2}}{2E}V=U^{*}V$$
#### Toughness
We then continue loading until failure, where $F$ is the work expended in fracturing material over $da$. The energy dissipated per unit volume of the material up to failure is known as toughness:
$$\frac{d}{da}(W-U-F)=0$$
![[Pasted image 20250925112735.png|centre|250]]
![[Pasted image 20250925112802.png|centre|250]]
$$Uc^{*}=\frac{1}{2}\sigma \varepsilon$$
### Modes of Failure
### Brittle Material
![[Pasted image 20250925112852.png|centre]]
#### Ductile Material
![[Pasted image 20250925112936.png|centre]]
#### Ductile vs Brittle
Once failed, the area under the stress-strain curves indicates the level of energy dissipation of absorption per unit volume.
Brittle materials exhibit little or no plastic deformation and low energy dissipation or absoption.
Ductile materials exhibit extensive plastic deformation and high energy absorption.
Ductile materials produce a non-linear stress-strain response; toughness (strain energy density before failure) definition is still the same but strain energy is no longer the same past the elastic limit.

Once a material has plastically deformed, the elastic strain energy is the energy that is recovered when the material is unloaded.
he inelastic strain energy ($U_\text{inelastic}$) is the energy that is absorbed by the material through plastic deformation.
The elastic strain energy $U$ can drive the crack to grow.
![[Pasted image 20250925113328.png|centre|250]]
$$Uc^{*}=\int_{0}^{\varepsilon_{f}}\sigma d\varepsilon$$
$$U=\frac{1}{2}\sigma(\varepsilon-\varepsilon_{P})V$$
$$U_\text{inelastic}=Uc^{*}V-U$$
### [[Fracture Mechanics Lecture1 - Failure Of Materials.pdf#page=24|Fractography: The Study of Fracture Surfaces]]
![[Pasted image 20250925113556.png|centre]]
#### Brittle Fracture
![[Pasted image 20250925113618.png|centre]]
#### Atomic Bonds and Grain Boundaries
![[Pasted image 20250925113639.png|centre]]
#### Fractography in Metals
![[Pasted image 20250925113657.png|centre|250]]
Cleavage fracture is the breaking of atomic bonds along crystallographic planes (Trans-granular). This results in a rough and textured surface with river and feather patterns.
In some metal alloys cracks form along grain boundaries (Intergranular). This results in sharp and 3D faceted grains.
#### Brittle Fracture Surfaces
![[Pasted image 20250925113859.png|centre]]
#### Imperfections
Defects and flaws limit the potential elastic strain energy that can be stored by the material; however, extra deformation (strain) prior to failure would mean the material is tougher.
For example, dislocations in crystalline structure results in slip planes.
Extra energy is absorbed when the crystalline structure slides, this is what we refer to as plastic deformation.
#### Ductile Fracture
Under uniaxial tensile force in ductile materials:
- Necking caused by dislocation movements or polymer chain sliding
- Atomic debonding and microvoid formation
- These coalesce (join) to form larger cracks
- Eventually they propagate in the direction normal to the tensile axis.
Ductile fracture is much less critical in engineering. Failure can be detected beforehand due to observable plastic deformation.
For round coupons: a crack eventually propagates through the periphery along the shear plane at 45 degrees leaving the typical cup and cone pattern.
#### Microvoid Formation, Growth, and Coalescence
![[Pasted image 20250925115109.png]]
#### Micro-Void Shape
![[Pasted image 20250925115149.png|centre]]
