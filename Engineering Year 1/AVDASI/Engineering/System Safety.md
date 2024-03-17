Aircraft types have a **type approval** or **type certificate** which assures the adequacy of the design work.
Specific aircraft have **certificates of airworthiness**. A requirement for this is a type certificate. This assures the adequacy of the aircraft (e.g. maintenance, repairs, etc). This is an ongoing obligation for each aircraft.  
#### Hazard and Risk Assessment Process
The process for dealing with risk is as follows:
![[Pasted image 20240311104047.png|center|400]]
We define risk as:
$$Severity \times Likelihood = Risk$$
The severity of any event fits into the following categories:
![[Pasted image 20240311104352.png|center|500]]
Whilst likelihood is defined as follows:
![[Pasted image 20240311104428.png|center|500]]
The following table shows the relationship between the severity and probability of failures:
![[Pasted image 20240312123107.png]]
#### Types of Failure
There are two main types of failure:
**Systematic Failure:**
- These failures will always occur for a given set of conditions. They are repeatable and *potentially* predictable
- For example software 'bugs' - once the code is written the potential for failure is intrinsic to the system
- These are hard to mitigate for and difficult to analyse with rigor, in many cases accidents happen because of events or behaviour that were not foreseen
- The primary approach is to try and design out this type of fault.
**Random Failures**
- These failures occur during normal operation and are not repeatable or predictable, but can be dealt with analytically using probability.
- For example a light bulb blowing
- Once extensive testing has determined the probability of failure then reliability analysis can be used to ensure the probability of failure is within acceptable bounds.

#### Design Safety Features
##### Process Assurance
This is where cross checking us used in the development process, helping to uncover systematic errors:
![[Pasted image 20240311111054.png|center]]
#### Architectural Safety Features
##### Redundancy
Redundant architectures provide mitigation for random failures, two (or more) systems provide the same functionality.
There are different types of redundancy:
![[Pasted image 20240311111610.png|center|525]]
#### Dissimilar Redundancy
This is mitigation for common mode systematic failures and can be achieved by using dissimilar hardware/software for each channel.

