Static and Default Routing Lab

1. Project Overview

This project demonstrates Static Routing and Default Routing configuration between two different LAN networks using Cisco routers in GNS3.

The main goal is to establish end-to-end connectivity between devices located in different networks.

2. Network Topology

The topology consists of:

- Two Cisco Routers (R1 and R2).
- Two Layer 2 Switches (SW1 and SW2).
- Four end devices (PC1, PC2, PC3, and PC4).
- An Ethernet connection between R1 and R2.

"Network Topology" (Topology/topology.png)

3. IP Addressing Table

Device| Interface| IP Address| Subnet Mask
R1| G0/0| 192.168.1.1| 255.255.255.0
R1| G0/1| 10.0.0.1| 255.255.255.252
R2| G0/0| 10.0.0.2| 255.255.255.252
R2| G0/1| 192.168.2.2| 255.255.255.0
PC1| NIC| 192.168.1.10| 255.255.255.0
PC2| NIC| 192.168.1.11| 255.255.255.0
PC3| NIC| 192.168.2.10| 255.255.255.0
PC4| NIC| 192.168.2.11| 255.255.255.0

4. Default Gateway Configuration

- LAN 1 Default Gateway: 192.168.1.1
- LAN 2 Default Gateway: 192.168.2.2

5. Static Routing Configuration

On R1:

ip route 192.168.2.0 255.255.255.0 10.0.0.2

On R2:

ip route 192.168.1.0 255.255.255.0 10.0.0.1

6. Default Routing Configuration

A default route was configured on R2 to forward traffic for unknown destinations toward R1.

On R2:

ip route 0.0.0.0 0.0.0.0 10.0.0.1

7. Verification and Testing

The following commands were used:

show ip interface brief
show ip route
show running-config

Connectivity was tested using ICMP Ping.

Examples:

ping 192.168.2.10
ping 192.168.2.11

Successful ping responses confirm connectivity between the two LAN networks.

8. Technologies and Concepts

- Cisco IOS
- GNS3 Network Simulator
- IPv4 Addressing and Subnetting
- Static Routing
- Default Routing
- Routing Table Verification
- ICMP and Ping Testing
- End-to-End Connectivity

9. Configuration Files

- "Configurations/R1.txt" – R1 running configuration.
- "Configurations/R2.txt" – R2 running configuration.

10. Learning Outcomes

- Understanding router-to-router communication.
- Configuring static routes using next-hop addresses.
- Understanding default route functionality.
- Reading and verifying routing tables.
- Testing end-to-end connectivity between different networks.