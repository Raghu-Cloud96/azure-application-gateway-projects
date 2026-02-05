# Project 2: Secure Single Web Application using Azure Application Gateway

## Overview
This project focuses on a clean and minimal Azure setup to expose a private Linux web server securely using Azure Application Gateway.

## Architecture
- Virtual Network with two subnets:
  - Web Subnet
  - Application Gateway Subnet
- One private Linux VM running nginx
- Azure Application Gateway (WAF v2) as the public entry point

## Key Features
- Web VM has no public IP
- Only Application Gateway is internet-facing
- Subnet-level NSG restricts access to Web VM
- Health probes ensure backend availability

## Responsibilities Performed
- Created Azure VNet and subnets with proper IP planning
- Configured NSG to allow traffic only from Application Gateway
- Deployed Linux VM and installed nginx
- Configured Application Gateway with backend pool and routing rules
- Validated backend health and application accessibility

## Lessons Learned
- Importance of dedicated subnet for Application Gateway
- Difference between HTTP and HTTPS listeners
- How backend health probes work
- How NSGs affect Application Gateway connectivity

## Outcome
Successfully exposed a private web application securely using Azure Application Gateway with clean and repeatable architecture.

