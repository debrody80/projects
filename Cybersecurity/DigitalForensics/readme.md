# Digital Forensics Final Project

**Author:** Dennis Brody  


## Overview
This project involves a forensic investigation of a crime scene with both physical and digital evidence. The incident under investigation took place in a residential kitchen, and the forensic analysis focused on digital devices such as a laptop, USB drive, and cell phone found at the scene. The case presents a combination of digital and physical elements, with potential cybersecurity and biochemical hazards involved. The primary goal of this investigation was to analyze the digital evidence, identify possible connections between the devices, and uncover any hidden or encrypted data.

## Objectives
The investigation focused on two key objectives:
1. **Laptop Forensic Analysis:** Examine the laptop found at the scene, particularly focusing on the active Nmap scan and the open applications, such as the image of the reactor on the screen. This included analyzing system logs, network activity, and running processes to understand the device's role in the crime.
2. **USB and Cell Phone Data Recovery and Analysis:** Recover and analyze the contents of the USB drive and cell phone found at the scene. This included extracting hidden, encrypted, or deleted files and reviewing call logs, text messages, and other data from the cell phone to establish any connections with the incident.

## Crime Scene Details
The crime scene was set in a residential kitchen with the following notable evidence:
- A body lying in front of the kitchen island.
- A laptop running Kali Linux, displaying an Nmap scan and an image of a reactor.
- A cup of tea containing high levels of radiation.
- A cell phone near the victim's body.
- A USB drive hidden under a coffee container at the kitchen's coffee station.

## Key Findings
### Exhibit A: HP ProBook 650 G4 Laptop
- **Operating System:** Kali Linux.
- **Key Activity:** Active Nmap scan targeting the NuScale IP subnet, suggesting potential cyber espionage or unauthorized network scanning.
- **Admin Account Change:** The laptop's admin account was changed to "JACKO SMITH" and encrypted password hashes were found, indicating attempts to secure or obscure activities.

### Exhibit B: PNY USB 2.0 Drive
- **Contents:** Contained schematics of NuScale reactors and documents related to the "Bahama Papers," indicating a connection to nuclear technology and possibly financial crimes.
- **Concealment:** The drive was hidden, indicating an attempt to protect sensitive information.

### Exhibit C: Apple iPhone 12
- **Proximity:** Found near the victim, potentially containing relevant call logs, messages, and application data related to the incident.

## Tools Used
- **Autopsy:** Digital forensics tool for analyzing file systems and recovering deleted data.
- **Nmap:** Network scanning tool found actively running on the laptop.
- **Wireshark:** Network traffic analysis tool found installed on the laptop.

## Recommendations
1. **Decryption of Encrypted Data:** Further analysis is needed to crack the encrypted hashes found on the laptop and USB drive to uncover potential crucial information.
2. **Review Network Logs:** Network logs from the NuScale IP subnet should be reviewed for unauthorized access attempts and data exfiltration.
3. **Forensic Analysis of Cell Phone:** Extracting communications and browsing history from the cell phone could provide further insights into the victim's activities before the incident.

## Conclusion
This forensic investigation uncovered significant digital evidence that points to the victim’s involvement in unauthorized network activities and possession of sensitive information related to nuclear technology and financial documents. Further investigation and analysis of encrypted data are essential for a complete understanding of the case.


