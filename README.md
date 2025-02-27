# Home Lab

## Objective

This project involves the creation of a home lab to develop a comprehensive understanding of network infrastructure and virtualization. The lab is designed to facilitate hands-on learning by configuring systems, managing virtual environments, and exploring fundamental networking concepts. By establishing this controlled environment, the project aims to enhance practical knowledge and technical proficiency in network administration and virtualization technologies.

### Skills Learned
- Hands-on experience in configuring and managing virtualized environments.
- In-depth understanding of network infrastructure and system administration.
- Proficiency in setting up and managing multiple operating systems.
- Enhanced knowledge of virtualization technologies and resource allocation.
- Improved troubleshooting and problem-solving skills in networking and system management.

### Tools Used
- Oracle VirtualBox for creating and managing virtual machines.
- Operating Systems: Kali Linux, Ubuntu, and Windows 10 for diverse system configurations.
- Networking Tools to explore and analyze network configurations and connectivity.




## Network Architecture
![Network_Architecture](https://github.com/user-attachments/assets/98bbbe9f-d704-4069-adc0-c9d5f952c03f)


*Reference Image: Network Diagram*

This network diagram allows the VMs to communicate with each other while also enabling external connectivity through the NAT network

- **Host Machine (Oracle VirtualBox)** Manages all virtual machines.
- **NAT Network**  Provides network connectivity between the VMs while allowing them to access the internet through the host.
- **Kali Linux VM** Used for penetration testing and security tools.
- **Ubuntu VM** Functions as a server environment.
- **Windows 10 VM** Acts as a client or workstation.


## Steps

## 1. Install Oracle VirtualBox  
- Download and install **Oracle VirtualBox** from the [official website](https://www.virtualbox.org/).  
- Ensure the installation is successful before proceeding with virtual machine setup.

![{BFF036C0-6E5D-4B82-8FC7-B6FC756A4F22}](https://github.com/user-attachments/assets/167e60f4-f0eb-4c9a-a7e6-c5f9cb102b17)

  *Reference Image: Oracle VirtualBox Official Site*  


## 2. Deploy Virtual Machines  
- Download the latest ISO files for **Kali Linux, Windows 10, and Ubuntu** from their respective official websites.  
- Open **Oracle VirtualBox** and create a new virtual machine for each operating system.  
- Assign appropriate system resources (CPU, RAM, and storage) to each VM based on recommended specifications.  
- Complete the OS installation process for all three virtual machines.  

 ![{0C9BD08A-D0DA-4312-808C-DCCC5E83DEA3}](https://github.com/user-attachments/assets/24539058-b68b-44b8-816c-c9ea8189461d)
  *Reference Image: Oracle VirtualBox Interface*

## 3. Configure Virtual Machine Network  

### A. Create a NAT Network  
- In **Oracle VirtualBox**, navigate to **File > Preferences > Network** and create a **NAT Network** to allow VMs to communicate while providing internet access.

![{4E53F4AA-97B1-4F4E-ABD4-84C9D9A8275E}](https://github.com/user-attachments/assets/00fac8f6-ca77-4c9d-a0f3-be0b7ab26dae)
*Reference Image: Oracle VirtualBox Network Tools Section*  

### B. Configure Network Connection for Each VM  
- Assign each virtual machine to the **NAT Network** through **VirtualBox Settings > Network > Adapter 1 > NAT Network**.  
- Set static or dynamic IP addresses as needed within each OS’s network settings.  


 ![{9BB9B9B2-C7ED-47B6-BB69-6267E369C50C}](https://github.com/user-attachments/assets/c0ff3865-c930-4c9f-96bb-f0da5b8a6353)

 *Reference Image: Ubuntu VM Network Configuration*


 ![{9B6227F0-805C-496E-819B-C086C0BC7FA9}](https://github.com/user-attachments/assets/fd106560-27c5-48d7-9701-4bc7518fde37)

 *Reference Image: Kali Linux VM Network Configuration*


 ![{6D60D3C8-BD66-4A90-88DD-EDFCA5DD3241}](https://github.com/user-attachments/assets/f2e9a5d7-21f3-4dce-b4e9-471afda53240)

 *Reference Image: Windows 10 VM Network Configuration*

### C. Disable Windows 10 Firewall  
- On the **Windows 10 VM**, go to **Windows Security > Firewall & network protection** and disable the firewall to allow unrestricted communication between VMs.

![{A1B8F28F-90AE-4D65-8599-CF8C9493B38F}](https://github.com/user-attachments/assets/1c9b39f2-b478-4636-9f2a-98917a72571c)
*Reference Images: Windows Security Settings*  

### D. Test Network Connectivity  
- Use the `ping` command within each VM’s terminal to verify connectivity between machines.  
- A successful ping response confirms proper network configuration.

![{8BBB1AD7-74F8-4B7F-A30F-4930BD204470}](https://github.com/user-attachments/assets/10ef2e83-73e6-4895-8796-3e9e863513b9)
*Reference Image: Ping command output validating connectivity*  



### 4. Creating a Base Install Image  
- To preserve the clean install state, take a **VirtualBox snapshot**.
- This allows for easy rollback in case of misconfigurations or testing failures.

![Windows 10 Installation Setup](https://github.com/user-attachments/assets/89917059-7ea0-4cc6-8252-438a6c2e61ef)
*Reference Image:Windows 10 VM*  

![Windows 10 Initial Configuration](https://github.com/user-attachments/assets/87cb467e-b27f-468e-b00c-fe11218671b6)
*Reference Image: Ubuntu VM*  

![Windows 10 Network & Update Settings](https://github.com/user-attachments/assets/9904dbaa-43c7-421e-93ef-387ebb445692)
*Reference Image: Kali Linux VM*  


---

## **Conclusion**
This project successfully established a home lab environment to enhance practical knowledge of network infrastructure and virtualization. By configuring and managing multiple virtual machines using Oracle VirtualBox, the lab provided hands-on experience with system administration, networking concepts, and resource allocation. The use of Kali Linux, Ubuntu, and Windows 10 allowed for a diverse exploration of operating systems, fostering a deeper understanding of virtualization technologies. Additionally, implementing a NAT network ensured controlled connectivity between virtual machines while maintaining external access. This setup serves as a foundational platform for further learning and experimentation in network management and system security.






