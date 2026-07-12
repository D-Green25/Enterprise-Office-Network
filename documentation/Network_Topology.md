# Network Topology and Design

## Overview

The enterprise network was designed using a layered architecture to represent a realistic business environment. The network consists of access switches, a core switch, routers, a firewall, servers, wireless devices, and client devices.

The overall communication path is:
End Devices
|
Department Switches
|
Core Switch
|
Office Router
|
ASA 5505 Firewall
|
ISP Router
|
Internet Cloud


## Network Components

### Switches

Department switches provide connectivity for users and devices within each department. These switches connect end devices such as:

- Desktop computers
- Laptops
- Printers
- Wireless access points

The department switches connect to the core switch, which provides centralized network communication.

### Core Switch

The core switch acts as the central connection point between department networks. It forwards traffic between access switches and the routing layer.

### Office Router

The office router provides inter-VLAN routing using router-on-a-stick configuration. It allows devices from different VLANs to communicate while maintaining network segmentation.

### ASA 5505 Firewall

The ASA 5505 firewall provides security between the internal network and external networks.

The firewall performs:

- Traffic filtering
- Network security
- NAT translation

### ISP Router

The ISP router represents the external service provider connection and provides connectivity toward the Internet Cloud.

## Wireless Network

Wireless connectivity was implemented using a Cisco access point. Laptops and smartphones were configured to connect securely using wireless authentication.
