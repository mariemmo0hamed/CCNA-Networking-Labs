OSPF Routing

Project Overview

This project demonstrates OSPF (Open Shortest Path First) routing configuration and implementation using GNS3.

The goal is to enable dynamic routing between multiple routers and networks using OSPF.

Objectives

- Configure Single-Area OSPF.
- Configure Multi-Area OSPF.
- Understand OSPF Area Design.
- Configure Area Border Routers (ABRs).
- Verify OSPF Neighbor Adjacencies.
- Verify Dynamic Route Learning.
- Understand Route Redistribution.

Technologies & Tools

- GNS3
- Cisco IOS Routers
- OSPF Routing Protocol
- SecureCRT

Implementation

The lab covers:

1. OSPF process configuration.
2. Router ID configuration.
3. Network advertisement using OSPF.
4. Multi-Area OSPF configuration.
5. OSPF neighbor relationship verification.
6. Routing table verification.
7. End-to-end connectivity testing.

Verification Commands

show ip ospf neighbor
show ip ospf interface brief
show ip route
show ip route ospf
show ip protocols

Testing

Connectivity was tested between devices in different networks using the "ping" command.

Successful ping tests confirmed end-to-end connectivity across the configured OSPF network.

Repository Structure

03-OSPF-Routing/
│
├── README.md
├── Topology/
├── Configurations/
└── Verification/

Key Concepts

- Dynamic Routing
- OSPF Neighbor Adjacency
- Single-Area and Multi-Area OSPF
- Area Border Router (ABR)
- OSPF Route Types
- Route Redistribution

Author

Networking Labs Portfolio