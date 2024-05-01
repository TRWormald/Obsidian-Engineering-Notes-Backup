A Payload-Range diagram allows you to visualise how the payload you carry affects the range you can fly. It helps airlines to define how they can use an aircraft and provides a better understanding of the utility of an airplane.
\
We first need to consider the [[Breguet Range - Jet#The Implications of our Assumptions#A more common notation for commercial aircraft is|range equation for commercial aircraft]]:
$$\boxed{R=\frac{a}{g\times tsfc}\left(M \frac{L}{D}\right)\ln\left(\frac{W_{initial}}{W_{final}}\right)}$$
So the range of an aircraft is a function of:
- Altitude through sound speed ($a$), and $tsfc$ (thrust specific fuel consumption)
- Engine efficiency, through $tsfc$
- Aerodynamic efficiency, through $M(L/D)$
- Structural efficiency through $(W_{initial}/W_{final})$
### Aircraft Weight
There are many components within the aircraft weight, it is not just a single number:
![[Aircraft Weight Breakdown.png|center]]
\
**Maximum Take-off Weight (MTOW)** - Maximum authorized weight for take-off due to strength and airworthiness requirements
**Operational Empty Weight (OEW)** - Basic weight of aircraft including all equipment and supplies needed for standard operation.
**Maximum Zero Fuel Weight (MZFW)** - Maximum weight allowed before fuel is loaded due to strength and airworthiness requirements.
$$W_{final}=OEW+Payload+Reserve~Fuel~Weight$$
$$W_{initial}=W_{final}+Trip~Fuel~Weight$$
Hence:
$$\frac{W_{initial}}{W_{final}}=\frac{W_{final}+Trip~Fuel~Weight}{OEW+Payload+Reserve~Fuel~Weight}$$
### Sample Payload-Range Diagram
![[Exemplar Payload-Weight Diagram.png|center]]
Note how as payload decreases the range increases, with the maximum range occurring with zero payload. Maximum payload is limited by MZFW. The bounded area represents the sum total of all possible combinations of payload and range.
### Generating A Payload-Range Diagram
The steps for generating a payload-range diagram are:
1) Finding the **maximum range given MZFW** - i.e. how far you can transport the maximum payload
	- So $W_{initial}=MTOW$
	- So $W_{final}=OEW+Reserve~Fuel+Payload$
2) Finding the **maximum range given maximum fuel**
	- So $Payload=MTOW-OEW-Max~Fuel$
	- Hence $W_{final}=MTOW-Max~Fuel$ 
3) Find the **maximum range given maximum fuel and no payload**
	- So $W_{initial}=OEW+Max~Fuel$
	- So $W_{final}=OEW$
	- $Payload=0$

This generates a diagram that looks like this:
![[Screenshot 2024-03-27 143715.png|center]]
Note how each line is defined by some maximum value (Max Payload, Trading Payload For Fuel, and Max Fuel Capacity).