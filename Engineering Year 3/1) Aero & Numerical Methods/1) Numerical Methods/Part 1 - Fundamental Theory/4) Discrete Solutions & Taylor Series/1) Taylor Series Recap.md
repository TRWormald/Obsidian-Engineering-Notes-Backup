Taylor series defines a polynomial expression in the neighbourhood of some arbitrary point that approximates the original function close to that point.
Consider a function of a single variable $f(x)$, the Taylor series polynomial approximation around $x$ reads:
![[Pasted image 20251002130553.png|centre]]
Consider setting $\Delta x=0$, then the expansion recovers $f$. Consider differentiating once, then setting $\Delta x=0$, and its recovers $f'$, etc. Each time you differentiate the right number of times and evaluate at zero, it recovers the derivative you want, hence the structure of the series.

For a general function of multiple variables (consider coordinates here), we can expand in any variable direction, assuming we expand over a "small" distance. For example consider expanding $F(x,y,z)$ in $x$:
![[Pasted image 20251002130928.png|centre]]
Expanding out the simulation gives:
![[Pasted image 20251002130951.png|centre]]
Clearly we cannot compute an infinite series - so we have to truncate the series which generates *Truncation Error*, we describe it in terms of the lowest power of $\Delta x$
#### Taylor Series Error
![[Pasted image 20251002131640.png|centre]]
![[Pasted image 20251002131700.png|centre]]
#### Using Taylor Series to Approximate Derivatives
##### Forward/Backward Difference Methods
##### Central Difference Methods
