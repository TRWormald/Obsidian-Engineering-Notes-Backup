Modern civil aircraft use electrical power for a wide variety of tasks and have a correspondingly higher demand. They feature multiple generators and system voltages, and are architected to provide redundancy in case of individual component failure. A typical system includes a 3 phase 115V AC system for high power loads and a back-up system based around a 28V DC supply.
\
In an AC system the polarity of both the current and the potential are bi-polar and time varying, normally sinusoidally. RMS (root mean square) quantities are used to simplify calculations. V and I are related by the impedance Z.
See [[AC Power]] for more information.
\
#### Single Phase vs Multi-Phase AC
In AC single phase we have a single live, neutral, and earth terminal.
![[Pasted image 20240318100601.png]]
Three Phase AC systems feature phase voltages displaced by $120\degree$. Most higher power systems are 3 phase AC.  
![[Pasted image 20240318100720.png]]
The advantages of three phase AC are as follows:
- At any point in time the sum of the three sine waves is zero. So in a balanced three phase system there is no neutral current (so there doesn't need to be a neutral return wire.)
- Three out of phase currents generate a rotating magnetic field, which simplifies the design of electric motors, as no starting circuit is required.
- The current is transmitted with only three connectors instead of six, because the return lines for each phase are not necessary, this halves the path covered by the flow of electrons, and thus the resistance, which is half with respect to a mono-phase system.
#### Key Terminology
**Rectification** - This is the process of going from AC to DC and can be carried out mechanically or electrically (with passive or active components)
**Inversion** - This is the process of going from DC to AC and is complex to achieve with mechanical components.
#### Aircraft Electrical Power Sources
There are several different forms of power sources on modern aircraft:
- **Generators**
These are the primary sources of electrical power on aircraft - they are driven by the aircraft engine (in light aircraft the system for converting the mechanical power to electrical power might be quite simple and produces a low voltage, whilst on a larger aircraft it involves auxiliary gearboxes with multiple generators converting into multiphase AC)
- **Batteries**
These are batteries - there's not much else to say about them. There are two main types: primary (non-rechargeable) cells, and secondary (rechargeable) cells.
- **APU (Auxiliary Power Unit)**
This is a small gas turbine that is used to start the engines, and provides backup for the hydraulic pneumatic and electrical power systems. It is started via the batteries.
- **RAT (Ram Air Turbine)**
This is an emergency air driven generator that is dropped into the air stream of a moving aircraft when other systems have failed. It will provide hydraulic as well as electrical power in the case of a failure of both the engine driven generators and the APU.
- **Ground Power**
This is where the aircraft is 'plugged in' to a generator on the ground meaning that it doesn't need to use any of its fuel/the energy stored in its batteries.
#### Fixed or Variable Frequency
Aircraft engines operate at variable speeds, so a generator attached to them will have variable output frequency.
This is not a problem where the output is rectified immediately.
However with an AC distribution system this can cause the frequency to vary resulting in problems with some loads which require a fixed frequency.
A way to fix this is to drive the generator through a constant speed gearbox.