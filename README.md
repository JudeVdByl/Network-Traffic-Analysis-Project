# NetworkMiner Traffic Analysis Project

## Overview
This project involves analyzing network traffic captured in PCAP files. Using **NetworkMiner**, a network forensic analysis tool, we examine network traffic for specific hosts and extract key details such as web server banners, usernames, and packet counts.

## Tools Used
- **NetworkMiner 2.7.2**: A network forensic analysis tool used to parse and analyze PCAP files.
- **Wireshark**: A network protocol analyzer to complement traffic inspection.
- **Operating System**: Linux (Ubuntu) for packet analysis.

## PCAP File Analysis

### 1. **mx-3.pcap**
- **Total number of frames**: `460`
- **IP addresses sharing the MAC address of host 145.253.2.203**: `2`
- **Packets sent by host 65.208.228.223**: `72`
- **Webserver banner under host 65.208.228.223**: `Apache`

#### Screenshots:
![NetworkMiner mx-3 Analysis](https://github.com/user-attachments/assets/51358a05-71ff-480b-94f6-ad4d41dfe50e)


### 2. **mx-4.pcap**
- **Extracted Username**: `#B\Administrator`
- **Extracted Password**: `$NETNTLMv2$#B136B077D942D9A63$FBBF3C253926907AAAAD670A903F2A550100000000000000094D71AE38CD60170ABD571127`

#### Screenshots:
![NetworkMiner mx-4 Analysis](https://github.com/user-attachments/assets/680a25eb-45d0-4455-87e3-867d2c8490a4)


## Key Findings
- Hosts using the same MAC address as host `145.253.2.203` indicate network bridging or load balancing.
- Host `65.208.228.223` is running an Apache server, sending a total of `72` packets during the captured session.
- An **NTLMv2 hash** was captured, revealing potential security vulnerabilities in the network.

## Conclusion
This analysis highlights the importance of monitoring network traffic to identify unauthorized access attempts and exposed credentials. Future steps will include deeper packet analysis, decryption attempts on captured hashes, and further inspection of the webserver security.

