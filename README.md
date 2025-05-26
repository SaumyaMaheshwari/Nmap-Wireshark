Conducted network reconnaissance by installing and using Nmap on a Linux system.
Identified the local IP range (192.168.1.0/24) using the ip a command.

Executed a TCP SYN scan with the following command:
bash
Copy
Edit
sudo nmap -sS 192.168.1.0/24
Discovered an active Windows machine at IP address 192.168.1.9, with open ports 135, 139, and 445.

Detected the following services on the host:
Microsoft RPC
NetBIOS
SMB (Server Message Block)

Attempted to run Nmap’s default vulnerability scripts on SMB-related ports. Some scripts failed to complete due to firewall restrictions or unsupported SMB versions.
Simultaneously captured network traffic with Wireshark on interface eth0.
Used filters such as ip.addr == 192.168.1.11 to isolate scan-related packets.
Saved the traffic capture as a .pcapng file for later analysis and reporting.
