## Moodle Resources

### Week 4
1. Which of the following are two common methods of deploying AAA? <br>
a. Flash-based<br>
b. Local<br>
c. Server-based<br>
d. PC-based<br>

Answer:
2. The simplest way to store AAA data is to use an ACS server. True or False?<br>
a. True<br>
b. False<br>

Answer:
3. Server-based AAA does not support accounting. True or False?
a. True
b. False
Answer:
4. Which authentication protocol is Cisco proprietary?
a. TACAS+
b. RADIUS
c. LDAP
d. AD
Answer:
Day 26 Page 8 of 9 Ian Patterson (2021 – S02)
5 Which function of AAA is responsible for permitting a user’s access to the network?
a. Authentication
b. Authorisation
c. Accounting
d. Access
Answer:
6 Which function of AAA is responsible for controlling what users can and cannot do 
on the network?
a. Authentication
b. Authorisation
c. Accounting
d. Access
Answer:
7 Which function of AAA is responsible for auditing and reporting?
a. Authentication
b. Authorisation
c. Accounting
d. Access
Answer:
8 Where is AAA authentication data most commonly stored in large networks?
a. Local database.
b. ACS server
c. LDAP or AD server
d. Flash memory
Answer:
Day 26 Page 9 of 9 Ian Patterson (2021 – S02)
9 Which two types of Cisco AAA server can consult user repositories such as Active 
Directory for user authentication?
a. ACS
b. ISE
c. NAS
d. RSA
e. Kerberos
Answer:
10 Which AAA protocol does ISE use to negotiate a user’s network access?
a. TACACS+
b. TACACS
c. RADIUS
d. LDAP
Answer
1 What command must first be enabled before configuring AAA on a Cisco router.
a. aaa new-model
b. username
c. privilege
d. enable secret
Answer:
2 Which command allows the TACACS+ server to economise on the number of TCP 
connections it must establish with the NAS?
a. single-connection
b. server address ipv4 10.1.1.1 single-connection
c. tacacs single-connection
d. aaa tacacs server single connection
Answer:
Day 25 Page 10 of 12 Ian Patterson (2021 – S02)
3 What two parameters must match between the ACS server and the NAS for 
TACACS+ or RADIUS session to be established.
a. Shared secret key
b. Port numbers
c. Server names
d. Username
e. Privilege level
Answer:
4 Which of the following should be used to specify that a username configured locally 
on the router must be used to authenticate?
a. aaa authentication login default local
b. aaa authentication login default group tacacs+
c. aaa authentication login default group radius
d. aaa authentication login default enable
Answer:
5 Which of the following should be used to enable a custom method list on the vty 
lines?
a. login authentication MYAUTH
b. aaa authentication login MYAUTH
c. aaa new-model
d. aaa authorization exec MYAUTH
Answer:
6 Why would a custom authentication method list include the “enable” option at the 
end?
a. To provide fault tolerance in the event multiple servers are added.
b. To enable RADIUS as a backup default method.
c. To enable the method list.
d. To avoid locking the administrators out of the router.
Answer:
Day 25 Page 11 of 12 Ian Patterson (2021 – S02)
7 According to the following command, what would need to occur for the user’s 
credentials to be verified against the RADIUS server?
aaa authentication login default group tacacs+ group radius local none
a. The TACACS+ server returns a FAIL result.
b. The TACACS+ server returns a PASS result.
c. The local database is missing.
d. The TACACS+ server is unreachable.
Answer:
8 Which of the following can be used to authenticate switch users? 
(Choose two).
a. RADIUS server
b. TACACS+ server
c. SNMP server
d. SYSLOG server
e. TFTP server
f. NTP server
Answer:
9 Which are the possible methods that a Cisco router can use to send accounting 
information? (Choose two).
a. Syslog servers
b. TFTP servers
c. SNMP server
d. RADIUS server
e. TACACS+ server
Answer:
Day 25 Page 12 of 12 Ian Patterson (2021 – S02)
10 Which debug command would track the commands that are attempted at the EXEC 
shell?
a. debug aaa authentication
b. debug aaa authorization
c. debug aaa accounting
d. debug aaa tracking
Answer:
1 Which 802.1X component is responsible for the actual authentication of the client 
device?
a. RADIUS server
b. Router
c. Switch
d. Firewall
Answer:
2 Which 802.1X component is responsible for controlling the physical access to the 
network?
a. RADIUS server
b. Router
c. Authenticator
d. Firewall
e. 
Answer:
3 802.1X can be configured on all switch interfaces, including Layer 3 interfaces and 
trunks. True or false?
a. True
b. False
Answer:
4 When configuring a Cisco switch for 802.1X, at which level of the configuration do 
the 802.1X-related commands exist?
a. Global configuration only
b. Interface configuration only
c. Line configuration only
d. Both global and interface configuration
Answer:
Day 24 Page 8 of 9 Ian Patterson (2021 – S02)
5 IEEE 802.1X may use TACACS+ to communicate the EAP identity to the 
authentication server. True or false?
a. True
b. False
Answer:
6 What are the three main components of IEEE 802.1X?
a. Agent, broker, authentication server.
b. Supplicant, authoriser, authorisation server.
c. Authentication server, supplicant, authenticator.
d. EAP, RADIUS, TLS.
Answer:
7 Which two devices can initiate 802.1X authentication?
a. Supplicant
b. Authenticator
c. Authentication server
d. Firewall
Answer:
8 Which command enables 802.1X on an interface?
a. authentication port-control auto
b. authentication port-control force-authorized
c. authentication port-control force-unauthorized
d. aaa authentication dot1x
Answer:
Day 24 Page 9 of 9 Ian Patterson (2021 – S02)
9 Prior to client authentication, which protocols are allowed to pass through a switch 
port? (Choose three).
a. CDP
b. EAPOL
c. STP
d. SNMP
e. RADIUS
f. TACACS+
Answer:
10 Which protocol is used for authentication in 802.1X?
a. RADIUS
b. TACACS+
c. MD5
d. SHA-1
e. DH
Answer:


