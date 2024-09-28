### The V-Model
All systems have a lifecycle, from the first observation of the problem to the final implementation of the solution to eventually retirement.
The V-Model walks us through this lifecycle rather neatly and is shown in the figure:
![[Pasted image 20240912210321.png|400|center]]
**But what are the key points of the V-Model?**
1) **Lifecycle**:
   All projects start with a *need*, a problem we want to solve. We must figure out what our system must do to solve this problem before we can start any design work.
   We then move onto what functions the system must perform to solve the problem.
   Design is the process of identifying *how* the system will achieve the functions.
   Once the system is designed we can begin to test it to see if it  achieves what we wanted and solves our original problem.
2) **Problem Break-Down and System Build-Up**:
   By starting from a need we can then break this need down into requirements.
   These are then decomposed and distributed to specific subsystems and ultimately components.
   This involves asking "What do we need to build?" at ever deeper levels.
   As we implement the system we work up through the levels of subsystems testing as we go.
   The build-up phase then asks "Have we built what we needed?"
3) **Iteration**:
   All engineering requires iteration and feedback, leading to a non-linear path through systems development.
   You can see that there is iterative feedback between each stage of the V-Model. When defining and decomposing the system, we find that investigating the problem helps us define the solution, but a defined solution often leads to more questions about the problem, so we iterate. When implementing the system, we often find that testing highlights elements of the system that need to be modified, after which we re-test the system.
   
The final consideration that we need to make is the end of a system's life and how this will be handled - we often suffer the repercussions of a lack of this consideration due to the lack of emphasis on it historically. 