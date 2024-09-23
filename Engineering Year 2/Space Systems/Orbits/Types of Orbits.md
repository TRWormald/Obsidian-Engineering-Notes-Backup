### Orbital Altitude Classifications
There are various different types of orbits, classified by altitude they are:

| Name                         | Altitude          |
| ---------------------------- | ----------------- |
| LEO<br>(Low Earth Orbit)     | <~2,000 km        |
| MEO<br>(Medium Earth Orbit)  | 2,000 - 36,000 km |
| GEO<br>(Geostationary Orbit) | Exactly 35,786 km |
### Nodal Regression
Nodal regression is caused by Earth not being a perfect sphere. It causes the ascending node to move eastwards or westwards depending whether the inclination is more or less than 90 degrees. 
![[Screenshot 2024-09-23 150933.png|centre]]
#### Sun-Synchronous Orbits
It is possible to choose the parameters of a spacecraft's orbit to take advantage of some or all of these gravitational influences to induce regression, which causes a motion of the orbital plane. Nodal regression shifts the ascending node by ~1 degree per day which gives a sun-synchronous obit. In this case, the satellite then scans the same path under the same lighting conditions, i.e. the same angle of sunlight. This requires a slightly retrograde orbit (i=97.56 for a 550km)
This kind of orbit is used for Earth Observation as having the same shadow direction makes comparison much easier.
### Molniya Orbit
These orbits are highly eccentric, meaning that due to Kepler's 3rd Law they will spend a lot of their time in the neighbourhood of their apoapsis, which for a Molniya orbit is over the northern hemisphere.
It is often used as a substitute for geostationary satellites in higher latitudes as they have limited coverage due to the curvature of the earth.
![[Pasted image 20240923151647.png]]
## Orbital Perturbations
All orbits evolve over time due to various factors, these can be:
- Atmospheric drag (at LEO altitudes only)
	- This is worse during increased solar activity, but insignificant over 800km
- Non-sphericity of the Earth
	- The gravity of the earth isn't a constant 9.81m/s, meaning th