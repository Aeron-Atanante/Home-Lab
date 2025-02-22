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
![{0C9BD08A-D0DA-4312-808C-DCCC5E83DEA3}](https://github.com/user-attachments/assets/24539058-b68b-44b8-816c-c9ea8189461d)
 *Ref 3: Oracle VirtualBox Interface*
### 3.Configure Virtual Machines Network
- Create a NAT Network
![{4E53F4AA-97B1-4F4E-ABD4-84C9D9A8275E}](https://github.com/user-attachments/assets/00fac8f6-ca77-4c9d-a0f3-be0b7ab26dae)
- Configure the Network Connection of the Virtual Machines
![{9BB9B9B2-C7ED-47B6-BB69-6267E369C50C}](https://github.com/user-attachments/assets/c0ff3865-c930-4c9f-96bb-f0da5b8a6353)
![{9B6227F0-805C-496E-819B-C086C0BC7FA9}](https://github.com/user-attachments/assets/fd106560-27c5-48d7-9701-4bc7518fde37)
![{6D60D3C8-BD66-4A90-88DD-EDFCA5DD3241}](https://github.com/user-attachments/assets/f2e9a5d7-21f3-4dce-b4e9-471afda53240)

- Check the connection of the Virtual Machines
  ![{A1B8F28F-90AE-4D65-8599-CF8C9493B38F}](https://github.com/user-attachments/assets/1c9b39f2-b478-4636-9f2a-98917a72571c)

![{09385D93-5225-4EA3-B309-B7A932D60373}](https://github.com/user-attachments/assets/ce2ab19f-cb89-44f4-9dcb-8b8b5f513718)
![{138EFE10-4A54-433A-9CFB-E6DEE2658743}](https://github.com/user-attachments/assets/f17113e0-57eb-4612-b39a-c05ec1f36a77)
![{C43C36D4-D976-4B77-ACE1-7326EE7E334F}](https://github.com/user-attachments/assets/7641a363-bdb1-42c5-8224-624bae670413)
![{8BBB1AD7-74F8-4B7F-A30F-4930BD204470}](https://github.com/user-attachments/assets/10ef2e83-73e6-4895-8796-3e9e863513b9)


#### 3. Creating a Base Install Image
- Windows (Victim System)

  ![{2DF0A1EB-8CF9-4CA4-A2E6-3E07118A2518}](https://github.com/user-attachments/assets/89917059-7ea0-4cc6-8252-438a6c2e61ef)
  ![{DF87C02A-0D79-4AB1-B7E3-DB27CCD1E40C}](https://github.com/user-attachments/assets/87cb467e-b27f-468e-b00c-fe11218671b6)
  ![{A1EBB550-D8D7-44B1-AFB4-6AB20D184DA2}](https://github.com/user-attachments/assets/9904dbaa-43c7-421e-93ef-387ebb445692)

![{C3737C42-26EF-4FA6-8C61-0A9D150F968B}](https://github.com/user-attachments/assets/807301e7-5601-4cda-be75-24f116d56d16)

#### 4. SIEM 
![{26C843B0-0A9A-48B3-BE2B-0F7026838D99}](https://github.com/user-attachments/assets/56e5b825-ffab-42ce-a8ff-bccff74626b9)
![{3B5133AC-ABFC-43A7-BCB6-8C4864EED8F2}](https://github.com/user-attachments/assets/235f8557-5772-4899-abe4-9f14c538be2d)

![{60065FD5-5A8F-4022-9A41-0164E9E53F09}](https://github.com/user-attachments/assets/b941a2c9-307a-477c-9102-adea7acefcf6)
![{9705F26D-B726-4E98-A7B5-A1907507CEA2}](https://github.com/user-attachments/assets/5df97897-88a6-4234-86b4-b9194e368b77)
![{81A4B74D-7DF7-462E-841B-99E45D08F6A8}](https://github.com/user-attachments/assets/a7662a09-da0b-4db6-aca0-2f74c43b426e)
![{B1CECD6A-21EB-4232-9547-32A4B00FEFF8}](https://github.com/user-attachments/assets/750ed603-8f42-42eb-a33c-4dc3de87b33b)

snort
![{6C3CBA13-EB39-4B0D-B24B-812DDFF48DC2}](https://github.com/user-attachments/assets/52b224b6-bb28-4709-b455-53a2f0b5a58b)

![{FD3DA695-4D86-46DC-B4E9-73C7E5D0F283}](https://github.com/user-attachments/assets/2c3966ba-9c68-44e2-a0b3-33e1f09c5c87)
![{695A9D11-E96D-4E28-AEAB-77716A285CA5}](https://github.com/user-attachments/assets/bbe32ece-bdc6-4cb1-831f-6bc8b7f8f1dd)
![{19B14FB9-4679-4E8D-82D4-479D0395AD3D}](https://github.com/user-attachments/assets/3b21ec39-9ab9-4d7d-bb2e-0e50335c0f0f)
![{A8200C74-4437-4DF3-A1AD-7B65EA69ACB8}](https://github.com/user-attachments/assets/9bdb9f3e-077e-4231-a387-965c709967a1)
![{F6DAF20C-60CC-41AD-B0E3-2A97DAE97D9E}](https://github.com/user-attachments/assets/da439797-755f-40b0-8f80-1eff9337aae3)
update ipvbar



#### 4. Configure Logging & Monitoring  
- Send logs from all machines to SIEM.  

#### 5. Simulate Attacks  
- Use **Nmap, Metasploit**, and other tools.  

#### 6. Analyze Alerts in SIEM  
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





