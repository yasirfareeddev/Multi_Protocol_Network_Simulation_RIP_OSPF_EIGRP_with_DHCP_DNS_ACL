# DCCN Final Project : DHCP + RIP/OSPF/EIGRP + Redistribution & Services

> This repository contains the simulations, device configurations, screenshots and documentation for a campus-style network lab. The lab demonstrates DHCP, routing protocols (RIP, OSPF, EIGRP), redistribution between protocols, email server configuration, ACL filtering, and wireless access point integration.

---

## Table of contents
- [Overview](#overview)  
- [Features](#features)  
- [Requirements](#requirements)  
- [Topology & Files](#topology--files)  
- [Quickstart — How to run the simulation](#quickstart---how-to-run-the-simulation)  
- [Step-by-step configuration (high-level)](#step-by-step-configuration-high-level)  
  - [Stage 1 — RIP + DHCP](#stage-1---rip--dhcp)  
  - [Stage 2 — OSPF + Redistribution to RIP](#stage-2---ospf--redistribution-to-rip)  
  - [Stage 3 — EIGRP + Redistribution to OSPF](#stage-3---eigrp--redistribution-to-ospf)  
  - [Stage 4 — Email service (SMTP/POP) setup](#stage-4---email-service-smtp-pop-setup)  
  - [Stage 5 — ACL & Wireless AP](#stage-5---acl--wireless-ap)  
- [Folder structure](#folder-structure)  
- [Credits & License](#credits--license)

---

## Overview
This project simulates a campus network with multiple LANs and a centralized DHCP server that assigns addresses across those LANs. Routing is demonstrated using RIP, OSPF, and EIGRP and redistribution is implemented on special "redistributor" routers so routes cross between the protocols. The project also includes an email server demonstration, access control lists and an access point + wireless client configuration.

**Source document:** Lab report and stepwise screenshots included in `/Project Documentation`. (See original Project document for full step details.)

---

## Features
- DHCP pools for multiple LANs (different subnets & masks)  
- RIP, OSPF and EIGRP routing domains and configuration examples  
- Route redistribution (RIP ↔ OSPF, OSPF ↔ EIGRP) on redistributor routers  
- Email server configuration and email exchange across routing domains  
- Example ACL to block a specific host from receiving traffic  
- Wireless AP setup and DHCP assignment to wireless clients  
- Screenshots, configs and Packet Tracer simulation files included

---

## Requirements
- **Cisco Packet Tracer 8.2.2**
  - Download from official source: https://www.netacad.com/courses/packet-tracer
  - You need a free Cisco Networking Academy account  
- Basic familiarity with Cisco CLI (enable, config t, interface, router <protocol>)  
- Git and GitHub account to host the repo

---

## Topology & Files
## Final Network Topology : 
![Final Topology](./Project%20Documentation/topology.png)
- Main simulation file : `Multi_Protocol_Network_Simulation_RIP_OSPF_EIGRP_with_DHCP_DNS_ACL.pkt`    
## RIP using DHCP :
![Final Topology](./Project%20Documentation/DHCP(RIP).png)
## OSPF using DHCP :
![Final Topology](./Project%20Documentation/DHCP(OSPF).png)
## EIGRP using DHCP :
![Final Topology](./Project%20Documentation/DHCP(EIGRP).png)
## Email Configuration using server in EIGRP :
![Final Topology](./Project%20Documentation/Email_Configuration_using_server_in_EIGRP.png)
## ACL Implementation :
![Final Topology](./Project%20Documentation/ACL_Implementation.png)

## Quickstart — How to run the simulation
1. Clone the repo:
   ```bash
   git clone https://github.com/yasirfareeddev/Multi_Protocol_Network_Simulation_RIP_OSPF_EIGRP_with_DHCP_DNS_ACL.git


## Authors : 
- Yasir Fareed 
- Huma Ibrar
- Umer Qazi
- Abdullah  
## Course : 
Data Communication and Computer Networks (DCCN)  
## Submitted to : 
- Sir Gulam Raza