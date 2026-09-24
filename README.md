# Zero Trust Access Control Lab
A practical cybersecurity lab that demonstrates Zero Trust access control in an isolated virtual environment using Ubuntu, Kali Linux, VirtualBox, networking, authentication, authorization, and security logging.

## Project Objective
The objective is to build a working access-control environment where network connectivity alone does not automatically grant access to protected resources.
The project will progressively implement:
- Network segmentation
- Authentication
- Identity-based access
- Role-Based Access Control (RBAC)
- Least-privilege access
- Application-level authorization
- Security logging
- Access auditing
- Security testing

## Lab Architecture
```text
                         Windows 11 Host
                               |
                            VirtualBox
                               |
                +--------------+--------------+
                |                             |
             Ubuntu                         Kali
          Security Server              Security Client
         192.168.56.101               192.168.56.102
                |                             |
                +--------- Host-only ---------+
                       192.168.56.0/24
```

## Lab Components
- **Component** - Role
- **Windows 11** -	Physical host
- **VirtualBox**	- Virtualization platform
- **Ubuntu	Server** - protected resources
- **Kali Linux** -	Client and security testing
- **Host-only Network** - Isolated lab communication

## Current Network
- **Machine** - Private IP
- **Ubuntu**	- '192.168.56.101'
- **Kali Linux** -	'192.168.56.102'

## Progress
- [x] Create Ubuntu virtual machine
- [x] Create Kali Linux virtual machine
- [x] Configure VirtualBox host-only network
- [x] Connect Ubuntu to private network
- [x] Connect Kali to private network
- [x] Verify Kali → Ubuntu connectivity
- [x] Verify Ubuntu → Kali connectivity
- [ ] Deploy protected web application
- [ ] Implement authentication
- [ ] Implement RBAC
- [ ] Implement least-privilege policies
- [ ] Implement access logging
- [ ] Test authorized access
- [ ] Test unauthorized access
- [ ] Analyze security logs
- [ ] Document security decisions

## Technologies
- Ubuntu Linux
- Kali Linux
- VirtualBox
- TCP/IP networking
- Python
- HTTP
- Authentication
- Authorization
- RBAC
- Security logging

## Security Principle
- The project follows the Zero Trust principle:
- Network location alone should not be treated as proof of trust.
- Access decisions will be based on the identity, role, and requested resource rather than simply allowing access because a system is connected to the private network.

## Project Status
- Currently, the isolated lab network has been successfully established and connectivity between Kali Linux and Ubuntu has been verified.
- The next phase is to deploy a protected application on Ubuntu and begin implementing authentication and authorization.

## Disclaimer
- This project is conducted entirely within an isolated virtual laboratory for educational and defensive cybersecurity purposes.
