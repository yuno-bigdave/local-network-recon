# Network Scan Task

## Objective
To scan local network and identify open ports.

## Tools Used
- Nmap
- Wireshark

## Scan Command
nmap -sS 192.168.1.0/24

## Findings
- Port 22 (SSH) open
- Port 80 (HTTP) open

## Risks
- HTTP is not secure
- SSH vulnerable to brute force

## Conclusion
The network has multiple open ports which could pose security risks.
