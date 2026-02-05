# Project 1: Secure Multi-Tier Azure Architecture using Application Gateway

## Overview
This project demonstrates a secure, enterprise-style Azure architecture using multiple subnets, private virtual machines, Network Security Groups (NSGs), and Azure Application Gateway (WAF v2) as the single public entry point.

## Architecture
- Virtual Network with multiple subnets:
  - Web Subnet
  - App Subnet
  - DB Subnet
  - Application Gateway Subnet
- Linux Virtual Machines without public IPs
- Application Gateway (WAF v2) for HTTP traffic
- Subnet-level NSGs for traffic control

## Key Features
- No VM exposed directly to the internet
- Application Gateway handles all inbound traffic
- Strict NSG rules for east-west traffic
- Backend health monitoring using Application Gateway probes

## Responsibilities Performed
- Designed Azure VNet and subnet architecture
- Implemented subnet-level NSGs
- Deployed Linux VMs and installed nginx
- Configured Application Gateway frontend, backend pools, listeners, and routing rules
- Troubleshot backend health issues (NSG blocks, missing services)
- Validated secure end-to-end traffic flow

## Troubleshooting Experience
- Resolved 502 errors caused by unhealthy backend
- Identified blocked health probes due to NSG rules
- Fixed missing application service (nginx)
- Validated 200 OK backend health status

## Outcome
Successfully deployed a secure, multi-tier Azure environment in line with enterprise best practices.

