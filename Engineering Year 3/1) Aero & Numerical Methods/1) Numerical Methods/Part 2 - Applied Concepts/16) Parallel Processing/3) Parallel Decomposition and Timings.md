Consider a mesh containing $N\times N$ points, which are distributed uniformly over $P$ processors. Four times are defined:
$t_{proc}$ - time to execute one timestep for one mesh point on the processor
$t_{comms}$ - time required to send the data associated with one boundary mesh point between processors
$t_{global}$ - time for global data transfer
$t_{serial}$ - time for serial part of the code

As a rough estimate, the total time to compute a single timestep on the parallel computer is thus the sum of these times, or:
$$T_{N}(P) = \frac{N^{2}}{P}t_{proc}+\frac{N}{\sqrt{P}}t_{comms}+\log(P)t_{global}+t_{serial}$$
The speedup, $S_{N}(P)$, is the ratio of the time to execute a problem of size $N$ on one processor to the time to execute the same problem on $P$ processors:
$$S_{N}(P)=\frac{T_{N}(1)}{T_{N}(P)}$$
![[Pasted image 20251118133205.png|centre|350]]
The efficiency of parallelisation is $\eta$ :
$$\eta=\frac{S_{N}(P)}{P}$$
![[Pasted image 20251118133249.png|centre|350]]
![[Pasted image 20251118133626.png|centre]]
![[Pasted image 20251118133636.png|centre]]
