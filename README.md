# 🌐 ConnectX Company Network – OSPF-Based Enterprise Design
📘 Overview

ConnectX Company Network is a complete enterprise-level network design and implementation project built for the Networking course.

# The project simulates a multi-branch company operating across:

Amman (HQ)

Irbid

Zarqa

Aqaba

Beirut

Cairo

The network was designed with scalability, redundancy, security, and service availability in mind.

# 🏗 Network Architecture
# 🔹 Topology Design

Hybrid Ring with Partial Mesh

Ring connectivity between branch routers

Direct links from HQ to Aqaba and Beirut for performance optimization

Star topology inside each branch (switch-based LAN)

# 🔹 Subnetting Strategy

LAN subnets: /27 (30 usable IPs per branch)

WAN links: /30 (point-to-point router connections)

Loopbacks: /32 (used for OSPF Router IDs)

# 🔹 Routing Protocol

OSPF (Open Shortest Path First)

Fast convergence

Cost-based path selection

VLSM support

Automatic rerouting on failure

Loop prevention mechanisms

# 🖥 Implemented Services

The following enterprise services were deployed:

Server Role	IP Address	Purpose
DHCP	192.168.1.2	Dynamic IP assignment
DNS	192.168.1.3	Domain name resolution
Web Server (HTTPS)	192.168.1.4	Internal secure company portal
Email Server	192.168.1.5	Internal communication
FTP Server	192.168.1.6	File sharing between branches
# 🔐 Security Configuration

Basic router-level security was implemented:

enable secret for privileged access

Console and remote login protection

OSPF Router IDs configured using loopback interfaces

Configuration backups

# 🧪 Testing & Validation

The network was tested using:

✅ Inter-branch connectivity (Ping tests)

✅ DHCP auto-configuration

✅ DNS resolution

✅ HTTPS website access

✅ Email sending & receiving

✅ FTP file transfer

✅ OSPF neighbor verification

Issues encountered (DHCP relay, DNS misconfiguration, OSPF neighbor loss) were identified and resolved through structured troubleshooting.
