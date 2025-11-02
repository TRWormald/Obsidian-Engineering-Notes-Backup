There are two broad classes of mesh type - Structured and Unstructured.
#### Structured Meshes
In a structured mesh grid lines in each coordinate direction are indexed by $i,~j,~k$ integer indices. Every line in each family has the same number of points as every other line in the same family.
![[Pasted image 20251021130445.png|centre|300]]
#### Unstructured Meshes
In an unstructured mesh there is no logical or regular structure to grid point arrangement. Connectivity between points, faces, and cells needs to be specified for every element.
![[Pasted image 20251021130539.png|centre|300]]
#### Comparing Mesh Types

| Structured Meshes                                                                                      | Unstructured Meshes                                                                                                             |
| ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------- |
| Simple data structure                                                                                  | Easier to generate for complex geometries                                                                                       |
| Regular (fast) data access                                                                             | Easy to apply automatic refinement                                                                                              |
| Neighboring points are known implicitly                                                                | <font color="#ffffff"><span style="background:#ff4d4f">Connectivity data needs to be computed and stored</span></font>          |
| <font color="#ffffff"><span style="background:#ff4d4f">Difficult and user-intensive generation process | <font color="#ffffff"><span style="background:#ff4d4f">Lower quality than structured grid worse for viscous flows</span></font> |
>Also note that a mesh that has been generated as a structured mesh, can be stored as an unstructured mesh - but not vice versa.

