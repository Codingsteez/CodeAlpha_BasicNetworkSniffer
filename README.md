# CodeAlpha_BasicNetworkSniffer
Basic Network Sniffer built with Python and Scapy - CodeAlpha Cybersecurity Internship Task 1
A Python-based network packet sniffer that captures and analyzes network traffic in real-time.

**Overview**
This network sniffer demonstrates fundamental cybersecurity concepts by capturing and analyzing network packets. It provides insights into how data flows through networks and helps understand various networking protocols.

**Features**
Real-time packet capture using Scapy library
Protocol analysis for Ethernet, IP, TCP, UDP, ICMP, and ARP
Traffic detection for HTTP, HTTPS, DNS, and ICMP
Payload inspection with text decoding attempts
Interactive menu for easy operation
Network interface selection
Packet counting and filtering options

**Requirements**
Python 3.6+
Scapy library
Administrator/root privileges (required for raw socket access)

**Installation**
1. Clone this repository:
  git clone https://github.com/Codingsteez/CodeAlpha_BasicNetworkSniffer
  cd CodeAlpha_BasicNetworkSniffer
3. Install required dependencies:
  pip install scapy

Usage
Windows:
bash
# Run as Administrator
python network_sniffer.py
Linux/Mac:
bash
# Run with sudo
sudo python network_sniffer.py

**Menu Options:**
1. List network interfaces - View available network interfaces
2. Start sniffing (default interface) - Begin packet capture on default interface
3. Start sniffing (specific interface) - Choose specific network interface
4. Exit - Close the program
   
**Information Captured**
Ethernet Frame:
> Source and destination MAC addresses
> Protocol type

IP Header:
> Version and header length
> Time to Live (TTL)
> Source and destination IP addresses
> Protocol type

TCP/UDP Headers:
> Source and destination ports
> Sequence numbers (TCP)
> Flags and acknowledgments (TCP)
> Packet length (UDP)

Protocol Detection:
> HTTP traffic (port 80)
> HTTPS traffic (port 443)
> DNS queries (port 53)
> ICMP ping traffic

Raw Payload:
> First 50 bytes of packet data
> Text decoding attempts

**Security Considerations**
Important: This tool is for educational purposes only. Use responsibly and only on networks you own or have explicit permission to monitor.

> Always run with appropriate permissions
> Respect privacy and legal boundaries
> Use only for legitimate security testing and learning

**Learning Objectives**
This project helps understand:

> Network packet structure and protocols
> How data flows through networks
> Basic packet analysis techniques
> Python socket programming
> Cybersecurity monitoring concepts

Sample Output
==============================================================
PACKET #1
==============================================================
Timestamp: 2025-07-09 10:30:45.123456
Ethernet Frame:
  Source MAC: aa:bb:cc:dd:ee:ff
  Destination MAC: 11:22:33:44:55:66
  Protocol: 2048
IP Header:
  Version: 4
  Header Length: 5
  TTL: 64
  Protocol: 6
  Source IP: 192.168.1.100
  Destination IP: 8.8.8.8
TCP Header:
  Source Port: 54321
  Destination Port: 443
  [HTTPS Traffic Detected]
Packet Size: 66 bytes

Technologies Used
> Python 3: Core programming language
> Scapy: Packet manipulation and analysis library
> Socket: Low-level network interface
> Datetime: Timestamp generation

Author
Bongani Funzo
CodeAlpha Cybersecurity Intern
Student ID: CA/JU1/27523

Internship Details
> Program: CodeAlpha Cybersecurity Internship
> Duration: July 10 - August 10, 2025
> Task: Basic Network Sniffer (Task 1)
> Company: CodeAlpha

License
This project is created for educational purposes as part of the CodeAlpha internship program.

Contributing
This is an educational project. Feel free to fork and experiment for learning purposes.

Contact
For questions about this project or the internship:
> Email: services@codealpha.tech
> Website: www.codealpha.tech
