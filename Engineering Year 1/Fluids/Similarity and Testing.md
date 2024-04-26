### Equivalent Flows
For most real life scenarios we can create the same conditions using scale testing - which allows for cheaper and easier prototyping.
Below is an example:
\
*Consider an aircraft moving into still air at a speed* $V_{\text{aircraft}}$
*The upstream static pressure is equal to the atmospheric pressure:*
![[Pasted image 20240426104622.png|center]]
We can replicate this by imagining the aircraft stationary in a wind tunnel. The wind tunnel has steady onset flow of $V_{\text{aircraft}}$ and the inlet pressure is adjusted so that the static pressure of the onset flow is equal to atmospheric.
![[Pasted image 20240426104742.png|center]]
If the wind tunnel is large enough for the streamlines to be unaffected by the tunnel walls then the flow speed relative to the aircraft and the pressure would be identical in both cases.
This is due to us performing a [[The Galilean Transform|Galilean Transform]] on the first scenario to achieve the second.
**These are referred to as similar flows.**
\
However if the fluid starts from atmospheric pressure, when it is accelerated the static pressure will decrease - meaning that the pressure isn't the same in both cases - and if the pressures are different how can the speeds be the same.
This is usually ok as it is the pressure gradients that define the flow rather than the absolute values - so if the upstream static pressure isn't so different such that a change of state results, the relative flow speeds will be the same and change from upstream pressure will be the same.
### Flow Similarity
**Similar flows** produce the same force coefficients ($C_{p},C_{L},C_{D}$)
Two flows over different bodies are similar if:
- The streamlines are the same
- Values of flow quantities ($u,p,t$), are the same relative to some reference values throughout the flow field.
This requires that:
- Bodies are geometrically similar (but can be different sizes)
- The cross sectional area of the body is smaller compared to the wind tunnel

