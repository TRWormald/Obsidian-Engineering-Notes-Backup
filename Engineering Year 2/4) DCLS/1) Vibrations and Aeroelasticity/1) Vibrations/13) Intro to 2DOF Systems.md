Up until this point we have been looking at 1DOF systems:
![[Pasted image 20250128121237.png|centre|250]]
We are now going to start exploring 2DOF systems, some examples of which are shown below:
![[Pasted image 20250128121313.png|centre|300]]
### A 2DOF System
Consider the following 2DOF system:
![[Pasted image 20250128122510.png|centre]]
The main characteristics of this system are:
- The two masses characterised by the mass $m_{1}$ and $m_{2}$
- Two independent displacements described by $x_{1}$ and $x_{2}$
- Two DOFs and, therefore, two equations of motion
- Two applied forces $f_{1}$ and $f_{2}$ acting on the lumped masses
- Three springs with the stiffness parameters $k_{1}$, $k_{2}$, and $k_{3}$
- No damping (undamped system) - there is also no friction and no rolling resistance
#### Parametrising the 2DOF System
![[Pasted image 20250128122945.png|centre]]
#### The Free Body Diagram
![[Pasted image 20250128123009.png|centre]]
Note how that since we have assumed that $x_{1}<x_{2}$ the spring in the centre is in tension.
We can therefore generate the equations of dynamic equilibrium (in the horizontal direction only):
$$\text{Block 1: }-F_{S1}-F_{I1}+F_{S2}+f_{1}=0$$
$$\text{Block 2: }-F_{S2}-F_{I2}-F_{S3}+f_{2}=0$$
We can then substitute the equations for the forces in (they're all springs or inertial forces):
$$\text{Block 1: }-k_{1}x_{1}-m_1\ddot{x}_{1}+k_{2}(x_{2}-x_{1})+f_{1}=0$$
$$\text{Block 2: }-k_{2}(x_{2}-x_{1})-m_2\ddot{x}_{2}-k_{3}x_{3}+f_{2}=0$$
Which can be simplified to:
$$\text{Block 1: }m_{1}\ddot{x}_{1}+(k_{1}+k_{2})x_{1}-k_{2}x_{2}=f_{1}$$
$$\text{Block 2: }m_{2}\ddot{x}_{2}-k_{2}x_{1}+(k_{2}+k_{3})x_{2}=f_{2}$$
**With these EOMs found we can now represent them in matrix form:**
$$\begin{bmatrix}m_{1}&0\\0&m_{2}\end{bmatrix}\begin{bmatrix}\ddot{x}_{1}\\\ddot{x}_{2}\end{bmatrix}+\begin{bmatrix}k_{1}+k_{2}&-k_{2}\\-k_{2}&k_{2}+k_{3}\end{bmatrix}\begin{bmatrix}x_{1}\\x_{2}\end{bmatrix}=\begin{bmatrix}f_{1}\\f_{2}\end{bmatrix}$$
Which we can represent using the following notation:
$$\mathbf{M}\ddot{\mathbf{x}}+\mathbf{K}\mathbf{x}=\mathbf{f}(t)$$
