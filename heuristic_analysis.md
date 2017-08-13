# Heuristic Analysis
## Abstract  
This documents include my experiment of heuristic and non-heuristic planning searches. The algorithms are on the list below;
 - Uninformed algorithms
  * breadth_first_search(BFS)
  * breadth_first_tree_search(BFTS)
  * depth_first_graph_search(BFGS)
  * depth_limited_search(DLS)
  * uniform_cost_search(UCS)
 - Informed algorithms
  * recursive_best_first_search with h_1
  * greedy_best_first_graph_search with h_1
  * astar_search with h_1
  * astar_search with h_ignore_preconditions
  * astar_search with h_pg_levelsum

There are two types of algorithms, one is Uninformed, and the other is Informed. Uninformed algorithms do not take the knowledge of this problem, i.g. h_1, h_pg_levelsum and so on. The Uninformed algorithms do not contract with the problem so that we can use it any problem field of search, but generally, it needs the delay of elapsed time to find the solution. In spite of Uninformed algorithm, Informed algorithms use the knowledge of the problem using evaluate the function of h_1 or and so on. It is faster than Uninformed one if you choose a good evaluation function.
<div style="page-break-before:always"></div>

## My result
### Air Cargo Problem 1
![image1](images/image1.JPG)
#### Comments
 * "depth_limited_search" and "depth_first_graph_search" are not optimally, because it could not find plan of length 6.
 * "recursive_best_first_search" takes time to get solution, it might be this problem is not only based on the cost of deistance, so if we improve this, we should take the other cost value.
 * The other search method looks good to me especially "breadth_first_search" and "astar_search" looks optimal.
<div style="page-break-before:always"></div>

### Air Cargo Problem 2
![image2](images/image2.JPG)
#### Comments
 * "breadth_first_tree_search", "depth_limited_search" and "recursive_best_first_search" could not reach to the solution for calculation time.
 * "depth_first_graph_search" and "greedy_best_first_graph_search" could not take the optimal solution which is 9 length, because the problem space is more bigger than Problem 1.
 * "astar_search with h_pg_levelsum" could reach the optimal solution, however the elapsed time to get there is delayed.
 * The other search method looks nice to me especially "astar_search with h_ignore_preconditions" looks optimal.
<div style="page-break-before:always"></div>

### Air Cargo Problem 3
![image3](images/image3.JPG)
* "breadth_first_tree_search", "depth_limited_search" and "recursive_best_first_search" could not reach to the solution for calculation time.
* "depth_first_graph_search" and "greedy_best_first_graph_search" could not take the optimal solution which is 12 length, because the problem space is more bigger than Problem 1.
* "astar_search with h_pg_levelsum" could reach the optimal solution, however the elapsed time to get there is delayed.
* The other search method looks nice to me especially "astar_search with h_ignore_preconditions" looks optimal.
<div style="page-break-before:always"></div>

## Conclusion
 * The most recommendable algorithm is "astar_search with h_pg_levelsum" in reaching to the optimal solution and time elapsed.
 * The other method which can take in the solution seems like a good but the time is not optimal in this experiments.
 * In all cases, "depth_first_graph_search" and "depth_limited_search" could not reach the optimal solutions. I think this is because depth first search algorithm is not suitable for this type of problem. This type of problem can take many patterns and deeper nodes with the meaningless movement of airplane i.g. "To make a round-trip unnecessarily." That's why the optimal solution is not in the thick node of the problem space, and the depth first search did not work well on this issue.
