### The Three Common Cases of Harmonic Excitation
#### Force Excitation
![[Pasted image 20250123145809.png|centre|200]]
This is the kind of excitation that we have previously looked at - where an external force is applied to the system.
The mathematical model for this excitation is:
$$m\ddot{x}+c\dot{x}+kx=F_{0}\sin(\omega t)$$
#### Unbalance Excitation
![[Pasted image 20250123145838.png|centre|200]]
Consider a 1DOF system with a mass $m_{U}$ rotating with constant angual speed $\omega$ with an offset $e$. We are interested in the dynamic response of the mass as well as the properties or characteristics of the system loaded in this way.
![[Pasted image 20250123150208.png|centre]]
Based on this analysis, when constrained to move as a 1DOF system, the rotating unbalance causes harmonic excitation and the resulting EOM is:
$$m\ddot{x}+c\dot{x}+kx=(m_{U}\omega^{2}e)\cos(\omega t)$$
#### Base Motion Excitation
![[Pasted image 20250123145856.png|centre|200]]
Consider a 1DOF system where no external force is applied. However, the ground (base) is allowed to move according to the known function of time $y(t)$:
![[Pasted image 20250123150408.png|centre]]
Assume the base excitation model as defined as a function $y(t)=Y\sin(\omega t)$. The resulting EOM can be written in the following form:
$$m\ddot{x}+c\dot{x}+kx=c\omega Y\cos(\omega t)+kY\sin(\omega t)$$
### Summary of Harmonic Excitation
![[Pasted image 20250123150611.png|centre]]
### Load Transmitted to the Ground
In practical applications, we are often interested in the loads that are transmitted between the systems (mass) and the surrounding environment (base, ground, connected systems, etc.). Alternatively, we might be interested to know what the forces are that load the connecting links such as dampers or springs. The following system decomposition demonstrates the process:
![[Pasted image 20250123150829.png|centre]]
### Harmonic Excitation Summary (Complex Numbers)
![[Pasted image 20250123151017.png|centre]]
### Harmonic Excitation - Analytical Solution
![[Pasted image 20250123151238.png|centre]]
![[Pasted image 20250123151252.png|centre]]
![[Pasted image 20250123151334.png|centre]]
