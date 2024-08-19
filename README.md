# Splunk and Sysmon Telemetry

## Objective
Installing & configuring Splunk & SysMon, Windows 10 Pentest, and analyzing malware.

The Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test data to simulate real-world cyber-attack scenarios. This hands-on experience was designed to deepen my understanding of network security, attack patterns, and defensive strategies.

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

## Steps
- Sysmon Install On Windows Virtual Machine</a>

![Sysmon install](https://github.com/user-attachments/assets/0fc3d7d9-0839-493f-8102-5c20a4e78a18)

![Sysmon Installed ](https://github.com/user-attachments/assets/b663be94-9d6a-479d-a648-46a9027474a5)
 
- Spunk Enterprise Install On Windows Vm </a>

![Splunk Win Virtual Box installing](https://github.com/user-attachments/assets/dcc84d62-8784-4d7b-99d9-e8328c678773)

![Splunk Installed Win Virtual Box](https://github.com/user-attachments/assets/5bfac721-0ab1-4230-bd57-9fe596957fe8)

![Splunk Running Win VirtualBox Vm](https://github.com/user-attachments/assets/3fe1293a-776e-4db7-be65-59f7a0f027e7)

- Nmap Scanning all ports on windows machine from Kali Linux attack machine with no pings </a>

![nmap -A -Pn windows machine scan](https://github.com/user-attachments/assets/306ab89a-9e83-4916-9ae8-7ea68466d169)

- Building Malware with msfvenom, opening Metasploit Handler. Setting Payload Type, Lhost, and starting exploit. Malware File name = Resume.pdf.exe.  </a>

![msfvenom Malware](https://github.com/user-attachments/assets/02fc267e-2e20-46f3-b5e4-c442620b53c7)

![msfvenom Malware Package choice](https://github.com/user-attachments/assets/4237b91e-80ea-4d7b-a988-16bb867ebdf7)

![Generating Malware ](https://github.com/user-attachments/assets/48972f57-c715-41b0-b269-7fbdcb865a1e)

![Metasploit Handler open](https://github.com/user-attachments/assets/404824da-7cc2-4b08-b60c-d44185d61963)

![Set Payload Type](https://github.com/user-attachments/assets/019e91bc-3301-43ba-b516-97c7e0e6e764)

![Payload Options Changed](https://github.com/user-attachments/assets/f2a088f8-fa58-46da-9403-6b25fc7cd7dc)

![Set Lhost](https://github.com/user-attachments/assets/ad042b06-af48-46d1-bcd5-e2143a172d14)

![Lhost options changed](https://github.com/user-attachments/assets/9d84bef7-affd-424d-8642-57f8a64f1cfd)

![Exploit started](https://github.com/user-attachments/assets/a906c1e6-37a8-48ef-9b95-f9adc8f92f1a)

- Set up Python web server for windows machine to download malicious file from host: 192.168.20.11 over port: 9999  </a>

![Set up http Server to download Malware](https://github.com/user-attachments/assets/e9582922-b489-4960-9f6a-16e1480b0155)

- Victim downloading malicious file, showing connection established with Netstat and in Task Manager </a>

![Searching for Malware package on win machine](https://github.com/user-attachments/assets/df181e14-3243-4c0e-8de3-5ea1b28a594e)

![Downloading Malware File Windows](https://github.com/user-attachments/assets/3c2b5535-669e-48a4-ac5e-a7fe57670efc)

- Netstat </a>

![Netstat -anob Connection established confirmation](https://github.com/user-attachments/assets/85680b99-8fd2-40b8-8363-e25cbcbbce3f)

- Task manager </a>

![Task Manager Malware Confirmation](https://github.com/user-attachments/assets/5ff0a610-e21a-40e5-b01a-d2f8425a9370)

- Client Captured on Kali Linux attack machine after victum executed the Resume.pdf.exe Malware file. Establishing Shell on victim machine & running commands. </a>

![Client Captured after executing Malware](https://github.com/user-attachments/assets/ab21bfd4-7bf8-414e-9022-4f6f3717be47)

![Established Shell ](https://github.com/user-attachments/assets/9a4a1edf-9325-408b-bf57-d709d2b1e594)

![Running Commands from attack machine](https://github.com/user-attachments/assets/00d6123e-c115-42db-8a47-17293af7ee46)

- Viewing Telemetry generated on Splunk of malware </a>

![index=endpoint 192 168 20 11 dest_port](https://github.com/user-attachments/assets/e9a4f195-8035-4924-8f6f-c7bf74d0e368)

![Seeing what the malware looks like](https://github.com/user-attachments/assets/9f758fe5-887f-4e23-9854-38a81140b5af)

- Expanding Event Code 1 </a>

![Expanding Event code #1 ](https://github.com/user-attachments/assets/c70c2c98-800f-474d-bb27-ffc97efe21c4)

- Using Process Guid & seeing commands run by attacker </a>

![Copied Process Guid](https://github.com/user-attachments/assets/5ea7f3f4-b8bb-425e-940d-eb4c0416e923)

![Cleaned query](https://github.com/user-attachments/assets/abed4fdd-6514-44f4-8d6d-1ca244db7df4)

