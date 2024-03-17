__The Clausius Inequality__
"*Whenever a system undergoes a cycle, $\oint \frac{dQ}{T}$ is zero if the cycle is reversible and negative if irreversible, i.e. in general $\oint \frac{dQ}{T}\le 0$*"
\
Consider the following system:
![[Pasted image 20240226110042.png]]
Combining the Clausius Inequality with what we know of [[Entropy]] we get that:
$$\oint \frac{dQ}{T}\le 0$$
$$\int_1^2 \frac{Q_{12}}{T} + \int_2^1 \frac{Q_{21}}{T}\le 0$$
So, for a reversible process:
$$\int_2^1\frac{Q_{21}}{T}=S_1-S_2$$
But for a non reversible process:
$$\int_1^2\frac{Q_{12}}{T}\le S_2-S_1$$
Resulting in (when we add a constant):
$$S_2-S_1 = \int_1^2\frac{Q_{12}}{T}+S_{gen}$$
Where $S_{gen}\ge 0$
\
\
For an isolated system, $Q=0$, so there is no entropy transfer to the surroundings.
So we know that:
$$\Delta S_{sys}\ge 0$$
As it will be equal to zero when the processes are perfectly reversible and must be greater than zero in all other cases.

#### Important Equations
The key equations to take away from this are:
\
-The Clausius Inequality:
$$\oint \frac{dQ}{T}\le 0$$
-Entropy for a reversible process:
$$\int_1^2\left(\frac{dQ}{T}\right)=S_2-S_1=dS$$
-Entropy is generated in irreversible processes, so the entropy of a thermally isolated system increases or stays the same:
$$\Delta S_{sys}\ge 0$$
