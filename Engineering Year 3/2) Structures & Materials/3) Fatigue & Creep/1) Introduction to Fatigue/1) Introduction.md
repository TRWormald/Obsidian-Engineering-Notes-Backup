### Definitions and Load Cycles
> **Fatigue**
> This is the response to cyclic loads. It is defined by loading *below the elastic limit*. This results in the accumulation of microscopic damage leading to catastrophic failure.

There are a number of different kinds of load cycles that contribute to fatigue:
- Constant amplitude cycles
	- Completely reversed cycle $|S_{max}|=|S_{min}|,~~S_{m}=0$
	- Non-zero mean stress/partly reversed cycle $S_{m}\ne0$
	- Tension-tension cycle $S_{min}>0$
- Variable amplitude cycle
	- Constant mean stress cycle
	- Variable mean stress cycle
![[Pasted image 20251106111627.png|centre|400]]
### Material Level Fatigue Tests
We can test material fatigue using a number of different tests:
- Axial loading fatigue tests (alternating between tension and compression)
![[Pasted image 20251106112303.png|centre|200]]
- Rotating beam fatigue test (allowing you to test the bending response at all angles)
![[Pasted image 20251106112326.png|centre|400]]
For a *constant amplitude completely reversed cycle*:
$$S_{max}=M\cdot \frac{y}{I}=P\cdot L\cdot  \frac{y}{I}=P\cdot L\cdot \frac{\frac{d}{2}}{\frac{\pi}{64}d^{4}}$$
### S-N-P Curve
A S-N-P curve is generally presented as a S-N curve with P=0.5 (Probability of failure =50%). It shows the residual strength of a material vs the number of cycles to failure.
![[Pasted image 20251106112730.png|centre|500]]
The S-N curve can be used for:
- Predicting the component life for a given $S_{max}$
- Estimating allowable $S_{max}$ for an expected lift

>**Fatigue Strength**
>The maximum stress that can be applied in cycles  to give a specified fatigue life (normally $10^{6}$ cycles).

### Safe Design Curve
![[Pasted image 20251106113346.png|centre]]
![[Pasted image 20251106113401.png|centre]]
Sometimes the stress factor is used for reducing the allowable stress on a component - this is commonly used in helicopters.
### S-N Curves for Different Materials
![[Pasted image 20251106113456.png|centre|500]]
![[Pasted image 20251106113514.png|centre]]
>**Fatigue Limit**
>The maximum stress that can be applied in cycles to give an infinite fatigue lift (generally too low for airframe design)

- Metals/alloys with yield point elongation show FL (steel and titanium alloys)
- Metals/alloys with no YPE, do not have FL (Cu & Al alloys)
- Composites do not show FL, but generally have lesser fatigue slopes