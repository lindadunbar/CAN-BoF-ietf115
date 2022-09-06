# Suggested Charter Statement for CAN
Suggested Charter Statement for CAN
The CAN (Computing-Aware Networking) WG is a home to discuss topics related to computing-aware routing in IETF and to gain an understanding of the problems and use cases, as well as to understand the applicability of existing tools and techniques. Where necessary, new architectures and mechanisms will be developed to address the problem space.

Most modern applications create multiple service instances that are often geographically distributed in multiple Data Centers, either on-premises or in the cloud, to offset the load and scale up the service offerings. These solutions normally use the request/response-based solutions to achieve the multi-site load-distribution at either the application layer or the transport level. However, this requires additional message exchanges among controllers and service instances before an optimal service instance can be selected. This results in additional delay that often fails to meet the requirements of low latency and high efficiency services, such as real-time or near real-time applications.

Computing-aware networking is the process of dynamically steering service traffic to achieve better on-path service-instance selection by considering both the resource status of computing servers and network path metrics. This differs from existing standalone application-layer or transport-level schemes. 

The CAN WG will discuss the use cases, architecture, solutions and other related topics of computing-aware networking. There are some existing routing technologies in IETF such as ECMP, a Layer 3 Load Balancing based forwarding, and there has been lots of work on entropy-based and flow affinity forwarding. CAN will study and evaluate these mechanisms to identify the ones that can be used or enhanced with the objective of avoiding making modifications or introducing new solutions when possible, and in any case to ensure that all approaches are compatible with existing mechanisms. The goal is for ingress nodes to select the optimal instances holistically based on both network parameters of transport paths and real-time or near-real-time resource conditions or metrics at the destination service instances, e.g., computing power or application servers. 

The CAN working group is chartered to work on the following items:
- ### Groundwork
  - Problem statement
  - Use cases 
  - Architecture
  - Abstract metrics and parameters to describe characteristics
- ### Applicability of existing tools and mechanisms
  - Immediate delivery of simple services using existing mechanisms
  - Analysis of limitations of existing tools for delivering advanced services
  - Consideration of potential to extend existing tools or requirements for new protocol solutions.

Subject to the outcomes of these initial work items, the CAN working group may be rechartered to work on specific protocol solutions for IPv6 and MPLS networks.”


Milestones:
TBD
