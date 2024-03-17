### Aircraft Power Systems
A typical aircraft has three or four forms of power:
![[Screenshot 2024-03-11 144817.png|center]]
\
Aircraft, like cars, have gearboxes which transfer the shaft rotation in the engine into more useful forms of power - for example it might drive a hydraulic pump or an AC generator.
### Creating Pressure - Hydraulic Pumps
Hydraulic systems require pressure, these systems are used to move control surfaces/the undercarriage etc.
There are several types of pumps used:
#### Gear Pumps
Gear pumps are simple and reliable, they operate by meshing two gears in within a close tolerance housing. Oil in the space between the outside teeth is pumped from suction to discharge.
![[Pasted image 20240311145510.png|center|300]]
This type of pump can be noisy, so constant mesh patterns - like the herringbone - may be used.
#### Axial Piston Pumps
Axial piston pumps use a rotating swash plate to push pistons in and out. Check valves (which are one way) can direct fluid from the inlet to the outlet side.
The following diagram shows how these pumps work:
![[dp2.gif]]
The pump has two or more phases, in the simplest case when one piston is increasing the pressure of the fluid the other is regaining the fluid that it has pumped in. The check valves are spring loaded and the stiffness of these springs determines the increase in pressure as the compressed fluid will only be allowed through once sufficient force (pressure) is obtained.
**Note that this is only one way in which axial pumps work, there are also variants which rotate the piston block and align it with the inlet or outlet port at the correct timing of the piston stroke.**
### Hydraulic Actuators
Hydraulic cylinders allow us to easily produce linear motion:
![[hydraul1.gif]]
The above diagram is of a single action piston cylinder, a double action cylinder involves both sides of the piston head having fluid and the difference in pressure between the two sides (often caused by a reversal of flow direction) causing a force.
### Hydraulic Control
Hydraulic fluid is stored in a reservoir that feeds the pressure pump. Pressurised fluid is directed around the system using a series of valves - these can be mechanically or electrically signalled.
The fluid exiting the cylinder flows around a low pressure return back to the reservoir. **Volume flow is the same around the circuit.****
### Hydraulic System
High power density and instant response makes hydraulic systems particularly good for functions like moving flight control surfaces.
Most aircraft have three hydraulic systems for redundancy.
![[Pasted image 20240311152610.png|center|400]]
Hydraulic systems are reliable but are expensive to maintain as they are complex and require a high level of cleanliness. The fluid used on aircraft is highly corrosive to many materials.
Hydraulic systems are also quite heavy.
### Redundancy In Hydraulic Systems
Below is a diagram of a dual-tandem actuator, it is powered by two hydraulic systems which means that if one loses pressure there isn't complete actuator failure as the other takes over.
You can even have triple-tandem actuators (note that the tandem part of the name refers to the fact that both sides of the piston head are interfaced with hydraulics rather than being spring loaded as seen in the diagram in [[Hydraulic Systems#Hydraulic Actuators]])
![[Pasted image 20240311153007.png|center]]
\
In earlier aircraft, manual reversion (powering flight controls manually) was retained in case of hydraulic failures.
Some aircraft can also avoid the use of hydraulic controls through the use of servo tabs.