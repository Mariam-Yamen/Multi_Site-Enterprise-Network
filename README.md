#Multi-Site Enterprise Network - Cisco Packet Tracer

A self-directed project showing a company with 4 branch offices (Cairo, London, Madrid, Paris) connected in a
 ring topology with a central server site managing DNS, HTTP and Syslog servers.

##ACHIEVES THE THREE OF THE FOUR PILLARS
**Fault Tolerance**
 - The network can withstand failures without a total service disruption
 - Multiple OSPF Paths, Ring Topology
**Scalibility**
 - The network can grow (more users, more sites, more traffic) without needing a complete redesign
 - VLSM addressing, VLANS
**Security**
  -Protecting the network and its data from unauthorized access or attack
  - ACLS, SSH, Password Encryption

 ##Features
 **Routing**
   OSPF routing across all sites and static/default route edge for internet bound traffic.
 **VLAN**
   -each branch is segmented into 4 branches (HR, Sales, IT, Accountant) via router on stick (801.2Q 
   subinterfaces) 
   -HR- VLAN 10 | Sales= VLAN 20 | IT=VLAN 30  |Accountant = VLAN 40
 **DHCP** 
   -DHCP pool for each department per router.
 **Addressing**
   -Custom Vlan plan
   -subnets : /29 per department | /28 : shared services | /30 WAN Links
   - Static Addressing for servers (HTTP, DNS, syslog) and for router interfaces
 **SECURITY**
   - Extended ACL Enforcement in each department , where IT has full access, sales and accountant can reach
     each other, but HR is isolated.
   - SSH-only remote management
   - Encrypted Passwords on all devices
 **NAT/PAT**
  - Configured on edge router for outbound internet traffic
 **Services**
  - Centralized DNS, Internet web server, and syslog logging from all routers
 **Fault Tolerant**
