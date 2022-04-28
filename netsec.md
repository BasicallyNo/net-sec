[Markdown-Cheatsheet](https://www.markdownguide.org/cheat-sheet/)

# [Index]
# Module 1 - 4: Securing Networks
## 1. Network Topologies
#### Campus Area Networks
The main focus of this course is on securing Campus Area Networks (CANs). Campus Area Networks consists of interconnected LANs within a limited geographic area. Connections to untrusted networks must be checked in-depth by multiple layers of defense before reaching enterprise resources. This is known as defense-in-depth.

Useful technologies for providing Campus Area Network (CAN) defence:
- VPN
Virtual Private Networks are seperate from the internet and are a means of providing data confidentiality and integrity from authenticated sources.
#### Small Office & Home Office Networks
#### Wide Area Networks
#### Data Center Networks
#### Cloud Networks and Virtualization
#### The evolving Network Border

## 2. Network Threats
#### What are Network Threats?
#### Who is attacking networks?
#### Threat Actor Tools
#### Malware
#### Common Network Attacks
#### Denial of Service, Buffer Overflows, and Evasion
#### Summary

## 3. Mitigating Threats
#### Introduction
#### Defending a Network
#### Network Security Policies
#### Security Tools, Platforms, and Services
#### Mitigating Common Network Attacks
#### Cisco Foundation Protection Framework
#### Mitigating Threats Summary

## 4. Secure Device Access
#### Introduction
#### Secure the Edge Router
#### Configure Secure Administrative Access
#### Configure Enhanced Security for Virtual Logins
#### Configure SSH
#### Summary

# Module 5 - 7: Monitoring and Managing Devices
---
## 5. Assigning Admin Roles
#### Introduction
You will learn how to configure administrative privilege levels and role-based CLI.
The focus will be to:
- Configure privilege levels by using commands to configure admin privileges to control command availability.
- Configure a Role Based CLI to control command availability.
#### Configure Privilege Levels
We should limit command availability because not all job functions should have the same level of access to the infrastructure devices.
Cisco ISO software has two ways of limiting access.
1. Privilege level
2. Role based CLI (command line interface)
Both methods help determine who should be allowed to connect to the device and what that person should be able to do with it. Role-based CLI access provides more granularity and control.

By default, the Cisco IOS software CLI has two levels of access to commands:
- User EXEC mode        (Privilege lvl 1)  This allows only user-level commands.
- Privileged EXEC mode  (Privilege lvl 15) This includes all enable-level commands.

There are 16 privilege levels in total! The higher the level, the higher the access.
<u>Here is a basic guide for privilege levels:</u>
- ___Level 0___: Predefined for user-level access privileges. Seldom used, but includes five commands: disable, enable, exit, help, and logout.
- ___Level 1___: The default level for login with the router prompt Router >. A user cannot make any changes or view the running configuration file.
- ___Level 2 - 14___: May be customized for user-level privileges. Commands from lower levels may be moved up to another higher level, or commands from higher levels may be moved down to a lower level.
- ___Level 15___: Reserved for the enable mode privileges (enable command). Users can change configurations and view configuration files.
<br>
![cisco privilege global configuration mode](src/cisco_custom_privs.png)
---
<u>Configuring & Assigning Privilege Levels</u>
To configure a privilege level with specific commands, use the ___privilege exec level___ command. This example shows examples for three different privilege levels.
- Privilege level 5 has access to all the commands available for the predefined level 1 and the ping command.
- Privilege level 10 has access to all the commands available for level 5 as well as the reload command.
- Privilege level 15 is predefined and does not need to be explicitly configured. This privilege level has access to all commands including viewing and changing the configuration.
![configure privilege levels cisco](src/configure_privilege_levels_cisco.png)

There are two methods for assigning passwords to the different privilege levels:
- To a user that is granted a specific privilege level, use the username name privilege level secret password global configuration mode command.
- To the privilege level, use the enable secret level level password global configuration mode command.

___Note___: Both the username secret and the enable secret commands are configured for type 9 encryption.

To assign privileges to a specific user, use the _username_ command. Use the enable secret command to assign a privilege level to a specific EXEC mode password. For example, the SUPPORT user is assigned privilege level 5 with the password cisco5. However, as shown in the example below, any user can access privilege level 5 if that user knows that the enable secret password is cisco5.

  R1> enable 5
_Password:_ <cisco5>
  R1# show privilege
_Current privilege level is 5_

<u>Limitations of Privilege Levels</u>
- There is no access control to specific interfaces, ports, logical interfaces, and slots on a router.
- Commands available at lower privilege levels are always executable at higher levels.
- Commands specifically set at a higher privilege level are not available for lower privileged users.
- Assigning a command with multiple keywords allows access to all commands that use those keywords. For example, allowing access to show ip route allows the user access to all show and show ip commands.

___Note___: If an administrator must create a user account that has access to most but not all commands, privilege exec statements need to be configured for every command that must be executed at a privilege level lower than 15.

Do a practical router config here: [NetAcad Practical](https://contenthub.netacad.com/netsec/5.1.4)

<u>Role-Based CLI Access</u>



## 6. Device Monitoring and Management
#### Introduction
#### Secure Cisco ISO Image and Configuration Files
#### Lock Down a Router using AutoSecure
#### Routing Protocol Authentication
#### Secure Management and Reporting
#### Network Security using Syslog
#### NTP Configuration
#### SNMP Configuration
#### Summary

## 7. Authenticaion, Authorization, and Accounting
#### Introduction
#### AAA Characteristics and Protocols
#### Configure Server Based Authentication
#### Configure Server Based Authorization and Accounting
#### Summary

# Modules 8 - 10: ACLs and Firewalls
## 8. Access Control Lists
## 9. Firewall
## 10. Zone Based Policy Firewalls

# Modules 11 - 12: Intrusion Prevention
## 11. IPS Technologies
## 12. IPS Operation and Implementation

# Modules 13 - 14: Layer 2 and Endpoint Security
## 13. Endpoint Security
## 14. Layer 2 Security Considerations

# Modules 15 - 17: Cryptography
## 15. Cryptographic Services
## 16. Basic Integrity and Authenticity
## 17. Public Key Cryptography

# Modules 18 - 19: VPNs


# Modules 20 - 22: ASA

