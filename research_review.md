# Research Review
## STRIPS
### Research contents
 STRIPS is the Stanford Research Institute Problem Solver. It is one of the auto planning with Artificial intelligent developed by Richard Fikes et al. in 1971. The first problem solver of automated planning. STRIPS compose below;
  - Initial state
  - Goal state
  - the group of the action, including precondition and postcondition.
 STRIPS only run one action in each turn, so solving a complex problem 's hard for STRIPS.
### References
 * https://en.wikipedia.org/wiki/STRIPS

## Graphplan
### Research contents
Graphplan is the automated planning algorithm developed by Avrim and Merrick in 1995. Graphplan generates the sequence of operation to the goal with the input of the planning problem described by STRIPS. The name of "Graph" comes from the data structure of Graphplan to reduce the exploration of the problem space. This planner can use in STRIPS style domains. The Planning Graph has the property that does the constraining search quickly.
### References
 * https://en.wikipedia.org/wiki/Satplan
 * https://www.youtube.com/watch?v=RqhSLCfZdys
<div style="page-break-before:always"></div>

## Partial Order Planning
### Research contents  
Partial Order Planning is an approach to automated planning; it decides the order of the actions as open as possible. To achieve the goal, it divides the goal to the sub goals which can control the each action. If you make all subgoals, in turn, you can achieve a goal. In particular by the space of choice, the sub-goal set with backward flow from the goal. Treat the conflict with the logical method which checks the past state, and it can connect the current status with action operator, and this is the pros to the order planning.
### References
 * https://classroom.udacity.com/courses/ud409/lessons/1922019281/concepts/19409590450923
 * http://pages.cs.wisc.edu/~dyer/cs540/notes/pop.html
 * https://en.wikipedia.org/wiki/Partial-order_planning
