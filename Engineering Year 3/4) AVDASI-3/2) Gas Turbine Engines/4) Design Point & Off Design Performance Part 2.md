### Dimensional Relationships

| Group            | Non-Dimensional                                 | Quasi-Dimensional                 |
| ---------------- | ----------------------------------------------- | --------------------------------- |
| Rotational Speed | $$\frac{N\cdot D}{\sqrt{R\cdot T_O}}$$          | $$\frac{N}{\sqrt{T_{O}}}$$        |
| Mass Flow        | $$\frac{\dot{m}\sqrt{R\cdot T_O}}{A\cdot P_O}$$ | $$\frac{\dot{m}\sqrt{T_O}}{P_O}$$ |
| Flow Velocity    | $$\frac{C}{\sqrt{\gamma R T}}(M)$$              | $$\frac{C}{\sqrt{T}}$$            |
### The Flow Chart for Simple Design Point & Part Load Performance Calculation
![[Pasted image 20260210111744.png|centre|400]]
#### Part-Load Iteration Procedure#
Iteration carried out on $P_{03}/P_{02}$ and combustor temperature $T_{04}$ until the turbine "swallowing capacity" i.e. non-dimensional $m_{4}\sqrt{T_{04}}/P_{04}$ and nozzle throat area are the same as the engine design point values.

From the first guess, the combustor temperature $T_{04}$ is varied at constant compressor delivery pressure ratio until the design value of $\frac{\dot{m}\sqrt{T_{04}}}{P_{04}}$ is obtained.

This is repeated for another value of the compression ratio and so on until the final solution is reached.

*N/B The first guess would be valid if the engine could be designed with a variable throat area and a variable nozzle throat area and probided there is sufficient compressor surge margin.*

#### Turbojet Design Point Example
See [[Lecture 4 - Design Point, and Off-Design Performance Part 2.pdf#page=8|Lecture 4 - Design Point, and Off-Design Performance Part 2, p.8]] for the example.

### Typical Compressor Operating Line
![[Pasted image 20260210112205.png|centre|500]]

### Turbojet Thrust Variation with Combustion Temperature
![[Pasted image 20260210112241.png|centre|500]]
### Turbojet Thrust Variation with Ambient Temperature
![[Pasted image 20260210112309.png|centre|500]]
### Turbojet Thrust Variation with Mach No.
![[Pasted image 20260210112406.png|centre|500]]
### Turbojet Climb Thrust Characteristics
![[Pasted image 20260210112515.png|centre|500]]
### Turbojet Fuel Consumption Characteristics
![[Pasted image 20260210112547.png|centre|500]]
### Typical Engine Data
The following figure shows the typical engine data for a subsonic transport aircraft
