# Cisco-Networking-Lab
Hands-on Cisco Packet Tracer networking and troubleshooting projects
# Cyber Lab 01 — Small Office LAN Deployment

## Project Overview

Designed, configured, and tested a small office Local Area Network (LAN) using Cisco Packet Tracer.

The project demonstrates foundational networking concepts including IPv4 addressing, Ethernet switching, network connectivity testing, and MAC address learning.

## Tools and Technologies

- Cisco Packet Tracer
- Cisco Catalyst 2960 Switch (simulated)
- IPv4 / TCP-IP
- Ethernet
- Cisco IOS Command Line Interface (CLI)
- ICMP and ARP

## Network Topology

The network consists of three computers connected to one Cisco 2960 switch.

| Device | IPv4 Address | Subnet Mask | Switch Port |
|---|---|---|---|
| PC0 | 192.168.1.10 | 255.255.255.0 | Fa0/1 |
| PC1 | 192.168.1.11 | 255.255.255.0 | Fa0/2 |
| PC2 | 192.168.1.12 | 255.255.255.0 | Fa0/3 |

All workstations belong to the 192.168.1.0/24 network.

## Configuration

1. Connected three workstations to a Cisco 2960 switch using copper straight-through Ethernet cables.
2. Assigned unique static IPv4 addresses to each workstation.
3. Configured all workstations with the same /24 subnet mask.
4. Verified connectivity using ICMP ping tests.
5. Used the Cisco IOS CLI to inspect dynamically learned MAC addresses.

## Testing and Verification

The following connectivity tests were completed successfully:

- PC0 to PC1 — Passed
- PC0 to PC2 — Passed
- PC1 to PC2 — Passed

Each test demonstrated successful local network communication.

## MAC Address Table Analysis

Executed the Cisco IOS command:

`show mac address-table`

Verified three dynamically learned MAC addresses associated with switch ports Fa0/1, Fa0/2, and Fa0/3.

Observed an initially empty MAC address table and confirmed that entries appeared following additional network traffic, demonstrating dynamic MAC learning.

## Skills Demonstrated

- LAN design and implementation
- Static IPv4 configuration
- Ethernet connectivity
- Cisco switching fundamentals
- ICMP connectivity verification
- MAC address table inspection
- Foundational network troubleshooting

## Project Files

The repository includes the Cisco Packet Tracer project file. Additional screenshots and analysis may be added as the lab progresses.

## Project Status

Core LAN configuration and connectivity testing completed. ARP and Ethernet frame analysis in Packet Tracer Simulation Mode are planned as the next phase.

## Lab Evidence

### Network Topology
![Network Topology](screenshots/Network%20Topology.png)

### PC0 Connectivity
![PC0 Ping Test](screenshots/PCO-Ping%20Test.png)

### PC1 Connectivity
![PC1 Ping Test](screenshots/PC1-Ping%20Test.png)

### PC2 Connectivity
![PC2 Ping Test](screenshots/PC2-Ping%20Test.png)

### MAC Address Table
![Switch MAC Table](screenshots/Mac%20address%20table.png)
