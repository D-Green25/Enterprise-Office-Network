# Testing and Analysis

## Connectivity Testing

Network functionality was verified using ping tests.

Tests included:

- PC to default gateway
- PC to servers
- Router communication
- ASA firewall communication
- ISP router communication

Successful ping responses confirmed proper routing and connectivity.

## Browser Testing

HTTP communication was tested by accessing the internal web server through a client browser.

This verified that application-layer services were functioning.

## Wireshark Analysis

Wireshark was used to analyze network traffic.

Captured protocols included:

### ARP

Used to map IP addresses to MAC addresses.

### ICMP

Used for ping testing and connectivity verification.

### TCP

Observed TCP connection establishment through the three-way handshake:

1. SYN
2. SYN-ACK
3. ACK

### DNS

Observed DNS queries and responses between clients and servers.
