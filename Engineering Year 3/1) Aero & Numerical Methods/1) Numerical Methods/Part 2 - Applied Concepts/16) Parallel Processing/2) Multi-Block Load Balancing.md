If we have more mesh blocks than processors - we need to put more than one block on a processor.
**But what if our blocks each have different numbers of cells?**
- We will have a different number of cells on each processor
- Each processor will take a different amount of time to update solution
- But: must wait for all processors to finish before starting the next iteration
- Therefore time-per-iteration is determined by the processor with the most cells

**Load Balancing**:
For 100% efficiency (ignoring communications) we want all processors to have exactly the same number of cells. Note: an unstructured mesh doesn't have blocks: and therefore you can easily divide the mesh for an arbitrary number of processors.

