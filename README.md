# DelTech Enterprise Network Infrastructure

## Project Overview

This project is an enterprise network infrastructure simulation developed using Cisco Packet Tracer.

The network is designed to represent a small enterprise environment with separate departments, centralized server services, inter-VLAN routing, and network security policies.

## Project Objectives

- Design an enterprise network topology.
- Implement VLAN segmentation for different departments.
- Configure inter-VLAN routing using Router-on-a-Stick.
- Implement DHCP and DNS services.
- Provide an internal web server.
- Apply Access Control Lists (ACL) for network security.
- Enable secure remote router management using SSH.

## Network Departments
| VLAN | Department | Network | Gateway |
|---|---|---|---|
| 10 | IT | 192.168.10.0/24 | 192.168.10.1 |
| 20 | HR | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Server | 192.168.40.0/24 | 192.168.40.1 |

## Technologies Used

- Cisco Packet Tracer
- Cisco 2911 Router
- Cisco 2960 Switch
- VLAN and Trunking
- Inter-VLAN Routing
- DHCP
- DNS
- HTTP Web Server
- Access Control List (ACL)
- SSH Remote Management

## Network Security

An Extended ACL is implemented to prevent the Finance department from initiating access to the IT network, while allowing other permitted network traffic.

## Server Configuration

- Server IP: 192.168.40.10
- DNS Domain: intranet.deltech.local
- DNS Service: Enabled
- HTTP Service: Enabled

## Testing and Validation

The following network functions have been tested:

- Connectivity between PCs and their gateways.
- Inter-VLAN communication.
- DHCP address assignment.
- DNS name resolution.
- Internal web server access.
- ACL access restrictions.
- SSH remote management.

## Project Files

The Cisco Packet Tracer simulation file and supporting documentation will be provided in this repository.

## Author

**Sri Indah Permata Silalahi**

Network Infrastructure Project  
Institut Teknologi Del