## Week 5
1 Which three of the following are zones typically associated with firewalls?
a. Inside
b. Outside
c. Server farm
d. DMZ
Answer:
2 Which of the following is not a basic requirement of a firewall?
a. A firewall must be resistant to attacks.
b. A firewall must be the only transit point between network zones.
c. A firewall must enforce the access control policy of the organisation.
d. A firewall must be manageable from the Internet.
Answer:
3 Which of the following is not a benefit of a firewall?
a. Prevents exposure of sensitive hosts
b. Establish BGP peering sessions
c. Block malicious data
d. Control user access with AAA
Answer:
Day 11 Page 11 of 12 Ian Patterson (2019 – S02)
4 Which of the following does a packet-filtering firewall use to match packets?
a. NAT
b. ACL
c. SSH
d. Route map
Answer:
5 At which layer of the OSI model do packet-filtering firewalls not normally operate?
a. 2
b. 3
c. 4
d. 7
Answer:
6 A proxy server allows clients direct access to Internet servers. True or false?
a. True
b. False
Answer:
7 Which table do stateful firewalls use to track TCP sessions between clients and 
Internet servers?
a. State table
b. MAC address table
c. Routing table
d. ARP table
Answer:
Day 11 Page 12 of 12 Ian Patterson (2019 – S02)
8 Which of the following features is not included in a next-generation firewall?
a. Stateful inspection
b. IPS
c. Malware detection
d. Support for serial interfaces
Answer:
9 Which of the following types of firewalls is normally deployed on an endpoint?
a. Proxy server
b. Personal
c. Stateful
d. Packet filtering
Answer:
10 Using the established keyword with an ACL allows the firewall to track which TCP 
flags? (Choose two).
a. SYN
b. ACK
c. FIN
d. RST
Answer:
1 Which of the following statements are true about Zone-Based Policy Firewall?
Choose two.
a. It applies firewall policies to traffic that traverses zones.
b. Interzone polices enable you to apply different inspection policies to multiple host 
groups that are connected to the same router interface.
c. The router security posture is not restrictive.
d. Interface ACLs are applied before a zone-based policy firewall when they are 
applied outbound.
Answer:
2 If interface number 1 is in zone A, and interface number 2 is in zone B, and there is no 
policy command applied yet to the configuration, what is the status of the transit 
traffic that is being routed between these two interfaces?
a. Denied
b. Permitted
c. Inspected
d. Logged
Answer:
3 Which of the following actions cannot be applied between two zones?
a. Deny
b. Drop
c. Pass
d. Inspect
Answer:
4 What is the default policy between an administratively created zone and the self zone?
a. Deny
b. Permit
c. Inspect
d. Log
Answer:
Day 9 Page 14 of 15 Ian Patterson (2021 – S02)
5 What is required to permit traffic between zone-member interfaces?
a. Stateful Inspection
b. Policy
c. PAT
d. CBAC
Answer:
6 Which policy map action is used to permit protocols that the zone-based firewall 
supports for inspection between zones?
a. Log
b. Pass
c. Drop
d. Inspect
Answer:
7 Which zone is implied by default and does not need to be manually created?
a. Inside
b. Outside
c. DMZ
d. Self
Answer:
8 What is the default action when a source interface is a member of a zone, but the 
destination interface is not a member of a zone?
a. Deny
b. Drop
c. Policy actions
d. Pass
Answer:
Day 9 Page 15 of 15 Ian Patterson (2021 – S02)
9 If the class map “match-any” is specified, traffic must match all of the class-map 
criteria in order to belong to that particular class. True or false?
a. True
b. False
Answer:
10 Which component of C3PL is used to determine the ZPF action taken on a certain 
class of traffic?
a. Class map
b. Service policy
c. Policy map
d. Route map
Answer:


