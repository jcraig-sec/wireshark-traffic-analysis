# Network Traffic Analysis in a Virtualized Environment

## Objective
Demonstrate understanding of modern encrypted network traffic by capturing and
analyzing VM-generated traffic using Wireshark.

## Environment
- Host OS: macOS (Apple Silicon)
- VM Platform: UTM
- Guest OS: Ubuntu Linux (ARM)
- Network Mode: Shared / NAT
- Capture Tool: Wireshark

## Methodology
- Deployed an Ubuntu virtual machine using shared networking
- Captured traffic on the host Wi-Fi interface
- Generated controlled network traffic from the VM
- Applied protocol and IP-based display filters in Wireshark

## Traffic Observed
- ICMP: Verified connectivity using echo requests and replies
- DNS: Captured domain name resolution queries and responses
  ### DNS Query Example

![DNS Query Screenshot](screenshots/dns-query.png)
- HTTPS: Observed TLS handshakes and encrypted payloads

## Key Insight
Modern web traffic is encrypted by default. While packet capture allows
visibility into metadata such as DNS queries and TLS handshakes, application
payloads remain protected. This project focuses on realistic defensive
visibility rather than bypassing encryption.

## Files
- Packet capture (.pcapng)
- Screenshots demonstrating DNS, TLS, and filtered traffic
- 
