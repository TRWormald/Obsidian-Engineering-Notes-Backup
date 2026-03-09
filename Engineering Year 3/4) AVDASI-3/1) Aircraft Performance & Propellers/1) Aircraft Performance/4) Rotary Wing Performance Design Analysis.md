### Rotary Wing Design Requirements
- General requirements
	- Payload
	- Speed
	- Range
	- Altitude
	- Cost
- Key mission requirements
	- Transportation
	- Firefighting
	- Training
	- Surveillance
	- Military
- Compliance with standards
- Inoperable engine requirements
	- Urban area
	- Traffic controlled area

### Simplistic View of Performance Model
![[Pasted image 20260309110011.png|centre]]
### Typical Helicopter Mission
![[Pasted image 20260309110033.png]]
### Considerations in Helicopter Design

| General                                          | Rotors                             | Mission Performance                                               | Drive Train                                                                                   |
| ------------------------------------------------ | ---------------------------------- | ----------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Is the aircraft the correct size to do the task? | Disc loading & blade loading       | Is the empty mass fraction achievable?                            | What engines are available and how many do I need?                                            |
|                                                  | Growth potential                   | Is there sufficient space allowance for the required fuel volume? | Engine power lapses with altitude and temperature                                             |
|                                                  | Noise                              | Has all the necessary role equipment been accounted for?          | Installation losses typically 5-10%                                                           |
|                                                  | Maximum length with rotors turning | Mission fuel = Trip fuel + Reserve fuel                           | What transmission limits do I need and can these be achieved within the allotted mass budget? |
|                                                  | Flight envelope                    |                                                                   |                                                                                               |
### Initial Sizing and Power Model Calculations
![[Pasted image 20260309110818.png|centre]]
#### Helicopter Mass Breakdown
![[Pasted image 20260309110840.png|centre|445]]![[Pasted image 20260309110900.png|459]]
#### Initial Sizing
![[Pasted image 20260309111006.png|centre]]
#### Rotor Design Process
The design process for a rotor is always iterative, but there is a general order to the definition of the rotor parameters and the various analyses required to select them:
- Rotor Diameter
- Rotor Tip Speed
- Total Rotor Blade Area
- Number of Blades - and hence Blade Chord
And then subsequently:
- Blade Mass
- Blade Flap Stiffness
- Blade Mode Natural Frequencies
- Lag Damping

##### Rotor Sizing Overview
- Rotor diameter is primarily defined to optimise hover performance
- Rotor tip speed is defined on the basis of providing the requisite rotor performance and providing acceptable noise levels and Mach number limits
- The selection of blade aerodynamic technology will influence the required total blade area
- Blade area is to be defined on the basis of achieving a forward flight envelope to meet specification requirements. This defines the parameter which is the product of blade chord and blade number.

##### Rotor Diameter
With an initial estimate of rotor area, rotor diameter is based on achieving the specified hover performance.
Blade radius can also be constrained by other limitations, e.g. fuselage length, transportation and stowage requirements, restricted landing zones, etc.
Relatively small rotor diameters will result in high Disc Loadings, wake velocities, and hover powers
Relatively large rotor diameters will require increased fuselage length (for adequate rotor separation) and hence higher aircraft weight.
##### Rotor Tip Speed
Rotor tip speed must be sufficiently high to provide the requisite rotor performance.
Rotor tip speed must be constrained to provide acceptable noise levels to meet certification requirements
Relatively low rotor speeds will:
- Increase rotor torque levels and will therefore penalise transmission design
- Require increased blade area (hence weight) to meet performance requirements
Relatively high rotor speeds will:
- Generate unacceptable noise levels
- Result in unacceptably high Mach Numbers at high speed conditions on the advancing blade tip
![[Pasted image 20260309113707.png|329]]
##### Rotor Blade Area
The total blade area is defined on the basis of achieving the required thrust and forward speed envelope.
The blade loading $C_{w}/s$ is defined as:
$$C_{w}/s=\frac{T}{0.5 \rho Nc R(\Omega R)^{2}}$$
A range of blade aerodynamic technologies are available:
- A low level aerodynamic technology will result in increased blade area, drag and weight.
- Beware that an advanced aerodynamic technology may lead to inadequate blade area and hence rotational inertial for auto-rotation purposes.
![[Pasted image 20260309113955.png|507]]
##### Rotor Blade Technology
![[Pasted image 20260309114012.png|488]]

##### Blade Number vs Blade Chord
