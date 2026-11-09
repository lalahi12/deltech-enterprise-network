# DelTech Enterprise Network Infrastructure

A network infrastructure project built using Cisco Packet Tracer.

## About This Project

In this project, I designed and configured a small enterprise network for a company with three departments: IT, HR, and Finance.

Each department uses a separate VLAN so that the network is easier to manage. I also connected all departments to a central server for internal network services.

I worked on the network configuration step by step, starting from connecting the devices and setting up VLANs to testing communication between different networks.

## What I Worked On

Here are the main configurations I completed in this project:

- Created VLANs for IT, HR, Finance, and Server.
- Configured trunk connections between switches and the router.
- Set up inter-VLAN routing using Router-on-a-Stick.
- Configured DHCP to assign IP addresses automatically.
- Set up DNS for the internal domain.
- Configured an internal web server.
- Added ACL rules to restrict access from Finance to IT.
- Enabled SSH for remote router management.

## Network Design

The network uses one Cisco 2911 router, two Cisco 2960 switches, one server, and six client PCs.

| VLAN | Department | Network | Gateway |
|---|---|---|---|
| 10 | IT | 192.168.10.0/24 | 192.168.10.1 |
| 20 | HR | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Server | 192.168.40.0/24 | 192.168.40.1 |

## Server Information

The server is connected to VLAN 40 and provides internal network services.

| Configuration | Value |
|---|---|
| Server IP Address | 192.168.40.10 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 192.168.40.1 |
| DNS Domain | intranet.deltech.local |
| Web Service | HTTP |

## Network Security

I configured an Extended ACL on the router to prevent devices in the Finance VLAN from initiating communication with the IT VLAN.

Other permitted network traffic is still allowed. This configuration was tested using ping between PCs in different VLANs.

SSH was also enabled so the router can be accessed remotely from a PC without using Telnet.

## Testing

After configuring the network, I performed several tests to check whether everything was working properly.

The tests included:

- Checking connectivity between PCs and their gateways.
- Testing communication between different VLANs.
- Checking DHCP address assignment.
- Accessing the server using its IP address.
- Opening the internal website using `intranet.deltech.local`.
- Testing the ACL rules between Finance and IT.
- Connecting to the router using SSH.

The tests helped me identify and fix some configuration issues during the project.

## Tools and Devices

- Cisco Packet Tracer
- Cisco 2911 Router
- Cisco 2960 Switch
- Server
- End Devices (PCs)

## What I Learned

Through this project, I gained practical experience in configuring VLANs, routing, DHCP, DNS, and network security.

I also learned how to troubleshoot network connectivity problems and verify configurations using Cisco IOS commands.

## Project File

The Packet Tracer file and supporting screenshots are included in this repository.

## Network Topology

The following diagram shows the network layout built in Cisco Packet Tracer.

![Network Topology](Topologi%20Jaringan.png)

## Project Testing

The following screenshots show the results of the network configuration and testing:

### DNS Testing
![DNS Testing](Pengujian%20DNS.png)

### Web Server Testing
![Web Server Testing](Pengujian%20Web%20Server.png)

### ACL Testing
![ACL Testing](Pengujian%20ACL.png)
![ACL Testing](Pengujuan%20ACL.png)

### SSH Testing
![SSH Testing](Pengujian%20SSH.png)

## Author

**Sri Indah Permata Silalahi**

Institut Teknologi Del  
Network Infrastructure Project
