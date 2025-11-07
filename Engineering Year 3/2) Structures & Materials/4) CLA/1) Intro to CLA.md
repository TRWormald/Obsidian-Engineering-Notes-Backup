>**Composite Materials**
>Composed of at least two materials, which combine to achieve enhanced properties and functionality

In Fibre Reinforced Polymer (FRP) composites, there is:
- Fibre Reinforcement - provides stiffness and strength
- Polymer Matrix - transfers load between fibres, provides toughness, and protects fibres

The advantages of using fibres in composites (and in general) is that it is very easy to identify whether there is material defects in them, as in the event of a fibre being compromised it will not stand up to any level of scrutiny. Think about the reasons for the use of wire-wound vs built up guns.

Common types of fibres used in FRP are:
- Carbon
- Glass
- Aramid
- Natural Fibres (like flax, or cactus!)

The matrix is typically some kind of polymer with a low stiffness (~5 GPa).

Laminates are composed of multiple plies of composite. These can be oriented in different directions to provide axial strength in the desired directions. i.e. composites can be tailored to a specific situation based on load requirements.

### Micro-Mechanics and Homogenisation
At a micro-mechanical scale the composite is heterogeneous (i.e. fibres and matrix), however at the macro-mechanical level the composite ply has homogeneous material properties.

>**Representative Volume Element (RVE)**
>The smallest volume over which the material properties are homogeneous.

The choice of RVE is informed by the composite microstructure, a larger RVE might capture random fibre distribution, manufacturing imperfections, voids, etc.

#### Continuous Fibre Composites
In a continuous fibre-reinforced composite we assume:
- Fibres are uniformly distributed and perfectly aligned
- Fibres and Matrix are linear-elastic and isotropic
- There is perfect bonding between fibres and the matrix
- Fibre and matrix stresses may be assumed constant along the fibre length

#### Fibre Volume Fraction
One of the key composite parameters is the fibre volume fraction $V_{f}$.
The upper bound is defined by fibre packing geometry. It is usually within the range:
$$0.3<V_{f}<0.8$$
#### Longitudinal Stiffness ($E_{11}$)
The strain in the matrix and fibres is the same:
$$\varepsilon_{11}=\varepsilon_{f}=\varepsilon_{m}$$
However the load taken is proportional to the stiffness.$$E_{11}=E_{f}V_{f}+E_{m}V_{m}=\sum\limits_{i=1}^{n}E_{i}V_{i}$$
#### Transverse Stiffness ($E_{22}$)
In a basic analysis of this case the stress in the fibres and the matrix are the same. However this assumption does not hold up to closer scrutiny, and predictions do not match experimental variation.
$$\frac{1}{E_{22}}=\frac{V_{f}}{E_{f}}+\frac{V_{m}}{E_{m}}$$
#### Shear Modulus ($G_{12}$) and Poisson's Ratio ($\nu_{12}$)