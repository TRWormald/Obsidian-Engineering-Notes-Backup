### Measurement of Fracture Toughness
Materials are more susceptible to fracture by normal stresses than shear.
#### Test Configurations
![[Pasted image 20251023111528.png|centre|400]]
![[Pasted image 20251023111610.png|centre|400]]
![[Pasted image 20251023111626.png|centre|400]]
![[Pasted image 20251023111641.png|centre|400]]
#### Measuring the Mode I Fracture Toughness
The critical stress intensity factor required to extend the crack under an opening mode is called the Mode I fracture toughness $K_{Ic}$. But measured fracture toughness can depend on sample size, so we need to improve control of the test dimensions.
![[Pasted image 20251023111826.png|centre]]
Specimens having standard proportions but which are different in absolute size produce different values for $K_{c}$. The stress states depend on the specimen thickness (B) until the thickness exceeds some critical dimension.
One thickness exceeds the critical dimension, the value of $K_{c}$ becomes relatively constant, which is regarded as the true material property called the plane-strain fracture toughness $K_{Ic}$.
But why does this happen? Its because of constraint.

When a crack is loaded the stress increases exponentially. However a material will yield before the stress reaches this singularity. The yield region is known as the Plastic Zone. It is clear that this region depends on the nature of the stress ahead of the crack. Plane stress $r_{p}\approx$ 3x Plane Strain $r_{p}$
![[Pasted image 20251023112519.png|centre]]
#### Plane Stress
For thin sheets there is no stress in the thickness direction, i.e. $\sigma_{zz}=0$. This stress state is known as Plane Stress. However there is still a $\varepsilon_{zz}$ which results in a bi-axial stress state such that the material fractures in a characteristic ductile manner, with a 45 degree shear lip being formed at each free surface. The plastic zone radius can be approximated:
$$r_{p}=\frac{1}{2\pi} \left(\frac{K_{c}}{\sigma_{y}}\right)^{2}$$
#### Plane Strain
For a thick material the stress in the thickness direction becomes significant. i.e. there's a tri-axial stress state.
With the thickness contraction effectively being zero.
This stress state is known as Plane Strain.
And the Plastic zone radius can be approximated as:
$$r_{p}=\frac{1}{6\pi }\left(\frac{K_{Ic}}{\sigma_{y}}\right)^{2}$$
![[Pasted image 20251023112930.png|centre]]
### Shear Lips
As the crack approaches the surface it tends to run out into a shear lip. For small samples, the shear lips are the dominant failure mechanism, whilst at the thickest sample size the contribution of the shear lips is trivial and we have a valid measurement of the plane strain fracture toughness:
![[Pasted image 20251023113057.png|centre]]
### Mode 1 Fracture Toughness ASTM Standard
![[Pasted image 20251023113235.png|centre]]
![[Pasted image 20251023113504.png|centre]]
### LEFM Validity
![[Pasted image 20251023113256.png|centre]]
### Factors that Influence Fracture Toughness
Extrinsic and Intrinsic Toughness Mechanisms:
![[Pasted image 20251023113619.png|centre]]
Extrinsic toughness mechanisms are placed behind the crack tip to impede the crack advance, whilst intrinsic toughening mechanisms are ahead of the crack tip which typically are extra fractures that occur in the plastic zone which don't directly contribute to the original crack.
This is relevant as our equations assume that everything is broken behind the crack whereas in actual fact some fibres or parts of the grain may still be connected. 