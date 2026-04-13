There are 3 main configurations of propellers:
- Open propellers (most common & earliest use)
- Shrouded propellers (for low speed applications)
- Ducted fans (Good for low speed STOL and VTOL applications, also sometimes features in high speed applications especially in turbo-fans for efficiency gains at cruise)

### Open Propellers
**Pros**
- Simple
- Relatively insensitive to yaw and pitch
- Has little or no effect on lateral stability
- Noise
- Affordable
**Cons**
- Tip losses can be significant
- Poor static thrust performance
- Potential hazard to ground personnel
- No containment in the event of "blade-off" failure
- Noise

### Shrouded Propellers
**Pros**
- Tip losses significantly reduced
- Reduced hazard to ground personnel
- Static thrust greater than equivalent open propeller
- Relatively insensitive to yaw and pitch
- Has little effect on aircraft lateral stability
- Some containment in the event of blade off failure
- Noise
- Structural support for control surface
**Cons**
- Lower static thrust efficiency than an open propeller
- Higher profile drag
- Structural complexity

### Ducted Fans (Low Speed)
**Pros**
- Tip losses significantly reduced
- Reduced hazard to ground personnel
- Static thrust greater than equivalent open propeller
- Significant containment in the event of blade off failure
- Conductive to thrust vectoring
- Noise

**Cons**
- Lower static thrust efficiency than equivalent open propeller
- Very sensitive to pitch and yaw
- May have significant effect on aircraft lateral stability
- High profile drag
- Structural complexity

### Ducted Fans (High Speed)
**Pros**
- Tip losses significantly reduced
- Natural flow conditioning to satisfy engine entry requirements
- Reduced hazard to ground personnel
- Total containment in the event of blade off failure
- Noise
**Cons**
- Very low static thrust efficiency
- Very sensitive to pitch and yaw
- May have significant effect on aircraft lateral stability
- High profile drag
- Structural complexity and weight

### Open Propeller (Tractor Prop Drag Effects)
When we have previously considered momentum disc theory:
![[Pasted image 20260413112436.png]]
Which shows that the velocity downstream is modified by a factor of $(1+2a)$, where $a=v/V$. This means that we can represent the thrust as:
$$T=2\rho A(V+v)v=2\rho AV^{2}(1+a)a$$
or:
$$(1+2a)^{2}=1+\frac{2T}{\rho AV^{2}}$$
So we can represent this factor in terms of Thrust. The aircraft body (in the wake) experiences this increased velocity and hence sees a higher drag. The drag is increased to $D^{*}_{btw}$:
$$D^{*}_{btw}= D(1+2a)^{2} = D\left[1+\frac{2T}{\rho AV}\right]$$
We can also define propulsive thrust, which is the amount of thrust required to overcome this additional drag:
$$T_{P}=T-(D^{*}-D)=T\left[1-\frac{2D}{\rho AV^{2}}\right]$$
Since the drag $D$ (and $D^{*}$) is proportional to the square of the velocity, the propulsive thrust is a constant fraction of the apparent (or total) thrust (i.e. $\frac{T_{p}}{T}=\text{constant}$)

### Effect of Propeller on Yaw & Pit