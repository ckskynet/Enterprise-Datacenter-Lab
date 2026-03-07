# Enterprise-Datacenter-Lab
Designed and deployed a virtual enterprise datacenter lab using OPNsense and Windows Server to simulate a small business network. Implemented segmented networks, domain services, and centralized infrastructure to practice enterprise system administration and cybersecurity concepts.

## Objectives
- Build an enterprise-style virtual lab
- Practice network segmentation and firewall administration
- Deploy Windows Server infrastructure services
- Configure domain-based management
- Improve hands-on cybersecurity and systems administration skills

## Technologies Used
- VirtualBox
- OPNsense
- Windows Server
- Windows client systems
- Linux administration client
- Active Directory Domain Services
- DNS
- DHCP
- Firewall rules / routing / NAT

## Lab Architecture
The lab was designed with OPNsense as the perimeter firewall/router between the WAN and internal networks. Internal resources were separated into trusted and isolated segments to simulate enterprise network design. Windows Server was used to provide centralized identity and core infrastructure services.

## Network Design
- WAN: Upstream network connection
- LAN: Trusted internal server / management segment
- LAB_DMZ: Isolated client/testing segment
- Domain: `corp.home.arpa`

## Implementation Summary
### Phase 1: Planning
- Defined scope, topology, and addressing strategy

### Phase 2: Firewall Deployment
- Installed and configured OPNsense
- Assigned interfaces and configured internal routing
- Created initial firewall policies

### Phase 3: Core Infrastructure
- Deployed Windows Server
- Configured Active Directory, DNS, and DHCP
- Established domain services for the lab

### Phase 4: Endpoint Deployment
- Installed client systems
- Connected endpoints to designated network segments
- Validated connectivity and service access

### Phase 5: Testing and Validation
- Tested segmentation behavior
- Verified name resolution and routing
- Confirmed access to internal services

## Challenges Encountered
- Resolved routing and gateway assignment issues during initial configuration
- Troubleshot management connectivity to OPNsense from client systems
- Refined internal segmentation strategy between LAN and LAB_DMZ
- Worked around virtualization constraints for certain Windows client images

## Security Concepts Demonstrated
- Network segmentation
- Firewall policy enforcement
- Centralized identity management
- Secure internal service deployment
- Administrative troubleshooting in an enterprise-style environment

## Results
The completed lab provides a working enterprise-style environment for practicing system administration, network engineering, and cybersecurity concepts in a controlled virtual setting.

## Lessons Learned
- Proper IP planning simplifies multi-network deployments
- DNS and routing are critical to Windows-based infrastructure
- Segmentation design directly affects usability and security
- Hands-on troubleshooting is essential in lab development

## Future Improvements
- Add SIEM/log collection
- Implement vulnerability scanning
- Deploy additional DMZ services
- Expand hardening and monitoring controls
- Add VPN-based remote access
