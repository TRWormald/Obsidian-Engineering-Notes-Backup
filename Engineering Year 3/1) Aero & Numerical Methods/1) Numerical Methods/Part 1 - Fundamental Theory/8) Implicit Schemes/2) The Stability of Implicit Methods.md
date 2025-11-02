Using the Von-Neumann Fourier stability analysis with the implicit scheme:
$$u_{i}^{n+1}=n_{i}^{n}-\nu_{i}(u_{i}^{n+1}-u_{i-1}^{n+1})$$
where as before:
$$\nu_{i}=\frac{c\Delta t}{\Delta x}$$
Substituting our Fourier representation gives:
$$u_{i}^{n+1}=u_{i}^{n}-\nu_{i}\left[e^{jki\Delta x}e^{-jkc(n+1)\Delta t}-\mathbf{e^{jk(i-1)\Delta x}}e^{-jkc(n+1)\Delta t}\right]$$
Expanding the bold term and then factorising our $e^{jki\Delta x}e^{-jkc(n+1)\Delta t}$ gives:
$$u_{i}^{n+1}=u_{i}^{n}-\nu_{i}u_{i}^{n+1}\left[1-e^{-jk\Delta x}\right]$$
Substituting $u_{i}^{n+1}=\lambda u_{i}^{n}$:
$$\lambda u_{i}^{n}=u_{i}^{n}-\nu_{i}\lambda u_{i}^{n}\left[1-e^{-jk\Delta x}\right]$$
We can then divide through by $u_{i}^{n}$ to give:
$$\lambda=1-\nu\lambda\left[1-e\right]$$
