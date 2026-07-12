# VLAN Design

## Overview

VLANs were implemented to separate departments into different logical networks. VLAN segmentation improves security, organization, and network performance by reducing unnecessary broadcast traffic.

## VLAN Configuration

| VLAN | Department | Purpose |
|------|------------|---------|
| VLAN 10 | HR | Department Network |
| VLAN 20 | Sales | Department Network |
| VLAN 30 | IT | Department Network |
| VLAN 40 | Servers | Network Services |

## Inter-VLAN Routing

Inter-VLAN communication is handled by the office router using router-on-a-stick configuration.

The router uses subinterfaces:

- GigabitEthernet 0/0.10
- GigabitEthernet 0/0.20
- GigabitEthernet 0/0.30
- GigabitEthernet 0/0.40

Each subinterface acts as the default gateway for its assigned VLAN.

This allows controlled communication between departments while maintaining logical separation.
