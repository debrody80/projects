# Home Lab Project

This project showcases a fully functional home lab environment, built using a Dell R730 server and Proxmox for virtualization. The lab is segmented into multiple VLANs for specific security and network testing purposes. Below is a breakdown of the setup and configuration of this project.

## Technologies Used
- **Proxmox**: Hypervisor for managing virtual machines
- **pfSense**: Firewall and router for network segmentation and VLAN setup
- **Kali Linux**: For penetration testing and security analysis
- **Nessus**: Vulnerability scanning and assessment tool
- **Windows Server 2019**: Domain Controller for a Windows enterprise environment
- **Windows 10 and 11 Clients**: Workstation environments connected to the domain
- **Metasploitable 2, DVWA, VulnHub**: Vulnerable virtual machines for exploitation practice
- **Ubuntu**: Hosting Docker and Portainer for container management
- **DVWA, WebGOAT, BWApp**: Vulnerable web applications for security testing
- **Wazuh**: Security monitoring and intrusion detection system (IDS) for real-time threat detection

## Lab Overview

### 1. pfSense Firewall & VLANs
The lab utilizes **pfSense** to manage firewall rules and create isolated VLANs for different network segments:
- **VLAN 10**: Scanning/attack LAN
- **VLAN 20**: Windows enterprise environment
- **VLAN 30**: Vulnerable machine network
- **VLAN 40**: Ubuntu instance with Docker and Portainer

### 2. Scanning/Attack LAN
This LAN contains **Kali Linux** and **Nessus**, used for penetration testing and vulnerability scanning on other segments of the network.

### 3. Windows Enterprise Environment
A separate VLAN houses a fully functioning Windows domain, including:
- **Windows Server 2019 Domain Controller**: Manages Active Directory, DNS, and DHCP services.
- **Windows 10 and 11 Clients**: Domain-joined workstations for testing domain policies and configurations.

### 4. Vulnerable Machine LAN
This network segment contains intentionally vulnerable machines to practice penetration testing and exploitation:
- **Metasploitable 2**
- **Damn Vulnerable Web Application (DVWA)**
- **VulnHub VMs**

### 5. Ubuntu with Docker and Portainer
In this segment, an **Ubuntu** instance runs **Docker** and **Portainer** to manage and deploy web application containers, including:
- **DVWA**
- **WebGOAT**
- **BWApp**

These web applications are purposefully vulnerable to allow for web security testing, including OWASP Top 10 vulnerabilities.

### 6. Wazuh for Monitoring
**Wazuh** is installed to monitor the entire environment for security threats. It acts as an intrusion detection system (IDS) and provides real-time alerts for suspicious activities within the network. Wazuh helps track file integrity, monitor system logs, and detect unauthorized access or potential breaches.

## Key Features
- **Virtualized Infrastructure**: The entire setup is virtualized using Proxmox, making it flexible and easy to manage.
- **Network Segmentation**: Each segment is isolated by VLANs to mimic real-world network environments and facilitate focused testing.
- **Vulnerability Testing**: The lab provides a variety of vulnerable machines and web applications for extensive penetration testing practice.
- **Containerized Web Applications**: Ubuntu instance with Docker simplifies the deployment and management of vulnerable web applications.

## Future Plans
- Add more vulnerable machines to expand testing opportunities.
- Automate the setup using Infrastructure as Code (IaC) tools like Ansible or Terraform.
- Integrate more advanced attack vectors and security tools like SIEM solutions.

## Getting Started
To replicate this home lab:
1. Set up **Proxmox** on a physical server or virtual environment.
2. Install **pfSense** and configure VLANs for network segmentation.
3. Deploy the virtual machines as described above, ensuring appropriate networking for each VLAN.
4. Download and install the necessary software (Kali, Nessus, Windows Server, etc.).
5. Configure Docker and Portainer on the Ubuntu instance to host web applications.

