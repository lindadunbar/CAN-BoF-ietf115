# Suggested Charter Statement for CAN
Suggested Charter Statement for CAN
The CAN (Computing-Aware Networking) WG is a home to discuss topics related to computing-aware routing in IETF and to gain an understanding of the problems and use cases, as well as to understand the applicability of existing tools and techniques. Where necessary, new architectures and mechanisms will be developed to address the problem space.

Most modern services create multiple service instances that are often geographically distributed in multiple on-premise or cloud data centres, to offset the load and scale up the service offerings. Solutions to steer traffic towards those (distributed) service instances normally use request/response-based methods to achieve multi-site load-distribution at either the application layer or the transport level. However, this requires additional message exchanges among controllers and service instances before an optimal service instance can be selected. This results in additional delay that often fails to meet the requirements of low latency and high efficiency services, such as real-time or near real-time applications, while also incurring costs for signaling as well as maintaining the required indirection infrastructure.

Computing-aware networking is the approach of dynamically steering service traffic through an on-path service-instance selection by considering both the resource status of computing servers and network path metrics. This differs from existing standalone application-layer or transport-level schemes. 

The CAN WG will discuss the use cases, architecture, and solutions to of computing-aware networking. There are some existing routing technologies in IETF such as ECMP, a Layer 3 Load Balancing based forwarding, and there has been lots of work on entropy-based and flow affinity forwarding. CAN will study and evaluate these mechanisms to identify the ones that can be used or enhanced with the objective of avoiding making modifications or introducing new solutions when possible, and in any case to ensure that all approaches are compatible with existing mechanisms. Furthermore, CAN will align the design principles for its architecture with that of LISP, which addresses a similar problem of separating service identification from network locations. The difference of CAN lies in its focus on the logics and inputs applied in the traffic steering decision itself, which in turn must be maintained across one or more such traffic steering decision to avoid disruptions of longer-lived service transactions in order for ingress nodes to select the optimal instances jointly based on both network parameters of transport paths and real-time or near-real-time resource conditions or metrics at the destination service instances. 

The CAN working group is chartered to work on the following items:
- ### Groundwork
  - Problem statement for the need for dynamically steering traffic based on existing deployments of computing resources.
  - Use cases for applications that have a critical SLA that would require the integrated considerations of network-path conditions and computing resources, and the overall load balance among the computing resources
  - Requirements for dynamically steering traffic across multi computing sites, flexibly using multi- metrics and maintaining flow affinity
  - Architecture that supports making instance/site selection considering both the metrics of network paths & computing resources
  - Analyse computing and networking metrics as to their suitability and usefulness for traffic steering decisions in CAN with a CAN metrics ontology as a possible outcome
  - Analyse and devise methods of signalling the necessary information for utilizing the identified metrics in traffic steering decisions in CAN
- ### Applicability of existing tools and mechanisms
  - Realization of the CAN control and data plane using existing mechanisms
  - Analysis of limitations of existing tools in fulfilling requirements
  - Study potential new approaches for a CAN control and plane solution that may fill the identified gaps of existing tools and solutions.
  - Study furthermore mechanisms for 
    - CAN OAM, Performance Management (PM), YANG, Protection, etc.
    - Instance affinity to avoid session interruption.
    - Add-on capabilities, such as mobility support, both in terms of client and service mobility, or transport layer security optimizations in multi-instance environments. 


- ### Milestones:
  - Nov 2025	Submit CAN OAM, Performance Management (PM), YANG, Protection document to the IESG for publication
  - Mar 2025	Submit CAN control plane, CAN data plane document to the IESG for publication
  - Mar 2025	Adopt the CAN OAM, Performance Management (PM), YANG, Protection document
  - Jul 2024  Submit CAN modeling, metrics and representation document to the IESG for publication
  - Jul 2024  Submit the the CAN Architecture document to the IESG for publication
  - Mar 2024	Adopt at least one CAN data plane protocol document
  - Mar 2024	Adopt at least one CAN control plane protocol document
  - Nov 2023  Submit the CAN Problem Statement, Use Cases, gap analysis and Requirements document to the IESG for publication
  - Nov 2023	Adopt the CAN modeling, metrics and representation document		
  - Nov 2023	Adopt the CAN Architecture document	
  - Jul 2023  Adopt the CAN Problem Statement, Use Cases, gap analysis and Requirements documents
