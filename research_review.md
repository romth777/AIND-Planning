# Research Review
## STRIPS
### Research contents
 * STRIPS is the Stanford Research Institute Problem Solver. It is one of the autoplanning with Airtificial intelligent developped by Richard Fikes et al in 1971.
 * The fundamental problem solver of auto planning.
 * STRIPS is composed by below;
  - Initial state
  - Goal state
  - the group of the action, including precondition and postcondition.
 * STRIPS only run one action in each turn, so solving complex problem is difficult for STRIPS.
### References
 * https://en.wikipedia.org/wiki/STRIPS

## Graphplan
### Research contents
 * Graphplan is the automated planning algorithm developped by Avrim and Merrick in 1995.
 * Graphplan generates the sequence of operation to the goal with input of the planning problem discribed by STRIPS.
 * The name of "Graph" comes from the data structure of Graphplan to reduce the exploration of the ploblem space.
 * This planner can use in STRIPS style domains.
 * The Planning Graph has the property that make the constraining search quickly.
### References
 * https://en.wikipedia.org/wiki/Satplan
 * https://www.youtube.com/watch?v=RqhSLCfZdys

## Partial Order Planning
### Research contents
* To achieve the goal, it devides the goal to the sub goals which can control in the each actions.
* If you achieve all subgoals in turn, you can achieve a goal.
* Especially by the space of choice, the sub-goal set with backward flow from the goal.
* Treat the conflict with logical method which check the past state and present state can be connect with action operator, and this is the pros to the totally order planning.
### References
 * https://classroom.udacity.com/courses/ud409/lessons/1922019281/concepts/19409590450923
 * http://pages.cs.wisc.edu/~dyer/cs540/notes/pop.html
 * https://en.wikipedia.org/wiki/Partial-order_planning
