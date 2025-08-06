Task: Scan Local Network for Open Ports

###  Objective
To discover open ports on devices in the local network and understand potential risks using Nmap.

###  Tools Used
- Nmap (TCP SYN scan)
- Operating System: Windows 10

###  Network Target Details
- Target IP: 10.230.187.74
- Scan Range: Single IP
- Scan Type: TCP SYN scan
- Command Used:
```bash
nmap -sS 10.230.187.74

 Scan Results

Port	State	Service

135/tcp	open	msrpc
139/tcp	open	netbios-ssn
445/tcp	open	microsoft-ds
5357/tcp	open	wsdapi
16992/tcp	open	amt-soap-http
  

 Observations

Ports 135, 139, and 445 are commonly used in Windows networking and are often targeted by malware (e.g., WannaCry).

Port 5357 is used for Web Services on Devices (WS-Discovery) — can leak information.

Port 16992 is related to Intel AMT for remote management and should be secured or disabled if not needed.


 Recommendations

Disable unused services and ports.

Use firewalls to limit external access to critical ports.

Ensure Intel AMT features are password protected or disabled if not in use.

Regularly audit open ports in the network.
