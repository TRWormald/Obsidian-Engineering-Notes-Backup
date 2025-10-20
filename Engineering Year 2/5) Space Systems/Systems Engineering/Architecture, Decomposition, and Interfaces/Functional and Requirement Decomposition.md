We have previously looked at how to decompose a system need into a set of requirements and a Functional Flow Block Diagram. Consequentially, we shouldn't be surprised to find that these are the sources we use to define our architecture.
The first iteration of constructing a system architecture should try to achieve a 1:1 mapping of functions to a sub-system/component element:
![[Pasted image 20241012172657.png|centre]]

This means an architecture is finally starting to define HOW our system will satisfy the system need.
### Derived Requirements
As we go through the definition of a system architecture, we will inevitably start to make assumptions about how our system is going satisfy the requirements placed upon it. This immediately puts us at risk of breaking one of our requirements of written requirements, which is that requirements should be Implementation Independent.
This results in us needing to consider two types of requirement:
![[Pasted image 20241012172841.png|centre]]
On the left-hand side of Figure 19 we can see Traceable requirements and these are requirements that can be directly mapped or decomposed to our sub-system elements without modification. Traceable requirements can also be linked back to system-level requirements based on any budgets we may have defined.
On the right-hand side of Figure 19, the generation of Derived requirements is shown. Derived requirements are those that can only be written, or only appear, once we’ve made some decisions about our system architecture. 
The processes shown in Figure 19 highlight a continual and iterative process that is performed as we make our way down the left-hand side of the V-mode.