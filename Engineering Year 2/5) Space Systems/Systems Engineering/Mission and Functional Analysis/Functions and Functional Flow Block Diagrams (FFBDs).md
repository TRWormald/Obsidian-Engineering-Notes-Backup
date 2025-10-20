 [[CONcept of OPerationS (CONOPS)|CONOPS]] provide us a high-level view of the system mission, but this doesn't provide enough detail to actually define it. We therefore need a mechanism to help us to go from the top-level CONOPS to a detailed step of steps that our system must carry out.
One method is using **functions** which are *"A characteristic task, action or activity that must be performed to achieve a desired outcome"*. They can be generated using the steps below:
1) Start with the outputs you are trying to achieve
2) Find other system(s) you need to interact with
3) Find inputs that may be required
4) Write the function
### FFBDs
Within complicated programmes we use FFBDs. To create them we need to define our functions as functional blocks. Each of these blocks will contain an *action word* for our function and any related systems.
Just like requirements, a functional block only shows a single function. For example:
![[Pasted image 20240928113636.png|centre|200]]
This might be an example of a functional block for HLS.
We can now create a FFBD with this functional block using other inputs and outputs:
![[Pasted image 20240928113804.png|centre]]
Note how the *action* words are underlined in these blocks to help identify the steps and make sure only one thing is occurring per block.
Each of these blocks can itself be decomposed into its own FFBD:
![[Pasted image 20240928114008.png|centre]]
### Techniques we can use in FFBDs
1) Gateways - We can capture the outcomes of tests we need to pass in order for the system to continue nominal operations (GO/NO-GO)
2) Parallel Function Paths - In a complex engineering system multiple things will need to happen at the same time. We can show this using an AND block.
3) Conditional Function Paths - Sometimes in nominal operation our system will get to a decision point, were it can respond in more than one way. We can show this using an OR block.
4) Feedback - Sometimes we will need to constantly pass data back so that we know that we are operating nominally, for example a guidance system keeping you on the right track.