# NetworkMiner Traffic Analysis Project
# Network Analysis Portfolio

## Objective
To demonstrate my skills in network forensics and packet capture analysis using **NetworkMiner**. The following project showcases the extraction of network information such as IP addresses, packet data, and login credentials from `.pcap` files.

---

## Tools Used
- **NetworkMiner 2.7.2**: Network forensic analysis tool for Windows.
- **Ubuntu**: Operating system used to run NetworkMiner.
- **Wireshark**: An additional tool for detailed packet analysis (optional).

---

## Skills Learned
- Analyzing and extracting metadata from `.pcap` files.
- Identifying hosts, packets, and traffic details from network captures.
- Extracting login credentials such as usernames and passwords.
- Interpreting HTTP, DNS, and TCP traffic for deeper insights.

---

## Project Steps

### 1. Setup
- Installed **NetworkMiner 2.7.2** on an **Ubuntu** virtual machine.
- Loaded `.pcap` files for forensic analysis.

### 2. Analysis of `mx-3.pcap`
- **Number of frames**: 460
- **IP addresses sharing the same MAC address**: 2
- **Number of packets sent from host 65.208.228.223**: 72
- **Webserver banner** for host `65.208.228.223`: Apache

### 3. Analysis of `mx-4.pcap`
- **Username extracted**: #B\Administrator
- **Password extracted**: $NETNTLMv2$#B$136B077D942D9A63$FBBF3C253926907AAAAD670A9037F2A$501010000000000000000000094D71AE38CD60170ABD571127

---

## Screenshots
Below are screenshots demonstrating the analysis process and the results:

### NetworkMiner 2.7.2 Interface
![NetworkMiner 2.7.2](https://via.placeholder.com/150)

### Extracted Metadata from `mx-3.pcap`
![Extracted Metadata](https://via.placeholder.com/150)

### Extracted Credentials from `mx-4.pcap`
![Extracted Credentials](https://via.placeholder.com/150)

---

## Conclusion
This project highlights my proficiency in network forensic analysis and demonstrates my ability to work with packet capture tools like NetworkMiner. By extracting crucial metadata and sensitive credentials, I can identify potential vulnerabilities within a network.



