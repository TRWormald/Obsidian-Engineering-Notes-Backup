### What will we cover?
Now we are going to look at:
- Supercritical Aerofoils for Transonic Flow
- 3D Compressible Flows, in particular at:
	- The effect of wing sweep
	- Wing Characteristics
	- The Area Rule
### The Supercritical Aerofoil
The aim of the supercritical aerofoil is to delay drag divergence by weakening upper surface shockwaves. A supercritical aerofoil has an:
![[Pasted image 20250407151113.png|centre]]
Note how in the graph in the bottom left the critical Mach number for the supercritical aerofoil doesn't occur  until M=0.8.
### Wing Sweep - Basic Effect
Transonic and supersonic design is characterised by wing sweep. It allows us to increase $M_{crit}$ and hence the drag divergence Mach number.
We can lower drag by a factor of 2 to 3 using wing sweep.
![[Pasted image 20250407151341.png|centre]]
There are two main effects of wing sweep:
1) Reduced effective Mach Number $M_{LE}$
2) Reduced effective thickness $t/c$
And since Prandtl-Glauert correction and critical pressure coefficient curves scale with $M_{LE}$ not $M_{\infty}$ we can see pretty drastic results:
![[Pasted image 20250407151537.png|centre]]
We see reduced press increase with $\Delta$ (wins sweep angle) and hence reduced compressible suction peak $C_{p_{min}}$. The result of which is an increased $M_{crit}$.
### The Effect of Sweep on Subsonic Wings
For transonic flow, drag rise is delayed and reduced by sweep, but when the Leading Edge Mach number is supersonic, the wave drag is increased by sweep.
We can consider the Prandtl-Glauert correction as a transformation to an "equivalent" incompressible flow. The aspect ratio of the wing is reduced and sweep increased with increasing $M$. This results in:
- The lift curve slope reducing
- No effect on the induced drag factor $k$.
### Supersonic Swept Wing Considerations
Interaction of aircraft components is limited by the Mach cone, which is very important for the control of the aircraft.
Leading edge sweep is very important:
- Supersonic leading edges generate bow shocks
- Subsonic leading edges give lower wave drag and we can also use subsonic aerofoil sections.
![[Pasted image 20250407170409.png|centre]]
In the image above (top, right) we can see how we go from having 2D supersonic flow, to having 3D flow at the tips of the wing, this can result in unpredictable behaviour. We can see how this is rectified on the F-15:
![[Pasted image 20250407171209.png|centre]]
The wing tips (as well as that of the tailplane) have been clipped to avoid this 3D flow.
### Zero Lift Drag
At zero lift the drag is made up from: skin friction on the surface, wave drag due to thickness distribution, and "base drag" due to afterbody separation. Below are some experimental results:
![[Pasted image 20250407171422.png]]Note how the "waisted" example produces less drag than the bulged example up to M=1.08.
This is because of the "Area Rule"
### The Transonic Area Rule
Drag rise is a function of the rate of change of the longitudinal distribution of cross-sectional area. We therefore need to aim to match the distribution of "minimum drag" - the Sears-Haak body.
![[Pasted image 20250407171928.png|centre]]
We have a boundary (the total equivalent area line) that we need to be under to minimise the drag. We sum all the contributions and they need to be as close to it as possible.
**Note** that in supersonic flow, it is the area distribution along the Mach cone that matters, not the flow axis.
#### An Understanding of the Area Rule
In 2D, streamlines form the edges of con-di nozzles. We hope that none of these nozzles choke as then a shock will occur (transonic case). A good area distribution achieves this.

In 3D we have streamtube, but the same argument holds. However tubes are bounded by the rest of the air - so how much the tubes are squeezed depends on the cross-sectional area of the body.
Recalling from earlier:
![[Pasted image 20250407175304.png|centre]]
This means that streamtube around the aircraft interact rather strongly, which means that if one is displaced outwards by a small change in the cross sectional area of the aircraft, this effect propagates a long way, and has quite a large influence.