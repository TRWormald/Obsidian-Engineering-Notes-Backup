Both types of circuit analysis that we will look at use similar techniques to solve circuits - primarily Kirchhoff's Circuit Laws.
### Nodal Analysis
In nodal analysis we are interested in what is happening at circuit nodes - we use Kirchhoff's current law as the basis for finding voltages at nodes.
**This can be used for both planar and non planar circuits.**
The steps are:
1) Label all the nodes in the circuit
2) Use our knowledge of currents flowing into and out of nodes to determine branch currents
3) Select a reference (or earth) node
4) Since we have resistances and currents we can calculate the voltages using Ohm's Law.
5) If we have voltage sources we need to create a super-node and use Kirchhoff's Voltage Law alongside Ohm's Law to calculate node voltages.
#### Worked Example
##### Example 1 (Using only KCL)
![[Pasted image 20240829121345.png|center|300]]
Taking the example above we can calculate the currents at each node:
1 - $I_{1}=60[mA]+20[mA]=80 [mA]$
2 - $I_{4}=I_{1}+I_{6}$
3 - $60[mA]+I_{5}=I_{4}+40[mA]$
4 - $20[mA]+30[mA]=I_{5}$
5 - $I_{6}+40[mA]=30[mA]$

We have five equations and 4 unknowns therefore it is simple to solve to get all of the currents:
$I_{1}=80[mA]$
$I_{5}=50[mA]$
$I_{6}=-10[mA]$
$I_{4}=70[mA]$
##### Example 2 (With Current Source)
##### Example 3 (With Voltage Source)

### Mesh Analysis