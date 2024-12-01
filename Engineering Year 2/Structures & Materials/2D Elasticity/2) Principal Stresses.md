![[Pasted image 20240929114152.png|centre]]
Looking at this graph from [[1) Stress and Stress Transformation]] we can identify that:
- Minimum/maximum direct stress occur in the principal directions
- The maximum and minimum direct stress for a given direction are offset by 90 degrees
- The shear stress is always zero in the principal directions, and maximum/minimum at a 45 degree offset.
\
#### Principal Stresses and Principal Directions
*For any state of stress, there exist perpendicular principal directions with corresponding principal stresses, where (i) direct stress is maximum or minimum, and (ii) shear stress is zero*:
![[Pasted image 20240929122738.png|centre]]
We explored this slightly when[[Defining Axes#Principal Axes (1,2) (angle $ theta_{P}$)| defining axes]] except there they were defined at the maximum/minimum second moment of area.
### Stress Analysis
We can find the **angle of the principal directions** in relation to our arbitrary axes using:
$$\tan2\theta_{p}=\frac{2\tau_{xy}}{\sigma_{xx}-\sigma_{yy}}$$
The **principal stresses** can be found to be:
$$\sigma_{1,2}=\frac{\sigma_{xx}+\sigma_{yy}}{2}\pm\sqrt{\left(\frac{\sigma_{xx}-\sigma_{yy}}{2}\right)^{2}+\tau_{xy}^{2}}$$
And the **constant mean stress** is:
$$\sigma_{m}=\frac{\sigma_{x'x'}+\sigma_{y'y}}{2}= \frac{\sigma_{1}+\sigma_{2}}{2}=C$$
The **maximum/minimum shear stress** can be found to be:
$$\tau_{\text{max, min}}=\pm\frac{\sigma_{1}-\sigma_{2}}{2}=\pm\sqrt{\left(\frac{\sigma_{xx}-\sigma_{yy}}{2}\right)^{2}+\tau_{xy}^{2}}$$
*With the directions of maximum/minimum shear stress at 45 degrees to the principal directions/axes.*
