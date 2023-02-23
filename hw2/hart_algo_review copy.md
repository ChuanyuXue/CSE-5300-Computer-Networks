- ### 1. Summary

  The paper presents a real-time scheduling formulation for WirelessHART networks and proves that it is NP-hard. The paper proposes both an optimal and a heuristic algorithm to solve this problem, and simulation experiments show that the heuristic algorithm is efficient in solving the problem and effective in meeting the end-to-end communication deadline requirements.

  ### 2. Contributions

  The paper's contributions include:

  - Formulating the real-time transmission scheduling problem based on the characteristics of WirelessHART networks and proving that it is NP-hard.
  - Identifying and proving the necessary condition for WirelessHART real-time scheduling, which can be used to prune the searching space and provide insight for the heuristic-based solution.
  - Proposing both optimal and heuristic solutions to the scheduling problem.

  ### 3. Strengths

  The paper has several strengths, including:

  - The paper is well written and presents the problem formulation, approach, and technical details effectively. The methods proposed are well verified by extensive experiments.
  - The paper provides a necessary condition for schedulability of real-time tasks in WirelessHART networks. This condition is important because it allows us to determine whether a set of real-time tasks can be scheduled on a WirelessHART network without actually performing the scheduling. This condition can be used to prune the searching space and provide insight for the heuristic-based solution.
  - The simulation experiments demonstrate the effectiveness of the proposed heuristic algorithm in meeting the end-to-end communication deadline requirements.

  ### 4. Weaknesses

  However, the paper has some weaknesses, including:

  - The necessary condition for schedulability is too obvious by only considering the utilization and release/deadline of the task set. It is unclear whether filtering based on this feasible condition can significantly improve the searching efficiency. It would be helpful to see an experiment or complexity analysis discussing this. It is well known that considering the periodicity of non-preemptive hard real-time tasks can significantly reduce the solving space.
  - The paper lacks experiment results comparing the branch-and-bound algorithm without the filtering to provide a better comparison with the proposed heuristic algorithm.

  Overall, the paper makes a valuable contribution by formulating and solving the real-time scheduling problem for WirelessHART networks. However, some areas could be improved to provide more information and better support the proposed solution's effectiveness and efficiency.
