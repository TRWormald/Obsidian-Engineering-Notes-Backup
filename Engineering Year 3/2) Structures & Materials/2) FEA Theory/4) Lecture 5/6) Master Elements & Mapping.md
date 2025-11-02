Master elements are defined in natural coordinates. These coordinates span unit domains, e.g.:
$$-1\le\xi\le 1$$
$$-1\le(\xi,\eta)\le1$$
![[Pasted image 20251024153634.png|centre|400]]
### Mapping
To map the elements from the natural coordinates onto the global reference system and vice versa, we require an invertible transformation of the form:
$$x=f(\xi)$$
An example for a straight 1D element of length $L$ with two nodes is:
$$f(\xi)=x_{a}+ \frac{1}{2}L(1+\xi)$$
$f(\xi)$ is linear. Hence, a straight line is transformed into a straight line.
In general, the domain of integration can have more complex shapes than just a line. If the element's shape is curved, a nonlinear function can map the segment onto the more complex geometry.

A systematic way of creating the map involves approximating the geometry of the element as we approximated the dependent variables. Recall:
![[Pasted image 20251024153933.png|centre|200]]
![[Pasted image 20251024154000.png|centre]]
### Isoparametric Formulations
![[Pasted image 20251024154032.png|centre]]
### Mapping
For more information on mapping refer to the notes starting on [[FEA Theory - Lecture 5.pdf#page=48|FEA Theory - Lecture 5, p.48]].
