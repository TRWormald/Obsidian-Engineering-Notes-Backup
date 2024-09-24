Along a given wall $i$ of arclength ($0\le s\le b_{i}$) we write:
$$\boxed{^{i}q_{(s)}=q_{[i-1]}-C_x\int_{0}^{s} {^{i}x_{(s)}}{^{i}t_{(s)}}~ds-C_{y}\int_{0}^{s}{^{i}y_{s}}{^{i}t_{s}}~ds}$$
Where:
$$\boxed{\begin{align*}
C_{x}&= \frac{S_{x}I_{xx}+S_{y}I_{xy}}{I_{xy}^{2}-I_{xx}I_{yy}}\\
C_{y}&= \frac{S_{y}I_{yy}+S_{x}I_{xy}}{I_{xx}I_{yy}-I_{xy}^{2}}
\end{align*}}$$
The constant of integration $q_{[i-1]}$ is the 'initial value' of $q_{(s)}$, i.e. at the end of the wall $(i-1)$ and at the start of the wall $(i)$.
If wall $i=1$ starts from a free edge, the constant $q_{0}=0$
### Conventions for Plotting Shear Flow
- Draw one graph per 'wall'
- Use height of graph to represent magnitude of the shear flow
- Draw arrows to indicate sense - avoiding ambiguity
- Important to obey the shear flow rules:
	- $q_{(s)}$ is zero at free edges
	- $q_{(s)}$ is continuous around the section
	- $q_{(s)}$ is conserved at branches
	- For vertical on-axis shear loading
		- Webs - parabolic distribution of $q_{(s)}$
		- Flanges - linear distribution of $q_{(s)}$
### Plotting Shear Flow in Thin-Walled Sections
Shear flow being transmitted along the span for a vertical upwards shear force $S_y$:
![[Pasted image 20240924100158.png]]
Note how the flanges have linear distribution and the webs have parabolic distribution. While the shear stress is conserved at corners.
### Physical Interpretation of $q_{(s)}$ - Shear Strains
Shear flow is proportional to shear strain $\gamma_{zs}$:
$$q_{(s)}=t_{(s)}\tau_{zs}=(t~G)~\gamma_{zs}$$
So when we consider a simply supported cantilever beam with an upwards shear force:
![[Pasted image 20240924100440.png|centre]]
Results in the following:
![[Screenshot 2024-09-24 100517.png|centre]]
The leftmost diagram shows the profile of the beam when it is undeformed, the second only considers the strain, whilst the third considers only the shear strain. The final image shows the combination of the shear and engineering strain - which is the most realistic model of the beam.
### Shear Flow across Joints
Shear flow is 'transferred' between thin-walled members, e.g. flanges and web:
![[Screenshot 2024-09-24 100826.png|centre]]
![[Pasted image 20240924101234.png]]
We can consider shear flow a lot like current - it is conserved, so if 15 units of shear flow goes into a joint all of that must come out.