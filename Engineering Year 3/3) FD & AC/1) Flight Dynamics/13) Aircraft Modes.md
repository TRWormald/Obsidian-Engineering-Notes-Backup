Following the trimming and linearisation of the aircraft and observing the eigenvalues and eigenvectors of the system we can observe the "modes" of the aircraft.

There are five primary modes in dynamic flight:
**Aircraft Modes - Longitudinal** (Phugoid & Short-Period)
**Aircraft Modes - Lateral-Directional** (Roll Subsidence, Dutch Roll, and Spiral)
### Longitudinal Modes
There are two complex conjugate pairs. One is low frequency and low damping ratio (the Phugoid) and can even be unstable (i.e. $\sigma$ is positive). The short-period pair is higher frequency and much more heavily damped. typically $\sigma$ is much more negative.
![[Pasted image 20251107111126.png|centre|500]]
#### The Short-Period Mode
The disturbance velocity in the transverse direction $w$ helps to define the total incidence during the disturbance because of $\Delta\alpha=w/U$
Thus, whatever steady flight incidence there has been, a transverse disturbance of $w$ will alter it, and the longitudinal balance of forces will be lost.
Similarly, a disturbance of the pitch balance will lead to pitching action and a pitch rate $q$. These two disturbances cause the wing and its tail lifts to depart from the trimmed values and thus the consequent short-period mode is essentially a seeking of that trimmed state again. It does not take long to achieve and is generally quite heavily damped.

The short period motion is thus composed of largely $w$ and $q$ with virtually no change in forward speed.
A typical period would be 1-4 seconds.
#### The Phugoid Mode
This is primarily $u$ and $\theta$ motion with small $q$ and nearly zero $w$. The $u$ and $\theta$ action can be envisaged as follows:
a) A pitch disturbance $\Delta\theta$ causes the aircraft to climb slowly
b) The forward speed $U$ is caused to drop ($u$ becomes negative)
c) For a stable aircraft, such a loss of speed will cause a pitching moment (nose down) that tends to restore the trimmed condition, so the positive disturbances $\Delta\theta$ tends to zero and then becomes negative after the aircraft reaches a peak departure in altitude from its former flight level. 
d) The inevitable overshoot in $\theta$ because of the vehicle's pitch inertia causes the aircraft to "start going downhill"
e) The speed slowly picks up ($u$ u now becoming positive)
f) Again for the same reason as in c) the overall pitching moment becomes positive and brings the nose up. So negative $\theta$ becomes zero and then becomes positive.
g) There will have been a noticeable loss of altitude and the climb back to the original height begins, at small positive $\theta$ 

The full cycle can involve change in altitude of tens of metres for a large aircraft, but the pitch action and the changes of forward speed are quite slow.
Periods are typically 15-100s and even if $\sigma$ >0 (unstable motion) it is controllable by the pilot because of the small frequency. In reality an autopilot loop often supresses the motion.
#### Typical Longitudinal Response
![[Pasted image 20251107111948.png|centre]]
![[Pasted image 20251107112009.png|centre]]
![[Pasted image 20251107112022.png|centre]]
### Lateral Modes
![[Pasted image 20251107112104.png|centre]]
1) A mode with a large negative real root is called the roll convergence (or roll subsidence). This implies almost pure rolling motion and of course it cannot last long because after the first 90 degrees you fall out of the sky. A more realistic attitude suggests that if you roll a "pulse" hits the aircraft (e.g. a brief up-gust on one wing), the consequent response in roll would be heavily damped.
2) A mode with a small real root of either sign is called the spiral mode. This would be, for an unstable case, a slow divergence in yaw (say nose to starboard) while a roll angle built up (rolling to starboard) and thus a sideslip would also develop. The later stage would be a tightening spiral dive with all three motion variables involved. In practice, a pilot can control an unstable spiral mode.
![[Pasted image 20251107112513.png|centre|500]]
3) A mode with a complex pair is called a Dutch Roll. Strictly speaking, all freedoms are active here, in an oscillatory sense, and out of phase with each other. This mode can be badly (though positively) damped and will affect handling qualities. The frequency is probably lower (the period a bit longer) than the longitudinal short-period mode. It is often poorly damped on swept wing aircraft, and is excited with the rudder of aileron.
![[Pasted image 20251107112802.png|centre]]
### System Stability
For notes on system stability look at [[Flight Dynamics Lecture 14 - Aircraft Dynamic Modes.pdf#page=28|Flight Dynamics Lecture 14 - Aircraft Dynamic Modes, p.28]].
