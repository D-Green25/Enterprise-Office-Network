# IP Addressing Plan

## Overview

Private IP addressing was used for internal networks. Each VLAN was assigned its own subnet to maintain separation between departments.

## Addressing Scheme

| Network | Purpose |
|---------|---------|
| 192.168.10.0/24 | VLAN 10 |
| 192.168.20.0/24 | VLAN 20 |
| 192.168.30.0/24 | VLAN 30 |
| 192.168.40.0/24 | Server Network |

## External Network

The ASA firewall connects to the ISP router using a separate external network.

Example:

- ASA Outside Interface: 203.0.113.2
- ISP Router Interface: 203.0.113.1

NAT allows internal private addresses to communicate externally.
