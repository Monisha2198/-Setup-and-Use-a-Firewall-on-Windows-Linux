Setup-and-Use-a-Firewall-on-Windows-Linux
To configure and test basic firewall rules in Windows to allow or block network traffic.

Tools Used:
Windows Defender Firewall
Windows Defender Firewall with Advanced Security

1.Opened Firewall Settings:
   -Searched for Windows Defender Firewall from the Start menu and opened it.
   -Clicked on Advanced Settings to manage inbound/outbound rules.
   
2.Listed Current Firewall Rules:
   -Navigated to Inbound Rules and Outbound Rules.
   -Reviewed the list of existing rules.
   
3.Blocked Inbound Traffic on Port 23 (Telnet):
  -Selected Inbound Rules → New Rule.
  -Chose Port → Selected TCP → Entered 23.
  -Chose Block the connection → Applied it to all profiles.
  -Named the rule "Block Telnet" and created it.
  
4.Tested the Rule:
  -Used telnet localhost 23 in Command Prompt.
  -Connection was refused, confirming the port was successfully blocked.
  
5.Allowed SSH Port (22):
  -Created another rule to allow TCP port 22 for SSH (for demonstration).
  
6.Removed Block Rule to Restore State:
  -Located Block Telnet rule in Inbound Rules.
  -Right-clicked and Deleted it.
  
How a Firewall Filters Traffic

A firewall acts as a security gate between your computer and the network. It filters incoming and outgoing network traffic based on predefined rules.
1. Traffic Filtering
   - Inspects data packets for source/destination IP address, port number, and protocol.
   - Allows or blocks traffic based on set rules.

2. Inbound vs. Outbound Rules
   - Inbound rules control incoming traffic to your system.
   - Outbound rules control outgoing traffic from your system.

3. Port-Based Control
   - Blocks or allows specific network ports (e.g., port 23 for Telnet, port 22 for SSH).

4. Application-Level Control
   - Can filter traffic based on the application requesting or receiving data.

5. Windows Firewall Profiles
   - Applies rules to different network types:
     - Domain (corporate network)
     - Private (home/trusted)
     - Public (open networks like Wi-Fi)
     - 
Firewalls help protect systems from:
- Unauthorized access
- Malware or suspicious traffic
- Data leaks and intrusions

They are essential in both personal computers and enterprise-level networks to enforce security policies and reduce attack surfaces.

  
  

