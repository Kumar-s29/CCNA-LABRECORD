# **EXERCISE 2**

## **Ethernet Concepts**

**Author**: Kumara Swamy S

---

### **1. Introduction to Ethernet**

Ethernet is one of the most widely adopted technologies for local area networks (LANs). It enables devices to communicate efficiently using protocols defined at the physical and data link layers of the OSI model. The primary goal of this experiment is to explore Ethernet's foundational concepts, such as frame structure, addressing methods, and transmission techniques, which are vital for robust network design and troubleshooting.

---

### **2. Network Interface Cards (NICs)**

- **NIC Functionality**: Network Interface Cards (NICs) serve as the hardware bridge between devices and networks, enabling data transmission. They can operate in wired (Ethernet) or wireless (WLAN) configurations.
- **Types of NICs**: Ethernet NICs support communication through twisted-pair cables, coaxial cables, or fiber-optic links, depending on the network infrastructure.
- **Roles in Ethernet**: NICs handle key functions like framing data, assigning MAC addresses, and ensuring error-free communication, making them essential for reliable network connectivity.

---

### **3. Ethernet Frame Structure**

- **Frame Components**: An Ethernet frame comprises critical fields:
  - **Destination MAC Address**: Identifies the receiving device within the network.
  - **Source MAC Address**: Specifies the sender's unique MAC address.
  - **EtherType**: Indicates the protocol being used (e.g., IPv4, ARP).
  - **Payload**: Contains the actual data being sent across the network.
  - **FCS (Frame Check Sequence)**: Validates the integrity of transmitted data by detecting errors.
- **Frame Format**: Understanding the frame's detailed structure is key to diagnosing network problems and optimizing performance.

---

### **4. MAC Addressing**

- **MAC Address**: A Media Access Control (MAC) address is a unique 48-bit identifier assigned to network devices. It ensures accurate data delivery within local networks.
- **Static vs. Dynamic Addressing**: Static addresses are manually assigned, while dynamic addressing uses ARP to resolve IP-to-MAC mappings automatically.
- **Role in Communication**: MAC addresses ensure that data packets reach their intended destination, forming the backbone of Ethernet-based communication.

---

### **5. Full-Duplex vs. Half-Duplex Communication**

- **Half-Duplex**: Data transmission occurs in one direction at a time, commonly seen in older Ethernet standards. This mode often results in collisions, reducing network efficiency.
- **Full-Duplex**: Allows simultaneous data transmission in both directions, doubling network throughput and reducing latency. Full-duplex is the default mode in most modern Ethernet environments.

---

### **6. Types of Ethernet Cables**

- **Copper Cables**: Widely used options like Cat5e and Cat6 cables are cost-effective but susceptible to electromagnetic interference, limiting their performance in high-noise environments.
- **Fiber Optic Cables**: Provide higher bandwidth, longer transmission distances, and immunity to interference, making them ideal for backbone networks and large-scale installations.

---

### **7. IPv4 and IPv6 Addressing**

- **IPv4**: A 32-bit addressing scheme represented in dotted decimal format (e.g., 192.168.1.1). While dominant today, IPv4 faces exhaustion due to limited address space.
- **IPv6**: A 128-bit scheme introduced to address IPv4's limitations. It offers a vast address space, enhanced security features, and more efficient routing mechanisms, paving the way for future networks.

---

### **8. ARP (Address Resolution Protocol)**

- **ARP Functionality**: Maps IP addresses to MAC addresses, enabling seamless communication between devices in the same network. ARP is crucial for routing data at the data link layer.
- **ARP Command**: Using `arp -a` displays a table of resolved MAC-to-IP mappings in the local network, aiding in network diagnostics and troubleshooting.

---

### **9. Practical Ethernet Setup**

- **Network Configuration**: Two devices are connected to an Ethernet switch using Cat5e or Cat6 cables. Both devices are configured with static or dynamic IPs within the same subnet to facilitate communication.
- **Data Transfer**: File transfers or ping commands verify connectivity, while performance metrics such as latency and throughput can be measured for analysis.

---

### **10. Using Wireshark for Packet Analysis**

- **Packet Capturing**: Wireshark is used to intercept Ethernet frames, providing insights into real-time data flow within a network.
- **Frame Inspection**: By analyzing captured frames, details such as source/destination MAC addresses, protocol types, and payload data can be observed, enhancing understanding of network behavior.

---

### **11. Ethernet Switch and MAC Address Table**

- **Switch Functionality**: Switches forward Ethernet frames based on MAC addresses, reducing collisions and improving network efficiency compared to hubs.
- **MAC Address Table**: A dynamic table mapping MAC addresses to specific ports on the switch is maintained, enabling precise frame forwarding and ensuring efficient communication within the network.
