This approach obtains the change in the solution over a time-step in multiple stages. (Also called the method of fractional steps)
Consider again the BTCS scheme for the 2D scalar equation:
![[Pasted image 20251113131555.png|centre|350]]
First, a half step of $\frac{\Delta t}{2}$ is used to solve:
![[Pasted image 20251113131633.png|centre|350]]
Notice only the $x$ derivative is implicit (the y derivative is at the known time level); this means there are only three unknowns per row, and hence a tri-diagonal matrix.

After the first fractional step (implicit in x), the implicit time step is completed by solving a second system, now only implicit in y (since the x derivative is at the known fractional time level):
![[Pasted image 20251113131802.png|centre]]

We have obtained an approximate 2D solution for the price of two tridiagonal matrix solutions. Importantly this is much less computational work than solving the full matrix all in one go.

>**Alternating Direction Implicit (AD)**
>Solve the implicit system by using differences in each direction separately - we alternate between x- and y-differences.

### Cost Savings
Let's now compare the cost between the full system solution and using ADI in 2D. For a full solution of an $NI\times NJ$ mesh we would store matrix with the index with the smallest number first. If $NI$ was smallest we would have:
$$N_{op}=\frac{1}{12}(b^{2}-1)(3n-b)=\frac{1}{12}((2NI+1)^{2}-1)(3(NI\cdot NJ)-(2NI+1))$$
For an ADI, we would have:
$$N_{op}=\frac{1}{12}(3^{2}-1)(3(NI\cdot NJ)-3)$$
for the $i$ direction. Then we would store the matrix with $j$ varying first, and so followed by:
$$N_{op=\frac{}1}{12}(3^{2}-1)(3(NI\cdot NJ)-3)$$
![[Pasted image 20251113132252.png|centre]]
