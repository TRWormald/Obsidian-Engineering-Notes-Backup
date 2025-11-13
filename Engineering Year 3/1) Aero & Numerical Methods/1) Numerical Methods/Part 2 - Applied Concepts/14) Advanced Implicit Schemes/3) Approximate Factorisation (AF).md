### Formulation
Again consider the left-hand side of the equation:
![[Pasted image 20251113132506.png|centre]]
This can be written in terms of difference operators:
![[Pasted image 20251113132522.png|centre]]
This is approximated by a factored form:
$$\left(1+a\frac{\Delta t}{2\Delta x}\delta_{x}\right)\left(1+b\frac{\Delta t}{2\Delta y}\delta_{y}\right)\Delta u_{i,j}^{n}$$
### Error
The difference between the factored and unfactored form of the equations is a term that is no larger than the truncation error in deriving the unfactored form. Multiply out, and that difference is:
![[Pasted image 20251113132729.png|centre]]
The factored form of the method has the same formal accuracy as the original unfactored form. If the set of equations are assembled for each point, the left-hand side now consists of two tri-diagonal matrices, one for the x-derivatives and one for the y-derivatives. It's much quicker to solve two tridiagonal matrices than one containing all the non-zeros.
### Solution Process
Set:![[Pasted image 20251113133028.png|centre]]
Then the factorised implicit system is written as:
$$\mathbf{AB\Delta \underline{u}}=\mathbf{\underline{R}}$$
This is solved in two stages:
$$\mathbf{A\Delta \underline{u}'}=\mathbf{\underline{R}}$$
Followed by:
$$\mathbf{AB\Delta \underline{u}}=\mathbf{\underline{R}}$$