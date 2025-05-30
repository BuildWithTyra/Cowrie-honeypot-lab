
# Cowrie SSH Honeypot Deployment & Attack Simulation

______________________________________________________________________________________________________

**Overview:**
Deployed a honeypot using Cowrie on an Ubuntu Server virtual machine to simulate real-world attacks. Captured and analyzed login attempts and attacker behavior in a safe lab environment. 

______________________________________________________________________________________________________

**Tools & Technologies Used:**

- Ubuntu Server 24.04 LTS (VirtualBox)
- Cowrie honeypot
- Python, virtual environments
- SSH protocol
- Linux terminal (command line)
- Log analysis with tail and cowrie.log

______________________________________________________________________________________________________

**Skills Demonstrated:**

- Configuring a cybersecurity lab
- Deploying and running a honeypot
- Simulating SSH attacks with fake credentials
- Analyzing attacker behavior through log files
- Understanding cyber deception and threat intelligence basics

______________________________________________________________________________________________________

**Screenshots:**
### Cowrie Startup Confirmation:
Cowrie honeypot initialized inside Python virtual environment, listening on port 2222.
![IMG_2357](https://github.com/user-attachments/assets/db96807d-e1b8-4d88-ae17-ef3f15f8d8ea)
### Live Log Monitoring:
Used tail -f cowrie.log to monitor honeypot activity in real time. This simulates how defenders watch for suspicious behavior and analyze live security logs on a production system. 
### Captured login Attempt:
Cowrie logged a brute-force SSH attempt using the credentials root / 123456. The honeypot blocked the attempt and recorded it in the logs, showing how fake services can deceive and log attacker behavior
![IMG_7FFBC3E6-CE9F-47D8-B6B5-09E1AF864954](https://github.com/user-attachments/assets/7182dc6e-5aae-4e2d-a816-dcfd9c309c85)
### Confirmation that it is actively listening:
Even though Cowrie is configured by default to listen on port 2222, here’s a confirmation that it is actively listening on TCP port 2222 using the s s command. 

This port is used to simulate a real SSH service and attract unauthorized login attempts, allowing me to safely observe attacker behavior inside a controlled honeypot environment. 
![image0](https://github.com/user-attachments/assets/5fd1b679-ce1a-447f-8253-d371a83049a1)

______________________________________________________________________________________________________

**Key Takeaways:**

- Practiced hands-on cybersecurity defense with honeypot technologies
- Gained working experience with SSH protocol, logging, and service detection
- Learned how attackers attempt to brute-force logins and how those actions are logged
- Saw the value of threat deception and how honeypots contribute to threat intel

______________________________________________________________________________________________________

**Reflection / What I Learned:**

Before this project, I had never deployed a honeypot or seen real-time simulated attacks in action. Setting up Cowrie from scratch gave me hands-on experience with virtual machines, Linux administrations, Python environments, and log analysis. I learned how to validate that a service is running, interpret log data, and simulate attacker behavior in a controlled way. 

Most importantly, I learned how valuable logs are for detecting and understanding malicious behavior, and how defenders can use deception (like honeypots) to turn the tables on attackers. I now feel more confident in my ability to spot and analyze security events in real-world systems. 

______________________________________________________________________________________________________

**Project Status:**
Completed - May 2025

Repeatable lab - can be shared, taught, or expanded for future use

______________________________________________________________________________________________________

**Next Steps / Improvements**

- Add local or cloud-based log aggregation ( e.g., ELK Stack or Splunk)
- Run honeypot on a real internal network for more realistic data
- Schedule automated log parsing for attacker trend analysis
- Test with additional honeypot services (e.g., HTTP, FTP)

______________________________________________________________________________________________________
