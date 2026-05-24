# Packet Tracer VLSM Routing Project

This is a Cisco Packet Tracer based computer networking project developed for CSE421. The project designs and implements a structured network topology using VLSM, DHCP, static routing, floating static routes, dynamic routing with RIP v2, DNS, web, and email services.

## Project Overview

The network connects multiple zones, including:

- Malcolm's School Lab
- Francis's Military Academy Network
- Hal's Workplace Office
- Reese's Kitchen Control Zone
- Dewey's Creative Experiment Lab
- Family Home Network

The project uses a base network address derived from the student ID and applies VLSM subnetting to reduce IP address waste.

## Key Features

- VLSM subnetting
- Static IP addressing for the Family Home network
- Router-based DHCP for selected networks
- Server-based DHCP for selected networks
- DNS server configuration
- Web server configuration
- Email server communication
- RIP v2 dynamic routing
- Standard static routes
- Default static route
- Floating static route with administrative distance
- Full network connectivity verification using ping

## Technologies Used

- Cisco Packet Tracer
- IPv4 Addressing
- VLSM
- DHCP
- DNS
- Web Server
- Email Server
- RIP v2
- Static Routing

## Network Design Summary

The project uses the base network address `24.24.0.0`. VLSM was applied to allocate subnets based on host requirements for different network zones.

Major LAN subnets include:

| Network Zone | Required Hosts | Subnet |
|---|---:|---|
| Malcolm's School Lab | 840 | /22 |
| Francis's Military Academy | 390 | /23 |
| Dewey's Creative Experiment Lab | 300 | /23 |
| Reese's Kitchen Control Zone | 210 | /24 |
| Hal's Workplace Office | 72 | /25 |
| Family Home Network | 25 | /27 |

## Routing Summary

- RIP v2 was used for dynamic routing between Malcolm, Reese, and Hal networks.
- Static routes were configured for selected network paths.
- A default static route was configured on the Family Home router.
- A floating static route was configured between Family Home and Dewey's Lab.
- Malcolm's router was used as a hybrid router with both static and dynamic routing.

## Files Included

- `Project.pkt` - Cisco Packet Tracer project file
- `docs/project-report.pdf` - Project report
- `screenshots/network-topology.png` - Network topology screenshot
- `configs/router-configurations.txt` - Router configuration commands

## How to Open

1. Install Cisco Packet Tracer.
2. Download or clone this repository.
3. Open `Project.pkt` using Cisco Packet Tracer.
4. Check router configurations, IP addressing, DHCP, DNS, web, email, and routing setup.

## Contributors

This project was developed as a group project by:

- Md. Fakhrul Abedin Shohrub
- Afifa Ahmed(https://github.com/afifa-ahmed-ammun)
- Chowdhury Zawad Al Munawar()

## Academic Context

Course: CSE421  
Project Topic: End of Experiment  
Tool: Cisco Packet Tracer
