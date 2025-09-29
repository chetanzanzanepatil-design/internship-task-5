# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## 🎯 Objective
The purpose of this task is to capture live network packets using **Wireshark**, analyze them, and identify different protocols and traffic types.

---

## ⚙️ Tools Used
- **Wireshark** (free, open-source packet analyzer)
- Active network interface (Wi-Fi/Ethernet)

---

## 📝 Steps Performed
1. Installed **Wireshark** on my system.  
2. Selected the **active network interface** (Wi-Fi).  
3. Started packet capture and generated traffic by:  
   - Visiting websites  
   - Pinging a server (`ping google.com`)  
4. Stopped the capture after ~1 minute.  
5. Applied filters in Wireshark to analyze protocols, such as:  
   - `udp` → Show UDP traffic  
   - `tcp` → Show TCP traffic  
   - `dns` → Show DNS queries  
6. Saved the capture as a `.pcap` file.  

---

## 🔍 Findings
From the captured data, the following protocols were identified:

1. **UDP (User Datagram Protocol)**  
   - Connectionless and faster but less reliable.  
   - Example: Multiple packets exchanged between local IP `192.168.1.3` and Google servers (`142.250.x.x`).  

2. **TCP (Transmission Control Protocol)**  
   - Connection-oriented and reliable.  
   - Example: TCP three-way handshake (`SYN`, `SYN-ACK`, `ACK`) observed.  

3. **TLSv1.2 (Transport Layer Security)**  
   - Used to secure communication over HTTPS.  
   - Example: Packets showing `Client Hello` and `Server Hello` exchanges for encrypted communication.  

4. **DNS (Domain Name System)** *(if captured during session)*  
   - Resolves domain names into IP addresses.  
   - Example: DNS query to resolve hostnames like `google.com`.  

---

## 📂 Deliverables
- **Packet Capture File:** `task5_capture.pcap`  
- **Screenshots:**  
  - UDP traffic  
  - TCP/TLS traffic  
- **Report File:** `README.md` (this file)  

---

## 📘 Key Learnings
- Understood how Wireshark captures real-time packets.  
- Learned how to filter and analyze traffic by protocol.  
- Observed differences between **TCP** and **UDP**.  
- Saw how **TLS** encrypts HTTPS communication.  

---

## ❓ Interview Questions (Prep)
- What is Wireshark used for?  
- What is a packet?  
- How do you filter packets in Wireshark?  
- Difference between TCP and UDP?  
- What is a DNS query packet?  
- Can Wireshark decrypt encrypted traffic?  

