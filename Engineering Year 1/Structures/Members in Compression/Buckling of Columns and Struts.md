Compared with members in tension, when in compression the ability to carry load is often much reduced.
With a column or strut the stress as a result of an applied compressive load is equal to:
\
$$ \sigma = -\frac{P}{A} $$
\
Where:
$\sigma$ is the [[Stress]] ($N/m^2$)
$P$ is the load applied ($N$)
$A$ is the cross sectional area of the column ($m^2$)
\
When we experimentally test the compressive strength of columns and struts we notice that as the length of these elements increases the load required for failure decreases. This leads us to the equation:
\
$$ P=\frac{{\pi}^2\cdot E \cdot I}{L^2}$$
\
Where:
$P$ is the buckling load or Euler Critical Load
$E$ is the [[Young's Modulus]] of the material ($Pa$)
$I$ is the [[Second Moment of Area]] of the element ($m^4$)
$L$ is the length of the element ($m$)
\
Which results in the displacement of the member by:
\
$$ w(x)=C \cdot sin\left(\frac{\pi x}{L}\right)$$
\
Where:
$w(x)$ is the displacement at distance $x$ from the support ($m$)
$C$ is a constant used to make the displacement zero at the joint/pin
$L$ is the overall length of the member
\
The above formula can be further expanded upon depending on how the member will buckle:
\
$$ w(x)=C \cdot sin\left(\frac{n\pi x}{L}\right)$$
\
Where $n$ is a constant (typically an integer)
The influence of the $n$ value can be seen below:
\
![[Pasted image 20240222101400.png]]
\
Note:
For elements with non uniform values of $I$ ([[Second Moment of Area]]) buckling will occur about the 'weak' axis, i.e. the axis which has the smallest value of $I$.
\
\
The compressive load a bar can resist becomes smaller with increasing slenderness:
\
$$ \sigma = \frac{P}{A} = \frac{\pi^2~E~I}{A~L^2} = \frac{\pi^2~E}{\left(\frac{L}{k}\right)^2}$$
\
Where:
\
Radius of Gyration = $k=\sqrt{\frac{I}{A}}$
Slenderness Ratio = $\frac{L}{k}$
\
However in practice imperfections exist and therefore experimentally measured buckling loads are lower than expected - even whilst using the above formula.