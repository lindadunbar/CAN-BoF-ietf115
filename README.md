# Scope and Charter Statement for CAN
The CAN (Computing-Aware Networking) working group (WG) is a home to discuss how computing-related resources, including but not limited to computing and storage capabilities, may impact the routing system. Therefore, new mechanisms and protocol extensions may need to be developed to address the requirements identified in this WG.

Most modern services create multiple service instances that are often geographically distributed in multiple sites, including on-premises or cloud data centers, to scale up the service offering for improving performance. As any of those sites can serve a service, the computing-related conditions at those sites are just as important as the network conditions derived by routing protocols & TE for the service performances. This is especially true in edge computing environments when supporting services such as VR/AR and intelligent transportation, whose traffic may need careful steering due to latency，bandwidth，required computing resource sensitivity, and the mobility. Therefore, joint consideration of network and computing resource status is needed for runtime traffic steering among multiple edge sites, as well as potential service deployment and resource management to meet the demand for optimal user experience. 

There are existing solutions that utilize end point resource information for selecting the server instance, such as DNS, ALTO, or Layer 4 & Layer 7 load balancers. Common to all those solutions is the exposure and usage of network conditions for decision making, while none of the existing solutions integrate the computing resource conditions with the network conditions for deciding on the optimal paths. 

CAN allows ingress nodes to consider computing-related resource conditions in  routing decisions. As such, the CAN WG may develop an informational document, or create a design team, to define use cases, gap analysis, requirements, characterization of the computing-related resources, and how those conditions impact the ingress nodes routing decision process. The findings will enable the CAN WG participants to also study the suitability of existing routing technologies, such as BGP. Further, the potential for extending existing technologies to signal computing information in addition to network conditions will be studied. Ancillary technologies, such as ALTO, NETCONF, OAM, and emerging telemetry proposals, will be investigated as for the purpose of joint computing/networking information collection and usage, so that FCAP (fault, configuration, accounting, performance, security) requirements may be met.

The CAN WG is chartered to work on the following items:

- ### Groundwork may be documented by a design team, or via a set of informational internet-drafts and not necessarily for publication as an RFC:
  - Problem statement for the need for considering both network and computing resource status.
  - Use cases for using the network and computing resource status to benefit the steering of traffic from applications that have a critical SLA that would require the integrated considerations of network-path conditions and computing resources
  - Requirements for commonly agreed computing metrics and their distribution across the network, as well as the appropriate frequency and scope of distribution.
  - Analyze the suitability and usefulness of computing and networking metrics for traffic steering decisions in CAN with a CAN metrics ontology as a possible outcome
  - Analyze methods for distributing the necessary information to utilize the identified metrics in CAN use cases.

- ### Applicability of existing tools and mechanisms
  - Analysis of implementing the CAN control and data plane using existing mechanisms, including identifying the limitations of existing tools in fulfilling requirements 
  - Study potential new approaches for the CAN control and data plane solution that can fill the identified gaps of existing tools and solutions.

- ### Milestones:
  - Jul 2023   Adopt the CAN Problem Statement, Use Cases, gap analysis and Requirements documents
  - Jul 2024   Adopt the CAN framework & architecture document
  - Mar 2025	 Adopt at least one CAN control plane protocol document
  - Mar 2025	 Adopt at least one CAN data plane protocol document
  - Nov 2025   Submit the CAN framework & architecture document to the IESG for publication
  - Mar 2026	 Adopt the CAN OAM, Performance Management (PM), YANG, Protection document
  - Mar 2026   Submit CAN control plane, CAN data plane document to the IESG for publication
  - Nov 2027	 Submit CAN OAM, Performance Management (PM), YANG, Protection document to the IESG for publication
 
