Multiple processes can be joined together to create cycles.
##### Gas Cycle Assumptions
We need to make several assumptions about gas cycles before we can analyse them:
- The cycle is closed
- The working fluid is an ideal gas
- Combustion is modelled by a heat input
- Exhaust is modelled by a heat output
- The specific heat capacity is constant
##### The Otto Cycle
One common cycle is 'The Otto Cycle':
\
![[Screenshot 2024-02-23 170259 1.png]]
\
It consists of 4 'strokes':
- Intake (of fuel/air mix)
- Compression
- Combustion
- Expulsion of exhaust gases
\
However these do not perfectly translate to the various processes that occur on the p-V diagram.
There is:
- Isentropic compression $W_{12}$ which reduces the volume (this is the backstroke after combustion)
- Isochoric heat addition $Q_{23}$ (this models the combustion)
- Isentropic expansion $W_{34}$ (this is the expansion due to the increased pressure due to combustion)
- Isochoric heat removal $Q_{41}$ (this is the removal of heat necessary to return to the original conditions)
\
One interesting property of this cycle is the 'compression ratio' ($r$) which is defined as:
\
$$ r=\frac{V_{max}}{v_{min}}=\frac{V_1}{V_2}=\frac{V_4}{V_3}$$
\
We can use the isentropic relation (See the [[Isentropic Process]]) combined with the [[Ideal Gas Law]] to get:
\
$$T_2 = T_1~r^{\gamma-1}$$
\
Allowing us to relate the temperatures with the compression ratio and the isentropic constant of proportionality.
##### Cycle Efficiency
We can calculate the efficiency of a cycle in the following way:
\
We know that efficiency is defined as:
$$\eta = \frac{useful~output}{paid~input}$$
Which we can rewrite as:
$$\eta = \frac{net~work~output}{heat~input}$$
Hence, as the net work output is:
$$|W_{34}| -|W_{12}|=|Q_{23}|-|Q_{41}|$$
The efficiency becomes (for any cycle):
$$\eta = \frac{|Q_{23}|-|Q_{41}|}{|Q_{23}|}=1-\frac{Q_{out}}{Q_{in}}$$
And for the Otto cycle only:
$$\eta = 1 - \frac{T_4-T_1}{T_3-T_2}=1-\frac{1}{r^{\gamma-1}}$$




