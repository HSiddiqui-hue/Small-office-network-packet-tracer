Small Office Network Project (Cisco Packet Tracer)
This home lab project simulates a real small office network using Cisco Packet Tracer.
The network includes a router, switch, server, wireless router, and multiple wired/wireless clients.

Technologies Used

Cisco Packet Tracer
- Cisco Router (IOS CLI)
- Switch (Layer 2)
- DHCP
- DNS
- FTP
- HTTP Server
- Wireless Networking
- TCP/IP

Network Topology
Below is the full topology for the small office network designed and configured in Cisco Packet Tracer:

<p align="center">
  <img src="https://github.com/user-attachments/assets/9088cbe8-0325-4741-8da4-f89ba6deb317" width="80%">
</p>

Network Configuration
- Router (Gateway)
- GigabitEthernet0/0 → 192.168.10.1
- DHCP enabled
- DNS provided by internal server
- LAN connects to switch

Server
- IP: 192.168.10.20
- Services: DNS, HTTP, FTP (internal website)

Clients
- PCs using DHCP
- Wireless client connected to WPA2-secured SSID

Services Configured
- DHCP
- Router assigns IP addresses: 192.168.10.100 – 192.168.10.150

DNS
DNS Records:
- office → 192.168.10.20
- server → 192.168.10.20
- router → 192.168.10.1

HTTP
- Simple intranet page hosted on server.

Testing Performed
Test	Result
- Ping Router	✔ Successful
- Ping Server	✔ Successful
- HTTP Webpage from Server	✔ Loaded
- DNS: ping office	✔ Resolved
- DHCP Assigned Address	✔ Yes
- PC to PC Connectivity	✔ Yes
- Wireless Client Connectivity	✔ Yes

Troubleshooting Performed
- DHCP failure due to incorrect network config (fixed 192.169 → 192.168)
- Interface down issues (no shutdown)
- DNS resolution errors (fixed by updating DNS server in DHCP)

Files in This Repo
- topology.png — Network diagram
- screenshots/ — Test results
- README.md — Project documentation

Skills Demonstrated
- Routing & Switching
- IP Addressing
- DHCP & DNS
- Wireless configuration
- Troubleshooting
- IT Support fundamentals
- Cisco IOS CLI commands
- Network design