## Week 7
1 Which resulting security control act is considered a consequence of non-malicious 
activity?
a. True positive
b. True negative
c. False positive
d. False negative
Answer:
2 In which ability does the primary difference between IDS and IPS lie?
a. Ability to perform anomaly detection and rule-based detection.
b. Ability to produce alerts when suspicious traffic is seen.
c. Ability to detect intrusions that utilise encrypted communications.
d. Ability to take action upon what is detected.
Answer:
3 In general, where is the best place to position a sensor in the network?
a. Behind the firewall
b. Near the assets you need to protect
c. Before the firewall
d. In the DMZ
Answer:
Day 06 Page 11 of 12 Ian Patterson (2021 – S02)
4 Which two modes of IPS operation are currently available with Cisco IDS and IPS 
solutions?
a. Promiscuous
b. Broadcast
c. Inline
d. In band
Answer:
5 IPS solutions are typically related to inline deployment of sensors. True or false?
a. True
b. False
Answer:
6 Which two detection strategies are used in modern IPS systems today?
a. Anomaly detection
b. ACL matching
c. Protocol checking
d. Rule-based detection
Answer:
7 Which type of IPS deployment is used for protecting critical hosts in an enterprise?
a. Network-based IPS
b. Management-based IPS
c. Host-based IPS
d. Router-based IPS
Answer:
Day 06 Page 12 of 12 Ian Patterson (2021 – S02)
8 Which Catalyst switch technology can be used when deploying an IPS in promiscuous 
mode?
a. HSRP
b. RSTP
c. VTP
d. SPAN
Answer:
9 Which two of the following are failure settings for the FirePOWER module in an 
ASA?
a. Fail-open
b. Fail-closed
c. Fail-active
d. Fail-passive
Answer:
10 Which of the following is an advantage of a host-based IPS?
a. Monitors all network traffic
b. Protects the network against malicious traffic
c. Can access encrypted data on a client device
d. Easy remote management
Answer:

Which of the following is not a detection technology commonly used in IDS/IPS 
sensors?
a. Location-based
b. Signature-based
c. Policy-based
d. Anomaly-based
e. Reputation-based
Answer:
2 Which of the following is a type of signature that examines individual packets for 
malicious activity?
a. Service
b. Pattern
c. String
d. Atomic
Answer:
3 Which of the following is a type of signature that uses regular expressions to detect 
malicious activity?
a. Atomic
b. String
c. Service
d. Pattern
Answer:
4 Which two of the following are considered passive trigger actions?
a. Alerts
b. Drop
c. Block
d. Monitor
Answer:
Day 05 Page 8 of 9 Ian Patterson (2021 – S02)
5 Which of the following is not considered an active trigger action?
(The “Reset” option is missing).
a. Drop
b. Block
c. Filter
d. Shun
Answer:
6 Which new IPS technology allows the administrator to build a list of IP addresses that 
might pose a danger to corporate users?
a. Whitelisting
b. Blacklisting
c. Filtering
d. Snorting
Answer:
7 What is an IPS signature?
a. It is the timestamp that is applied to logged security events and alarms.
b. It is the authorisation that is required to implement a security policy.
c. It is a set of rules used to detect typical intrusive activity.
d. It is a security script that is used to detect unknown threats.
Answer:
8 Anomaly-based IPS signatures typically look for predefined abnormal traffic. 
True or False?
a. True
b. False
Answer:
Day 05 Page 9 of 9 Ian Patterson (2021 – S02)
9 Which active trigger action can be used for stopping malicious UDP and ICMP 
traffic?
a. Reset
b. Restart
c. Block
d. Shun
Answer:
10 Which Cisco technology can be used to monitor FirePOWER and legacy IPS sensors?
a. FireSIGHT
b. FireAMP
c. Snort
d. NGIPSv
Answer:

### Resources
fklklbdfdklsb
### Questions
1. question one
2. question two
