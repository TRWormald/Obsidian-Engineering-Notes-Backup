### What Happens to Temperature Along a Stream-tube
A streamtube is defined by streamlines - with no flow normal to the streamlines the mass flow at 1 must equal the mass flow at 2:
$$\dot{m}=\rho_{1}A_{1}V_{1}=\rho_{2}A_{2}V_{2}$$
Then, with the following defined:
$$\text{Rate of KE entering}~~~~~~~~\frac{1}{2}\dot{m}v^{2}$$
$$\text{Rate of work done by pressure forces}~~~FV=pAV$$
$$\text{Rate internal energy entering}~~~~\dot{m}C_{v}T$$
Therefore is we consider energy conservation between 1 and 2:
$$\begin{align*}
const.&= p_{1}A_{1}V_{1}+ \frac{1}{2}\dot{m}V_{1}^{2}+\dot{m}C_{v}T_{1}\\
&= p_{2}A_{2}V_{2}+ \frac{1}{2}\dot{m}V_{2}^{2}+\dot{m}C_{v}T_{2}
\end{align*}$$
We can then rewrite $AV$ as $\dot{m}/\rho$ to get:
$$\begin{align*}
const.&= \frac{p_{1}}{\rho_{1}}\dot{m}+ \frac{1}{2}\dot{m}V_{1}^{2}+\dot{m}C_{v}T_{1}\\
&= \frac{p_{2}}{\rho_{1}}\dot{m}+ \frac{1}{2}\dot{m}V_{2}^{2}+\dot{m}C_{v}T_{2}
\end{align*}$$
And finally we can cancel the mass flow rate:
$$\boxed{\begin{align*}
const.&= \frac{p_{1}}{\rho_{1}}+ \frac{1}{2}V_{1}^{2}+C_{v}T_{1}\\
&= \frac{p_{2}}{\rho_{1}}+ \frac{1}{2}V_{2}^{2}+C_{v}T_{2}
\end{align*}}$$
Which we can rewrite in terms of enthalpy:
$$\boxed{h_{1}+ \frac{1}{2}V_{1}^{2}=h_{2}+ \frac{1}{2}V_{2}^{2}}$$
From which we can see enthalpy is conserved.
Hence we get "compressible Bernoulli":
$$\boxed{h_{0}=h+ \frac{1}{2}V^{2}=const.}$$
Which we can also rewrite for a calorically perfect gas:
$$\boxed{C_{p}T+ \frac{1}{2}V^{2}=const.=h_{0}=C_{p}T_{0}}$$