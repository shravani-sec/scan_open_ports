Task 1 of the Cyber Security Internship

## 🔍 Assignment: Check Local Networks for Open Ports

### ✅ Goal
to use Nmap to find open ports on local network devices and comprehend possible threats.

### 🛠️ Utilized Tools: Windows 10 Operating System; Nmap (TCP SYN scan)

### 🌐 Network Target Information
10.230.187.74 is the target IP.
- Scan Range: One IP
Type of Scan: TCP SYN scan
- Command Used: ```bash nmap -sS 10.230.187.74

📊 Scan Findings

The Port State Service

135/tcp open msrpc 139/tcp open netbios-ssn 445/tcp open microsoft-ds 5357/tcp open wsdapi 16992/tcp open amt-soap-http


🔐 Perspectives

Malware (like WannaCry) frequently targets ports 135, 139, and 445, which are frequently used in Windows networking.

Web Services on Devices (WS-Dis) use port 5357.
