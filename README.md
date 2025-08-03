# code_alpha-task2-setting-of-network-intrusion-detection-system
Network Intrusion Detection System (NIDS) using Snort, implemented on Ubuntu with Kali Linux attack simulations. Detects real-time threats like port scans and exploits through customized rules. Validated in a virtual lab environment, demonstrating effective traffic monitoring and alerting. Provides a foundation for network security hardening
# 📌 Objectives
Deploy Snort on Ubuntu as a NIDS to monitor a designated network.

Simulate reconnaissance attacks from Kali Linux using:

Nmap (port scanning, OS fingerprinting)

Evaluate Snort’s detection accuracy by analyzing generated alerts.

Document rules and configurations for reproducibility.
# Part I: Lab Environment Setup
1. Virtual Infrastructure
Attacker Machine: Kali Linux (Offensive Security Tools)

Monitored Machine: Ubuntu 22.04 LTS (Running Snort IDS)

Network: Host-only/NAT configuration to isolate lab traffic
<img width="1920" height="1080" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/7c3a932f-0977-4fbf-a442-d7f8b0983134" />
Figure 1.1: IP address and Network Interface Card for Ubuntu
<img width="1920" height="1080" alt="Screenshot (82)" src="https://github.com/user-attachments/assets/091a9124-12a1-44a2-aea4-ba5016e2ed80" />
Figure 1.2: Verifying attacking machine IP address
<img width="1920" height="1080" alt="Screenshot (83)" src="https://github.com/user-attachments/assets/0f40a6f4-1dee-4df9-a3d5-b6af75aa6a41" />
Figure 1.3: Snort successfully validated the configuration
# Part II: Attack Simulation & Detection Analysis
Simulated Attacks from Kali Linux
<img width="1920" height="1080" alt="Screenshot (84)" src="https://github.com/user-attachments/assets/20930303-73ab-4f45-8ca2-24833af85de8" />
Figure 2.1: Monitoring enabled

Kali Linux initiated an Nmap scan against an Ubuntu machine to test Snort’s reconnaissance detection.
The scan probed for open ports, services, and OS fingerprints, generating detectable network traffic.
Snort (if properly configured) should log alerts for scan patterns (e.g., SYN floods, service probes).
This simulation validates Snort’s ability to detect basic Nmap scans as part of intrusion detection.
<img width="1920" height="1080" alt="Screenshot (85)" src="https://github.com/user-attachments/assets/688988f4-88ec-4743-b071-5634ea99d24c" />
Figure 2.2: Nmap scan
Snort successfully detected the scan and generated alerts.
<img width="1920" height="1080" alt="Screenshot (93)" src="https://github.com/user-attachments/assets/160a10b4-171f-423a-a1fb-12a9b69429bd" />
Figure 2.3: Snort detecting the Nmap scan
Legion is another tool for information gathering. This tool was employed to simulate more advanced reconnaissance and network mapping attacks. Using Legion, the IP address of the Ubuntu machine was scoped, and detailed scans were performed.

The attack targeted different services running on the Ubuntu machine, attempting to map open ports and exploit known vulnerabilities.
<img width="1920" height="1080" alt="Screenshot (100)" src="https://github.com/user-attachments/assets/eb371656-d71e-4a0b-8a45-c4e537536d8c" />
Figure 2.4: adding Ubuntu machine IP address to scope
Snort was again successful in detecting these malicious activities and issued real-time alerts
<img width="1920" height="1080" alt="Screenshot (102)" src="https://github.com/user-attachments/assets/47f597c8-3ee6-42b1-a641-30f0fcd6ed18" />
Figure 2.5: Snort detecting Legion scanning attack








