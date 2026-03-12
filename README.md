# Network-Lab-SOHO-Routed-Topology

## Overview
A basic routed network topology featuring a central 2911 router connected to two access switches, each supporting a client workstation. This lab demonstrates fundamental networking concepts in a small office environment.

## Device Inventory
- **Router0**: Cisco 2911 integrated services router
- **Switch0, Switch1**: Generic Layer 2 switches
- **PC1, PC3**: Windows-based workstations

## Connection Scheme
- Router0 Gig0/0 → Switch0 Fa2/1
- Router0 Gig0/1 → Switch1 Fa2/1
- Switch0 Fa0/1 → PC1
- Switch1 Fa0/1 → PC3
- Additional connection: Router0 Fa0/0 ↔ Switch1 Fa1/1 (potential redundant link or misconfiguration)

## Lab Objectives
This topology is designed to practice:
- Basic device configuration (hostnames, banners, passwords)
- Interface IP addressing and subnetting
- Static route configuration
- Dynamic routing protocols (RIP, OSPF, EIGRP)
- Switch port security
- VLAN configuration and inter-VLAN routing
- Connectivity testing and troubleshooting

## IP Addressing Scheme (Suggested)
| Device | Interface | IP Address | Subnet Mask | Gateway |
|--------|-----------|------------|-------------|---------|
| Router0 | Gig0/0 | 192.168.1.1 | 255.255.255.0 | N/A |
| Router0 | Gig0/1 | 192.168.2.1 | 255.255.255.0 | N/A |
| PC1 | Fa0 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| PC3 | Fa0 | 192.168.2.10 | 255.255.255.0 | 192.168.2.1 |

## Quick Start Commands
To bring all interfaces up:

**Router0:**
