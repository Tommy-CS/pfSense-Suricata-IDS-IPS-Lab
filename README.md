# pfSense & Suricata IDS/IPS Lab
I built this lab to gain practical experience configuring and managing a firewall and IDS/IPS, specifically to understand how network threats are detected, logged, and prevented in real time. I began by experimenting with firewall rules in pfSense to understand how traffic is allowed or denied. Once I was comfortable with that, I moved on to configuring alerts and blocking suspicious traffic using Suricata. My goal was to become comfortable navigating alert logs, tuning rule sets, and simulating real-world traffic to better understand how security teams monitor and respond to potential intrusions. 

## Tools & Technologies Used

- VirtualBox (Home Lab Environment)
  - Ubuntu (24.04.2)
  - Kali-linux
-Wireshark
- pfSense (Firewall)
- Suricata (IDS/IPS)
  - Emerging Threats Rule Set

## What This Lab Does
- Sets up pfSense as the primary firewall and router within a virtual or physical home lab environment.
- Installs and configures Suricata to monitor traffic on the WAN and LAN interface.
- Enables IDS and IPS modes to detect and automatically block suspicious or malicious activity.
- Integrates Emerging Threats rule set to detect common attacks.
- Captures, logs, and displays real-time alerts through the pfSense GUI.

## Screenshots (before Suricata, just using pfSense)

Using Kali, I am using hping3 to flood my device:
<img src="https://github.com/user-attachments/assets/6f136ebf-5bba-4e4d-9878-f2a9aaefad1d" width="600"/>

Wireshark hping3 results:
<img src="https://github.com/user-attachments/assets/513d5f80-fe0e-4c21-9063-e180b25b74f8" width="600"/>

Now, I have implemented a pfSense rule to block TCP traffic from Kali:
<img src="https://github.com/user-attachments/assets/b80dee63-1d64-4366-a23e-60e8cc1d3643" width="600"/>

Now, with my new "Block Kali DoS" rule set up, the hping3 pings get blocked:
<img src="https://github.com/user-attachments/assets/113e5009-08d0-49ef-b20d-2017c25d4af9" width="600"/>

## Screenshots (Now, using Suricata)
After setting up my Suricata IDS, alerts can be seen now.

hping3:
<img src="https://github.com/user-attachments/assets/cc892952-a559-4426-ac5a-37dff1a401b4" width="600"/>

nmap:
<img src="https://github.com/user-attachments/assets/daac497a-66b1-4bfe-8574-0adca26ea770" width="600"/>

Then, I configured my 
