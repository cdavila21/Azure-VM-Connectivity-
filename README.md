# Azure-VM-Connectivity
Network Security Groups (NSGs) and Traffic Inspection Between Azure Virtual Machines
In this lab, we explore how Network Security Groups (NSGs) function in Microsoft Azure by inspecting network traffic between Azure Virtual Machines (VMs) using Wireshark. This hands-on approach provides a deeper understanding of network security and communication protocols within Azure environments.

Technologies and Tools Used
Cloud Platform: Microsoft Azure (Compute/Virtual Machines)

Remote Access: Remote Desktop Protocol (RDP)

Utilities and Tools:

Command-line tools (CMD, PowerShell, SSH)

Wireshark (for network protocol analysis)

Protocols Analyzed:

ICMP (Ping)

SSH (Port 22)

DHCP (Ports 67/68)

DNS (Port 53)

RDP (Port 3389)

Operating Systems Involved
Windows 10 (Version 21H2)

Ubuntu Server 20.04

Overview of Lab Steps
Create a Resource Group

Use the Azure Portal or CLI to set up a resource group for organizing related resources.

Deploy Two Virtual Machines

One VM running Windows 10 and another running Ubuntu Server 20.04.

Place both VMs in the same Virtual Network (VNet) and subnet to simplify traffic inspection.

Inspect and Analyze Traffic

Use Wireshark and command-line tools to capture and analyze traffic for:

ICMP (ping between VMs)

SSH (remote shell sessions)

DHCP (IP address assignment)

DNS (domain resolution)

RDP (remote desktop sessions)

