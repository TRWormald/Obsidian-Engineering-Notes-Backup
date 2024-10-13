In multi-cell sections we analyse each cell $j$ separately, considering individual cell areas $\bar{A}_{j}$ and solving for shear flow constants $\bar{q}_{j}$.
We follow the right hand rule when integrating along each cell.
Cells interact in two different ways:
![[Pasted image 20241013121607.png]]
### Simultaneous Equations
Cells are indexed by the subscript $j=1...n$, where $n$ is the total number of cells.
We introduce a 'notional cut' in each cell, and we get $n$ unknown values of $\bar{q}_{J}$.
The externally applied load or global deformation usually provides an additional unknown:
- Pure torsion: $T$ or $\frac{d\theta}{dz}$
- Shear loading $e_{x}$, $e_{y}$, or $\frac{d\theta}{dz}$
We need $(n+1)$ equations to solve for these unknowns.
#### Rates of twist for each cell $j$
Writing the twist rate equation for cell $j$ gives:
$$\frac{d\theta}{dz}=\frac{1}{2\bar{A}_{j}G}\oint_{j}q_{(s)}^{closed} \frac{ds}{t}$$
So we can rearrange this to be:
$$\oint_{j}q_{(s)}^{closed} \frac{ds}{t}=(2\bar{A}_{j}G) \frac{d\theta}{dz}$$
Convert the loop integral into a summation of all of the walls:
$$\sum\limits_{i\in j}\left[(q_{i}^{open}+^{*}\bar{q}_{i})\frac{b_{i}}{t_{i}}\right]=(2\bar{A}_{j}G)\frac{d\theta}{dz}$$
Where:
$$^{*}\bar{q}_{i}=\left\{\begin{matrix}\bar{q}_{j}~~~~~~~~~~~~~~~~~~{\text{Wall is exclusive to cell j}}\\\bar{q}_{j}-\bar{q}_{[j\pm 1]}~~~~~~~\text{Wall is shared with cell }[j\pm1]\end{matrix} \right.$$
#### Balance of Torques
We have an equation relating the pure torsion case and the shear loading case to the stress resultant torque:
$$T+S_{Y}e_{X}-S_{X}e_{Y}=\oint q_{(s)}^{closed}r_{(s)}ds$$
And:
$$\begin{align*}
\oint q_{(s)}^{closed}r_{(s)}ds&= \oint(q_{(s)}^{open}+\bar{q})r_{(s)}ds\\
&= \oint q_{(s)}^{open}r_{(s)}ds+\bar{q}\underbrace{\oint r_{(s)}ds}_{=2\bar{A}}
\end{align*}$$
Hence:
$$\underbrace{T}_{\text{Pure Torsion}}+\underbrace{S_{Y}e_{X}-S_{X}e_{Y}}_{\text{Shear Loading Case}}=\underbrace{\sum\limits_{\text{all } i}(q_{i}^{open}\cdot r_{i}\cdot b_{i})}_{\text{Open-cell flow along walls}}+\sum\limits_{\text{all }j}(2\bar{A}_{j}\bar{q}_{j})$$ 
