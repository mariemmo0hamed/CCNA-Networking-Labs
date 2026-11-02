# Basic Switching and VLANs Lab

## Overview
This lab demonstrates basic switching and routing concepts using GNS3.

## Network Topology
Two multilayer switches (SW1 and SW2) connected through an LACP EtherChannel.

![Topology](Topology/topology.png)

## VLAN Configuration

| VLAN ID | Name |
|---|---|
| 10 | IT |
| 20 | HR |
| 99 | Management |

## Implemented Technologies
- Basic Switch Configuration
- VLAN Creation and Assignment
- Access and Trunk Ports
- Native VLAN and Allowed VLANs
- Inter-VLAN Routing
- Spanning Tree Protocol (STP)
- Root Bridge Election
- EtherChannel (LACP)
- Port Security

## Configuration Files
- SW1.txt
- SW2.txt

## Tools
- GNS3
- Cisco IOS