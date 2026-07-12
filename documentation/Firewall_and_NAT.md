# Firewall and NAT Configuration

## ASA 5505 Firewall

The ASA 5505 firewall provides security between the internal office network and the external ISP network.

The firewall contains:

## Inside Interface

Connected to the office router and internal networks.

## Outside Interface

Connected to the ISP router and external network.

## NAT

Network Address Translation was configured to allow internal devices using private IP addresses to communicate externally.

NAT translates internal addresses into the firewall's outside address.

Benefits include:

- Hiding internal IP addresses
- Conserving public addresses
- Providing controlled external access
