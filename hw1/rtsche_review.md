### 1. Summary

The paper analyze 3 scheduling algorithms for multiprogramming in hard-real-time environments. It outlines five assumptions for the real-time scheduling environment, including strict periodic execution, explicit deadlines, no task dependencies, fixed run time, and absence of aperiodic traffic in the model. The paper demonstrates that the Rate Monotonic (RM) scheduling algorithm is optimal among fixed priority scheduling algorithms, with a minimum processor utilization rate of $ln2$ It also demonstrates that the Earliest Deadline First (EDF) scheduling algorithm is globally optimal and can achieve full processor utilization. Finally, the paper investigates a mixed scheduling algorithm, where two scheduling policies are available for a set of tasks, providing the benefits of deadline-driven scheduling while being easy to implement in existing computers. However, it is proven that the mixed scheduling algorithm cannot achieve full system utilization.

### 2. Contributions

- This paper lays the foundation for the hard real-time scheduling field and continues to be an important reference in the field. Its classical system model, assumptions, and terminology have been widely adopted in the real-time scheduling community.
- The paper provides a theoretical tool for determining the feasibility of tasksets for both dynamic and fixed scheduling algorithms, making it easier to assess their viability without relying on simulation. It also includes practical examples, such as when there are only two tasks in the taskset or when the ratio between request periods is less than 2, and provides the corresponding utilization bounds.
- The paper provides insights into when it is appropriate to use RM, EDF, or a combination of the two, offering valuable guidance to real-time scheduling practitioners.

### 3. Strengths

- The paper presents a well-defined system model for the real-time scheduling problem. The author provides clear mathematical modeling of the problem based on five assumptions, and these assumptions are explained well in terms of their realistic application.
- The paper is well-structured and easy to follow, with a clear and concise presentation of the proofs for RM and EDF scheduling algorithms. The author uses a step-by-step approach, starting with special cases and gradually building up to the general case, making the proof accessible even to readers with limited mathematical background. The analysis of the minimum upper bound based on the critical time zone boundary case is also noteworthy.
- The proposed idea of a mixed scheduling policy is both novel and practical. The author recognizes the limitations of existing computer hardware and acknowledges that current interrupt hardware acts as a fixed-priority scheduler, which is incompatible with dynamic scheduling algorithms. The proposed mixed policy provides a way to take advantage of the benefits of dynamic scheduling while being easily implementable in existing computers.

### 4. Weakness

- Some of the constraints presented in the model are too strong for practical real-world applications. For example, in process control and monitoring systems, tasks may have long periods with strict time requirements, or short periods with large deadlines, which are not covered by the assumptions of the model. Additionally, the preemption mechanism proposed by the model may not be straightforward to implement in real-world systems.

- The paper does not fully investigate some important special cases. For example, when all tasks within a task set are harmonic, the utilization bound for RM can be further reduced, as later proved by Kuo and Mok. This lack of investigation limits the practical applicability of the results.

- The algorithms presented in the paper only apply to dedicated resources and do not take into account the scheduling of shared resources. In practice, a utilization analysis tool that is designed to handle partitioned resources with defined interfaces may be more useful.

- The paper only considers single-core scheduling and is not applicable to tasks with dependencies, such as those encountered in multi-hop traffic scheduling. This narrow focus limits the practical application of the results."

  



