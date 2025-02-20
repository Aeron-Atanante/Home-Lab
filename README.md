# Detection Lab

## Objective

The Detection Lab project aims to establish a controlled environment for simulating and detecting cyber attacks. The primary focus is to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience will deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned
- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.




## Network Architecture
![Detection Lab Architecture](https://github.com/user-attachments/assets/cb92936d-2f70-432e-9fd6-cb7f65302eaa)

*Ref 1: Network Diagram*

This diagram represents the architecture of the detection lab, designed for monitoring and analyzing cyber threats.

- **SIEM Server (Splunk)** is at the top, acting as the central log collection and analysis system.
- **Attacker VM (Kali Linux)**  initiates attacks on the Victime System (Windows) and Web/App Server (Ubuntu) to simulate real-world threats.
- **IDS/IPS (Snort)** monitors network traffic for suspicious activity and sends alerts to the SIEM.
- **Arrows** indicate the direction of attack and log flow between components.



## Steps

#### 1. Install Oracle VirtualBox
- Download from official site.
![{BFF036C0-6E5D-4B82-8FC7-B6FC756A4F22}](https://github.com/user-attachments/assets/167e60f4-f0eb-4c9a-a7e6-c5f9cb102b17)

  *Ref 2: Oracle VirtualBox Official Site*


#### 2. Deploy Virtual Machines  
- Download Kali Linux, Windows, and Ubuntu ISO files fromm the official site.
- Deploy Kali Linux, Windows, and Ubuntu on the Oracle VirtualBox.  

#### 3. Configure Logging & Monitoring  
- Send logs from all machines to SIEM.  

#### 4. Simulate Attacks  
- Use **Nmap, Metasploit**, and other tools.  

#### 5. Analyze Alerts in SIEM  
- Investigate security incidents.  

### **Screenshots**
📸 *Ref 1: Network Diagram*  
📸 *Ref 2: SIEM Dashboard*  

---

## **Conclusion**
This lab provides hands-on experience in **threat detection, log analysis, and security monitoring**, helping to understand real-world attack patterns. 🚀  

![{5947C6A7-D937-4750-8726-DA6277C9A299}](https://github.com/user-attachments/assets/aeabe213-120a-4a86-ab06-98859202fcfb)
![{283510D9-B402-40CA-8172-2C9BCA652568}](https://github.com/user-attachments/assets/186643e4-b774-48ff-8565-e6182e4a172a)
![{18FD8E76-0373-4587-A70E-1FAC19BF453E}](https://github.com/user-attachments/assets/571104ae-9798-46ae-9aa5-6257948187c2)
![{A5E801CD-91AA-4039-BBB2-2B5DB1F68C51}](https://github.com/user-attachments/assets/7fb0fcad-deaf-4a52-8149-cc45166cf7ac)




