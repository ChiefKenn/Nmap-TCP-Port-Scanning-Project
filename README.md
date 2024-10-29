Perform a TCP port scan using Nmap
Hi, I am Chief Kenn, documenting my journey as a security engineer.


Background
Nmap is a versatile network exploration and security auditing tool used to identify hosts, services, and potential security issues on a network. One of its essential
features are the ability to perform TCP port scans, which helps in identifying open ports and the services running on a target system.
Understanding the open ports and services is crucial for securing the system and mitigating potential vulnerabilities.

Exercise
In this exercise, you will utilize Nmap to perform a comprehensive TCP port scan against a remote target machine. This will enable you to identify open ports and
the associated services running on the target system.

Specifications:
1. Important
● Research what flags do before using them.

● Nmap will return "open|filtered" when it is unable to determine whether a port is open or filtered. This exercise requires you to identify "open" ports!

3. Prepare the target machine
● Start a Linux virtual machine that will serve as the target for the TCP port scan.

● Start the "apache2" service and the "ssh" service on the target virtual machine.

● Verify that the services are running on the default ports (22 and 80).

● Validate that you can detect the "open" port(s) using Nmap and the loopback address (127.0.0.1). 


5. Perform TCP Scan
● Start another Linux virtual machine with Nmap installed, which will act as the attacker machine.

● Use Nmap's TCP Connect Scan ("-sT") against the target machine to identify open ports.

● Use Nmap's TCP SYN Scan ("-sS") against the target machine to identify open ports using SYN packets.

● Use Nmap's Service Detection ("-sV") against the target machine to identify the services running on open ports.

● Use Nmap's OS Detection ("-A") against the target machine to identify the operating system running on the target system.

● Use Nmap's scan option to scan all TCP ports ("-p-") against the target machine to identify all open ports.

● For each of the scans performed using the attacker machine, ensure that Nmap successfully discovers port 22 (SSH) and port 80 (HTTP)
as "open" on the target machine.
<!---
ChiefKenn/ChiefKenn is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
