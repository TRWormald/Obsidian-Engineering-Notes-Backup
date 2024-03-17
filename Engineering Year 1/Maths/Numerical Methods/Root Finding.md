For many functions we cannot use a simple formula (like the quadratic formula) to determine the roots of the equation (where $f(x)=0$). Instead we can apply numeric methods to estimate and gain approximations of roots.
\
*If an equation involves only continuous computable functions and has no symbolic parameters, then an isolated solution can be approximated numerically to any desired accuracy.*
\
*If $f$ is a computable function and $x'$ is a particular root of $f$ (i.e. $f(x')=0$) then a root finding algorithm computes a value $\hat{x}$ that is hopefully close to $x'$.*
\
A simple way of doing this is iterating values of $x$ until your result switches from positive to negative (or vice versa), which indicates that you have passed over a root. You then continue to choose values between those two points until you get your solution to a reasonable degree of accuracy.
### Bisection Method
The bisection method is the formalisation of the above method:
\
Consider the case where we are trying to find a root of a continuous function $f(x)$. If we are given two x-values, $a_o$ and $b_0$, which have been chosen so that $f(a_0)$ and $f(b_0)$ have opposite signs, then we can find a root using the following iterative method:
1) Let $c_n=\frac{1}{2}(a_n+b_n)$ be the $n$th approximation of the root
2) Look at the sign of $f(c_n)$
	- If $f(c_n)$ has the same sign as $f(a_n)$, then let $a_{n+1}=c_n$ and let $b_{n+1}=b_n$.
	- If $f(c_n)$ has the same sign as $f(b_n)$, then let $b_{n+1}=c_n$ and let $a_{n+1}=a_n$.
3) Return to Step 1 to find the next c value and repeat.

Note that the maximum error in the approximation halves at each step.

