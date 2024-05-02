Things to think about with regards to cruise:
- Density decreases with altitude
	- Lift will also decrease with decreasing density so we must speed up to compensate
	- Drag decreases with decreased density, but grows with increased speed required to maintain lift
	- Engine power decreases along with density - limits maximum altitude, but fuel consumption also decreases.
- Is there a point where power required = maximum power available? (i.e. no excess power)
- Regardless of optimum speeds for minimum drag or minimum power, operating conditions may dictate flight speeds (the plane is part of a schedule - it may not want to arrive earlier than expected as there may not be room at the airport)
### Power vs Altitude
#### Power Required at Sea Level
We can see the power required for different speeds at sea level on the graph below:
![[Screenshot 2024-03-14 144441.png]]
This is generated from the fact that at cruise power is equal to drag times velocity (as drag is equal to thrust and thrust times velocity is equal to the power output of the engines at constant speed.)
#### Impact of Propulsion
We also need to consider how different types of propulsion will impact our power available.
We know that, in simple terms, when thrust/power is plotted against speed:
**For Jet Aircraft**
- Thrust remains constant with speed
- Power increases linearly with speed ($P=TV$)
![[Thrust and Power Variation with TAS (Jet).png|center|300]]
**For Propeller Aircraft**
- Thrust reduces with speed ($T=P/V$)
- Power output remains constant with speed.
![[Thrust and Power Variation with TAS (Propeller).png|center|300]]
#### Power at Altitude
If we plot power against true air speed for a jet engine:
![[Power vs TAS (For a Jet Engine).png|center|500]]
We can see that increasing altitude reduces the slope of the power available at any given air speed. However as we increase altitude the power required for any given air speed is generally lower - however when flying at lower speeds the power required is actually higher when flying at altitude.
#### Power At Ceiling
If we continue to increase the altitude the line showing the amount of power required at that altitude will continue moving up and to the right until it intersects with the maximum power available line only once:
![[Power vs TAS (at Ceiling - for a Jet).png|center|500]]
This represents the only equilibrium point, if we were to attempt to fly higher we wouldn't have enough power as the power required curve would be above the power available line.
We have just described the 'ceiling' of the aircraft.
### Thrust vs Altitude
At a constant speed we know that drag is equal to thrust.
#### Drag (Thrust) at Sea Level
We have seen the graph of drag verses true air speed (at sea level) before [[Level Flight#Expanding on the Drag Equation|when considering Drag in Level Flight]], if we remind ourselves:
![[Total Drag Polar.png|center|500]]
The total drag (the black line) has a minimum value where the zero lift drag and induced drag lines intersect.
#### Thrust at Altitude (for a Jet)
If we plot a graph of drag/thrust against equivalent air speed (remembering that equivalent air speed is independent of altitude):
![[Drag or Thrust against EAS at Different Altitudes.png|center|500]]
Remembering that the stall boundary is the speed at which the lift coefficient required is equal to the maximum lift coefficient so at any speed lower than that we cannot produce enough lift to stay in the air.
We can also see the ceiling of the aircraft on this graph as well, it occurs at the turning point of the curve.
**Note that this occurs at the minimum drag speed!** (See [[Level Flight#Minimum Drag Speed]])
Increasing the weight increases the induced drag, however has a very small impact on the zero lift drag, this does significantly decrease the ceiling of the aircraft however.
#### Features of the Thrust at Altitude Diagram
The key features of the diagram above are as follows:
- We can represent thrust using a simplified equation:
$$\boxed{T=kT_o\sigma^2}$$
Where $T_0$ is the maximum thrust at sea level, $k$ is the throttle setting (i.e. how much throttle is being used), and $\sigma^x$ is the density ratio (note that the $x$ power is 0.7 below 11km, and 1.0 above)
- The maximum and minimum speed at each altitude are where $T=D$
	- Lower speeds may be unattainable at low altitudes due to stall
	- Upper speed is a practical cruise speed
	- Between the upper and lower speeds aircraft will accelerate or climb unless the throttle setting is reduced.
- The Absolute Ceiling is when there is no excess thrust available, this is achieved at minimum drag speed.
- Increasing weight reduces cruise speed and lowers ceiling.
### Cruise Speed vs Altitude
Plotting a graph of altitude against equivalent (blue)/true (black) air speed:
![[Cruise Speed vs Altitude Polar.png|center|500]]
So:
- Cruise speed in EAS reduces steadily as altitude increases (due to available power reductions)
- However maximum cruise speed in TAS increases with altitude
	- Up to a maximum $V_{max}$ before the absolute ceiling is approached
- This demonstrates the advantages of cruise at high altitude
	- Maximum cruise speed in TAS is similar to (or greater than) speed at sea level.
	- Thrust (drag) at maximum cruise speed reduces with altitude which results in a decrease in fuel consumption with altitude (as fuel consumption is directly proportional to thrust)
- Minimum fuel consumption at minimum drag speed (at the absolute ceiling).
	- Work done = thrust $\times$ distance - we want to minimise work done so we want to minimise the amount of thrust required.
	- In theory should be unaffected by altitude (since $D_{min}$ is constant) but at low altitudes the engine would need to be throttled back. This results in reduced thermodynamic efficiency and hence increased fuel burn.
### Speed Stability in Cruise
Lets consider an aircraft with throttle adjusted to cruise at points 1, 2, and 3:
![[Screenshot 2024-03-14 154840.png|center|500]]
Let us consider: what is the effect of a small fluctuation in velocity (e.g. due to gusts)?
1) Speed increase = increase in drag, however the throttle hasn't increased so the thrust available is the same resulting in the aircraft decelerating returning to the cruise speed. **The same is true of a speed decrease as the thrust would then be greater than the drag and hence the aircraft would accelerate back up to the cruise speed.**
2) Speed increase = reduction in drag, this results in an acceleration as the thrust is now greater than the drag, and as the aircraft continues to accelerate the drag decreases further resulting in even more excess thrust until we adjust the throttle. **Again this is the same when the aircraft slows down, there will be insufficient thrust which will result in a deceleration resulting in an even greater lack of thrust.** Hence the aircraft is unstable!
3) Speed increase = no change in drag, and as a result there is no/little change in the operating conditions. This is called a neutrally stable point (the return to the original conditions won't be very fast).
### Speed Stability at Ceiling
The absolute ceiling is an unstable condition to maintain, this is because it occurs at the maximum thrust setting at the minimum drag speed. This means that any change in speed will increase drag above the available thrust, and therefore the aircraft will have to descend.
Excess thrust and hence rate of climb also drop to zero as the ceiling is approached so the absolute ceiling cannot be established in reasonable time.
**The service ceiling is a practical alternative definition of maximum operating altitude. At the service ceiling the aircraft still has a small specified rate of climb.**
**This is defined as 2.5m/s for jet aircraft and 0.5m/s for propeller-driven aircraft.**