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
- port 9000-9003(unknown) open
- port 8080(proxy) open

## Risks
- HTTP is not secure
- SSH vulnerable to brute force
- Big attack surface
- proxy port can be abused

## Key Security Observations
1. **Prescence of open web services**
   multiple devices have **port 80 open**
   - data is transmitted in plaintext
   - Vulnerable to sniffing(can be seen in wireshark)
  
2. **SSH exposure**
   -Risk of Bruteforce attacks & Unauthorized access

3. **Unknown ports**
   - ports **9000-9003** could be potential vulnerabilities, misconfigured services

## Conclusion
The network has multiple open ports which could pose security risks.
