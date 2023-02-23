### 1. Summary

The paper presents WirelessHART, a time-triggered low-power real-time wireless network protocol. It discusses the challenges involved in designing such a protocol and proposes potential solutions to address them. The paper describes the architecture of the protocol, along with its features, and provides a detailed account of the experiences and lessons learned during the protocol's implementation. The paper also presents a real-world prototype testbed to demonstrate the protocol's feasibility.

### 2. Contributions

The paper makes several contributions, including:

- Introducing the architecture of WirelessHART and identifying the required features for wireless real-time applications.
- Presenting a real implementation of WirelessHART and identifying and solving key challenges during the implementation.
- Providing insights into the experiences and lessons learned during the implementation.

### 3. Strengths

The paper has several strengths, including:

- WirelessHART supports a unified transportation layer protocol for both wired and wireless networks, making it convenient for the industry to form a heterogeneous network with both backbone wired network and production line wireless network.
- Instead of only fulfilling the real-time requirements by introducing time-triggered scheduling mechanism into wireless network, this paper also solved the security issue by using four security keys (public key, network key, join key, and session key) for different usage.
- The paper proposes a solution that combines synchronous and asynchronous timer interruption to guarantee both precise time-triggered and event-triggered processing and avoid timeouts.

### 4. Weakness

However, the paper has some weaknesses, including:

- The synchronization procedure seems too simple, and the paper does not explain some real challenges, such as how to infer the link delay and the error in the time recording of the first bit of DLPUD message when correcting the local clock. The TsTxOffset is not defined previously in the paper.
- The paper does not explain the selection of granularity of the 10ms time slot defined in the standard, which could have a significant impact on the scheduling model and scheduling algorithms. Similarly, the paper does not provide enough information on how to select the length of superframe.
- The paper lacks measurement results comparing the quality of service (QoS) metrics between WirelessHART and existing solutions like Zigbee.

Overall, the paper makes a valuable contribution by presenting a novel protocol for wireless real-time applications and discussing the challenges involved in its implementation. However, some areas could be improved to provide more information and better support the protocol's implementation and adoption.
