We have seen previously, for the general finite-volume scheme, that we can obtain:
![[Pasted image 20251106130617.png|centre|400]]
And for a general discrete cell we have:
![[Pasted image 20251106130635.png|centre|250]]
Where $i$ is a cell counter. Hence we just need to loop over cell faces to compute the residual.
But how do we obtain the flux values $\mathbf{\underline{F}}_{k}$ and $\mathbf{\underline{G}}_{k}$ at the cell faces?

One method that has been developed uses "Central Discretisation" and was devised by Antony Jameson.
### Jameson's Central Discretisation
Jameson chose the most simple approximation. He evaluated the solution at each cell face using a simple average of the values either side:
![[Pasted image 20251106131124.png|centre|300]]
$$\mathbf{\underline{U}}_{BC}=\frac{1}{2}(\mathbf{\underline{U}}_{ij}+\mathbf{\underline{U}}_{i+1~j})$$
$$\mathbf{\underline{U}}_{DA}=\frac{1}{2}(\mathbf{\underline{U}}_{i-1~j}+\mathbf{\underline{U}}_{ij})$$
