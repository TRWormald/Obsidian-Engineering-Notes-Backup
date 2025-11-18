CFD Codes based on domain decomposition are the standard, however scaling of existing CFD is poor - and the efficient use of more than O(1000) cores is only possible for very large niche problems.
Traditional domain decomposition relies on $n$ high-speed inter-node communication. Communication costs quickly become dominant as parallelism increases, which leads to poor utilisation of computing resources.
Fine-grain (thread) parallelism is limited by available memory bandwidth.

### Summary
![[Pasted image 20251118131625.png|centre]]
