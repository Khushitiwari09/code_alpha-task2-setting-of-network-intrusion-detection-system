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
Part II: Attack Simulation & Detection Analysis
Simulated Attacks from Kali Linux


