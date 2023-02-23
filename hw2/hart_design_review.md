### 1. Summary

This paper proposed the design principle of a time-triggered low-power real-time wireless network, so called wirelessHART and introduced the challenges and the potential soluiton and implementations to address those challenges. The experiences and lessons learned from the design of this protocol is discussed in detail. One real-world prototype testbed is built for the demonstration. That author claims that this is the first paper indroducing how to build a WirelessHard protocol stack.

### 2. Contributions

- Introduction of the architecture of WirelessHART. Identified the required features for wireless real-time application.
- A real implementation of wirelessHart. Some key challenges are indentified and solved during the real implementation.
- The real experiences are lessons learned during the implementation.

### 3. Strengths

- The protocol supports a unified transportation layer protocol for both wired and wireless network, which is very convenient for industry to form a hetongenous network with both backbone wired network and production line wireless network.

### 4. Weakness

- The selection of granularity of 10ms time slot defined in the standard is not well explained. Also how to select the length of superframe is also not well explained in the paper. Those parameters should have great impact on the scheduling model and scheduling algorithms.
- 

