# Local Network Reconnaissance

## Objective
To scan the local network and identify open ports and services running on connected devices.

## Tools Used
- Nmap
- Wireshark (optional)

## Scan Command
nmap -sS 192.168.1.0/24

## Findings

### 192.168.1.1
- 22 (SSH)
- 80 (HTTP)
- 9000–9003 (Unknown services)

### 192.168.1.74
- 53 (DNS)
- 80 (HTTP)
- 443 (HTTPS)
- 8080 (Proxy)
- 8099 (Unknown)

### 192.168.1.213
- 53 (DNS)
- 80 (HTTP)
- 443 (HTTPS)

## Security Risks
- HTTP (port 80) is not encrypted and can expose sensitive data
- SSH (port 22) may be vulnerable to brute-force attacks
- Unknown ports (9000+, 8099) increase attack surface
- Open proxy ports may be abused

## Conclusion
The network contains multiple devices with open ports, some of which may pose security risks if not properly secured.
