### Types of Loading
There are a few main ways that an aircraft can be loaded:
\
**Tensile Loads**
Tie bars and wire are very efficient ways of transmitting tensile loads, the latter however cannot transmit compression loads, whilst the former can - however they do have the advantage that the failure of a single strand doesn't result in the complete failure of the cable.
The main issues with structures loaded in tension are fracture and fatigue. Some high strength materials are very brittle which makes them undesirable for tension members if there is a risk of sudden catastrophic failure.
\
**Compression**
Stiffness is critical in compression members because of the risk of buckling. This depends on the material stiffness (see [[Buckling of Columns and Struts]]) and the structural stiffness related to shape (see the [[Second Moment of Area]])
The ideal member is a thin walled tube as it maximises the second moment of area for a given amount of material. However, if the ratio of radius to wall thickness is too large there is a risk of local wall buckling.
Fatigue is much less of a concern as cracks do not usually propagate under compression.
\
**Shear**
Shear involves a change in angle or shape - complementary shear forces are required to produce shear.
Simple shear causes bending - not pure shear
Shear can be carried by tensile and compressive members at 45 degrees. Panels are good at carrying shear by resisting shape change.
\
**Bending**
Bending can be carried by tensile and compressive members separated in space. An I beam approximates this, and is efficient for resisting bending. The web separates the flanges, and helps prevent bucking of the compression flange.
\
**Bending With Shear**
The web of an I-beam carries the shear that is not present in pure bending. A warren truss is an efficient arrangement for carrying bending within shear. Compression members need to be larger section than tension members to resist bucking. Ties can carry tension loads. But if the direction of loading reverses, all members need to be able to resist both tension and compression.
Diagonal cross-bracing can be used if both directions of loading need to be considered - two ties which only have to carry tension may be lighter than a single compression member.
\
**Torsion**
Torsion is a twisting moment acting about the axis of the structure. It is most effectively carried by shear forces around a closed structure. A box or tube within a continuous skin is very efficient. Alternatively the shear can be carried by cross braced members.
### Types of Airframe Construction
There are several different types of airframe types:
#### Frame with non-structural Covering
This can be seen in many early bi- and tri-planes:
![[Pasted image 20240423094627.png|center|400]]
In this configuration all loads are carried by the frame structure, with the skin assumed not to carry any load except air pressure. This could be used for early aircraft due to the fact that the aerodynamic loads were very low.
#### Monocoque
This is where there is a single skin with no supporting frame, so all loads have to be carried by the skin. True monocoque was problematic for large scale use due to problems with buckling.
![[Screenshot 2024-04-23 094852.png|center|450]]
Sandwich structures can be used without supporting members - this is where you have two layers of skin separated with a core material.
#### Stressed Skin
This is where you have a 'stressed' (loaded) skin supported by an internal frame. This is very much the classic arrangement for aircraft load carrying.
The load is divided by the skin and the stringers, with the stringers and frames (or ribs) dividing the skin into small panels to provide resistance to buckling.
![[Pasted image 20240423095536.png|center|250]]
#### Shear Resistant Structures
In this method stiffeners divide up panels to prevent buckling, however this can result in a heavy design in some cases.
It is important to consider the different circumstances of each case and to choose the correct loading type for each - as the same method that might work well for a high AR wing might not work as well for a low one.
#### Tension Field Structures
When the panels buckle in this configuration they carry diagonal tension only - the 'diagonal tension field'
![[Pasted image 20240423100042.png|center|300]]
Stiffeners carry compressive loads - this is generally more efficient for thin skin structures.
Effectively what is happening here is the panels are being allowed to buckle deliberately and they then act as a tensile connector effectively creating a pseudo-truss structure as they carry the required tensile loads to hold the structure in place.
### Functions of basic structural members in a stressed skin construction
#### Skin
The skin carries tensile loads as well as compressive loads - however the effectiveness depends on the level of stiffening.
It also carries shear loads associated with bending and torsion.
It also provides a smooth aerodynamic surface as well as a sealed enclosure.
#### Stringers
These are the stiffening members within the wing. They carry tensile and compressive loads; add stiffness to the skin to enable it to resist bucking and carry higher compressive stresses. They also provide bending stiffness to resist distortion of skin due to local loads and divide up the skin into small panels to reduce bucking due to shear and/or compression.
#### Frames and Ribs
Frames are normally associated with the fuselage structure whilst Ribs are normally associated with the wing or box structure.
They are used to:
- Support stringers against compressive buckling
- To divide the skin into panels to reduce shear buckling
- To distribute discrete loads into the rest of the structure
- To maintain cross-sectional shape
### Fuselage Structures Loading
#### Loading in Level Flight
For simple illustration lets assume:
- Uniform distribution of mass along the length
- Wings and tail loads act at single points
- Thrust and drag are ignored
This leads to:
![[Pasted image 20240423101119.png|center|400]]
#### Loading in Symmetric Manoeuvre
A simple manoeuvre such as steady pull out from a dive gives the same basic type of loading. However the aerodynamic forces are higher, causing an upwards acceleration. **For steady state conditions this can be treated statically by applying inertia loads in the opposite direction. These are the normal loads due to weight multiplied by the load factor.** (See [[Manoeuvring Flight#Load Factor|here]] for more information about the load factor, and [[Airframe Loads#Aerodynamic and Inertia Loads|here]] for the typical load factor limits for various aircraft)
This results in:
![[Pasted image 20240423101557.png|center|400]]
From this you can calculate the shear force and bending moment diagrams for the aircraft.
#### Calculating the Fuselage Stresses and Deflections
##### Calculating Stresses
Once we calculate the shear forces and bending moments we can calculate the fuselage stresses and deflections.
For an aircraft's skin which has been stiffened using stringers we have to estimate the second moment of area, this can be done by calculating the equivalent thickness of a hollow tube of the same radius, without the stringers:
$$t_{e}=t\cdot \frac{A_{t}}{A_{s}}$$
Where $t$ is the initial thickness of the skin, $A_{t}$ is the total area of the cross section, and $A_{s}$ is the area of the skin.
This equivalent thickness can then be used in the equation for finding the [[Second Moment of Area]] of a thin walled tube:
$$I_{xx}=I_{yy}=\pi r^{3}t_{e},~~~~t<<r$$
The bending stress can therefore be calculated to be:
$$\sigma=\frac{My}{I}$$
Where $y=r$ (see more about this in [[Longitudinal Stresses in Beams#The Euler-Bernoulli Beam Theory|the Euler-Bernoulli Beam Theory]])
##### Calculating Deflections
We can now calculate the vertical deflections, but first we need to determine where our datum will be. The most logical place to put it is at the wing connection point as there will be zero displacement and rotation there.
If we consider the force diagram for the airframe:
![[Pasted image 20240423101557.png|center|400]]
We can see that forwards of the datum there is a simple distributed load, and aft of the datum there is a distributed load with an end load.
Hence we can use the formulae for a cantilever beam with an end load and a cantilever beam with a distributed load (see [[Deflections in Beams#Deflection Formulae]]):
$$\delta_{end~load}=\frac{PL^{3}}{3EI}$$
$$\delta_{distributed}=\frac{wL^{4}}{8EI}$$
Hence for the nose the deflection is just $\delta_{distributed}$ whilst for the tail it is $\delta_{end~load}+\delta_{distributed}$ due to the principle of [[Deflections in Beams#Superposition|superposition]].
#### Loading in Gusts
Symmetric gusts can be treated in a similar way to manoeuvre loading by using an appropriate load factor. Both positive (up) and negative (down) gusts have to be considered. However positive gusts are generally more critical because they add to the 1g level flight loading.
#### Loading During Landing
You have to consider various different cases due to the different ways aircraft might land. For example for an aircraft with a nose and two main undercarriages:
- Three point landing
- Tail down landing
- Touchdown on one wheel/bogie
There is also significant fore-aft loading which arises due to:
- Braking
- Attitude of the aircraft in tail down landing
#### Unbalanced Pitching Moments
For cases where there are net pitching moments on the aircraft, the inertia loading also includes a rotational acceleration about the centre of gravity. In such cases the load factor n is no longer constant. It varies linearly with distance from the centre of gravity.
#### Loading in Asymmetric Cases
This occurs when a gust is not uniform across the entire aircraft, take for example this case with a lateral gust on the tailfin of the aircraft:
![[Pasted image 20240423110123.png|center|400]]
##### Calculating Stresses in an Asymmetric Case
First we need to calculate the torque generated:
$$T=Fd$$
We then need to find the [[Polar Second Moment of Area]] of area for a thin walled cylinder:
$$J=2\pi r^{3}t$$
The shear stress on the fuselage skin can therefore be calculated using:
$$\frac{T}{J}=\tau/r$$
See [[Torsion of Shafts]] for more information about torsion, however we are using a thin walled cylinder rather than a solid one.
We can then use:
$$\frac{T}{J}=\frac{G\phi}{L}$$
To find $\phi$ and hence find our deflection simply using:
$$\phi r=d$$
**Note that this equation only gives the deflection due to the torsion of the fuselage, the tailfin will also experience bending due to the gust which would result in a greater deflection.**
#### Loading Due to Cabin Pressurisation
The pressure inside the cabin obviously results in stress due to the pressure differential:
![[Pasted image 20240423111416.png|center|400]]
We can calculate the two stresses in the following ways:
$$\text{Hoop Stress}=\sigma_{hoop}=\frac{Pr}{t}$$
$$\text{Axial Stress}=\sigma_{axial}=\frac{Pr}{2}\cdot t_e$$
