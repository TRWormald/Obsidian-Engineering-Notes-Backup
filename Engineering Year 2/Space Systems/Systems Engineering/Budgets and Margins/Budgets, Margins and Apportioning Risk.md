"Constraints" are requirements that dictate how much of a given quantity our systems will have. Some examples of constraints include, but are not limited to:
- Physical Size
- Mass
- Time
- Available Power
- Fuel/Propellant
- Cost
- Data Transmission Rates
**In fact, any quantitative aspect of our system is likely to be constrained!**
### Engineering Budgets
A budget is effectively the sum of elements within our system that will be constrained by an aspect of our system. A good example would be electrical power, the sum of the wattages of all of the electronics in our system is the "power budget" and it has to be less than the "Available Power" constraint.
We typically take a bottom up approach to calculating budgets - finding the maximum possible requirements (i.e. including margins) and summing them to get the required budget.
However known constraints (for example the maximum lift capacity of a launcher) might inform our budgeting and design in such a way that we limit the mass accordingly.
\
*Budgets provide a record of how physical quantities are used up across a system design. It is the System Engineers' job to manage the budgets both in a top-down manner by taking system level constraints and decomposing them across the system design, and in a bottom-up approach by adding up each system element's contribution to the physical quantity.*

### Margins
Contingency, Margins, CBE, and MEV are all terms which effectively refer to the "safety factor" within our system budget. MEV for instance is the "Maximum Expected Value" which is 30% greater than the predicted amount required.
The reason why we do this is multi-faceted:
1) Until we have built and tested the system any physical quantity relating to our system is just an estimate and hence full of uncertainty.
2) System development can take years - and stakeholders may wish to add more features on top as time goes on, so having additional bandwidth or power budget may prove useful
3) When dealing with safety critical systems we must account for "known unknowns" and "unknown unknowns" - safety factors are frequently used to provide additional margin to stop us ever observing failure.
\
We can calculate the margin using the following equation:
$$\text{Margin \%}=\frac{\text{Constraint Value - Current System Estimate}}{\text{Current System Estimate}}\times 100\%$$
### Timelines
Timeline analysis is where functional analysis and budgets combine - it is very important when, for example, you have 100W of power generation but you want to complete an experiment that requires 900W of power (as is the case for some of Perseverance's  experiments) this requires careful use of the rover's batteries.
### Managing Risk
Budgeting can also be applied to the safety of our system and any risks that we may face on an engineering programme and project.
Let's define some key terms:
**Hazard -** a state or set of conditions, known as a failure mode, internal or external to the system/project that has the potential to cause negative effects.
**Risk -** The potential for shortfalls, which may be realised in the future, with respect to achieving an intended outcome.
**Occurrence -** The likelihood of a hazard occurring.
**Severity -** The impact on the system/project of the hazard.
\
The first stage of prioritising risk is to think carefully about our failure mode, to establish the probability it will occur (occurrence), the impact it would have on the system (severity) but also whether we would have any warning or be able to know where the failure mode had come from (detectability).
For each identified Hazard, the scores for occurrence (O), severity (S) and detectability (R) will be defined.
We then combine the O, S, and D values into a Risk Priority Number (RPN) using:
$$RPN=O\times S\times D$$
If the RPN is too high then we have to take action to rectify it.