Much like with non-flow systems we can construct cycles out of steady-flow processes.
One such process is the Brayton Cycle, which produces power continuously.
The diagram below shows the cycle in full:
\
![[Screenshot 2024-02-25 120154.png]]
\
It consists of four stages:
- Isentropic compression (1-2)
- Isobaric heat addition $Q_{in}$ (2-3)
- Isentropic expansion (3-4)
- Isobaric heat rejection $Q_{out}$ (4-1)
\
##### Performance Indicators
Like with non-flow cycles we can calculate the efficiency of the cycle, there are two possible ways of doing this:
###### Gas Cycle Efficiency
Like with non-flow cycles:
$$ \eta = \frac{|\dot{W}_{net out}|}{|\dot{Q}_{in}|}=\frac{|\dot{W}_{34}-\dot{W}_{12}|}{|\dot{Q}_{23}|}$$
With:
$$\dot{W}_{net out}=|\dot{W}_{34}|-|\dot{W}_{12}|=|\dot{Q}_{23}|-|\dot{Q}_{41}|$$
So:
$$\eta = 1-\frac{|\dot{Q}_{41}|}{|\dot{Q}_{23}|}$$
Which when using the [[Steady-Flow Energy Equation]] for [[Heat Exchangers]]:
$$\eta = 1-\left|\frac{T_4-T_1}{T_3-T_2}\right|$$
###### Work Ratio
This is defined as the net work divided by the turbine work:
$$Work~Ratio = \frac{\dot{W}_{net}}{\dot{W}_{turb}}=1-\left|\frac{\dot{W}_{12}}{\dot{W}_{34}}\right|$$
Which is  then equal to:
$$Work~Ratio=1-\left|\frac{T_2-T_1}{T_3-T_4}\right|$$
In an ideal case we want this to be as close to one as possible.

##### The Turbojet Cycle
The turbojet cycle is very similar to the Brayton cycle but it differs in several ways:
![[Screenshot 2024-03-01 131740.png]]
Primarily it involves a diffuser and a nozzle, and thrust is produced. Also all of the energy produced by the turbine is typically used by the compressor.
The heat exchanger between the compressor and the nozzle models the combustion chamber.