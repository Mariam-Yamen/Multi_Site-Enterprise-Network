## Router Interface IP Addressing

| Router | Interface | IP Address | Subnet Mask | Description |
|---|---|---|---|---|
| **Cairo** | Gig0/0/0.10 | 192.168.10.1 | /29 | HR VLAN |
| Cairo | Gig0/0/0.20 | 192.168.20.1 | /29 | Sales VLAN |
| Cairo | Gig0/0/0.30 | 192.168.30.1 | /29 | IT VLAN |
| Cairo | Gig0/0/0.40 | 192.168.40.1 | /29 | Accounting VLAN |
| Cairo | Se0/2/0 | 200.0.0.1 | /30 | WAN to serverrouter |
| Cairo | Se0/2/1 | 200.0.0.18 | /30 | WAN to London |
| **London** | Gig0/0/0.10 | 192.168.50.1 | /29 | HR VLAN |
| London | Gig0/0/0.20 | 192.168.60.1 | /29 | Sales VLAN |
| London | Gig0/0/0.30 | 192.168.70.1 | /29 | IT VLAN |
| London | Gig0/0/0.40 | 192.168.80.1 | /29 | Accounting VLAN |
| London | Se0/2/0 | 200.0.0.2 | /30 | WAN to Cairo |
| London | Se0/2/1 | 200.0.0.5 | /30 | WAN to Madrid |
| **Madrid** | Gig0/0/0.10 | 192.168.90.1 | /29 | HR VLAN |
| Madrid | Gig0/0/0.20 | 192.168.100.1 | /29 | Sales VLAN |
| Madrid | Gig0/0/0.30 | 192.168.110.1 | /29 | IT VLAN |
| Madrid | Gig0/0/0.40 | 192.168.120.1 | /29 | Accounting VLAN |
| Madrid | Se0/2/0 | 200.0.0.6 | /30 | WAN to London |
| Madrid | Se0/2/1 | 200.0.0.9 | /30 | WAN to Paris |
| **Paris** | Gig0/0/0.10 | 192.168.130.1 | /29 | HR VLAN |
| Paris | Gig0/0/0.20 | 192.168.140.1 | /29 | Sales VLAN |
| Paris | Gig0/0/0.30 | 192.168.150.1 | /29 | IT VLAN |
| Paris | Gig0/0/0.40 | 192.168.160.1 | /29 | Accounting VLAN |
| Paris | Se0/2/0 | 200.0.0.10 | /30 | WAN to Madrid |
| Paris | Se0/2/1 | 200.0.0.13 | /30 | WAN to serverrouter |
| **serverrouter** | Gig0/0/0 | 192.168.0.65 | /28 | Servers VLAN |
| serverrouter | Gig0/0/1 | 203.162.0.1 | /30 | Edge (Cloud-PT) |
| serverrouter | Se0/2/0 | 200.0.0.17 | /30 | WAN to Cairo |
| serverrouter | Se0/2/1 | 200.0.0.14 | /30 | WAN to Paris |
