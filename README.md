# pfSense & Suricata IDS/IPS Lab
I built this lab to gain practical experience configuring and managing a firewall and IDS/IPS, specifically to understand how network threats are detected, logged, and prevented in real time. My goal was to become comfortable navigating alert logs, tuning rule sets, and simulating real-world traffic to better understand how security teams monitor and respond to potential intrusions.

## Tools & Technologies Used

- VirtualBox (Home Lab Environment)
  - Ubuntu (24.04.2)
  - Kali-linux
- pfSense (Firewall)
- Suricata (IDS/IPS)
  - Emerging Threats Rule Set

## What This Lab Does
- Sets up pfSense as the primary firewall and router within a virtual or physical home lab environment.
- Installs and configures Suricata to monitor traffic on the WAN and LAN interface.
- Enables IDS and IPS modes to detect and automatically block suspicious or malicious activity.
- Integrates Emerging Threats rule set to detect common attacks.
- Captures, logs, and displays real-time alerts through the pfSense GUI.

