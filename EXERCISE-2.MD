# EXERCISE 2

## **Ethernet Concepts**

**Author**: Kumara Swamy S

---

### **1. Introduction to Ethernet**

Ethernet is one of the most commonly used technologies for local area networks (LANs). It facilitates communication between devices through physical and data link layers in the OSI model. The goal of this experiment is to understand the core concepts of Ethernet, including its frame structure, addressing methods, and transmission techniques.

---

### **2. Network Interface Cards (NICs)**

- **NIC Functionality**: Network Interface Cards (NICs) are hardware components that connect devices to a network. They can be Ethernet-based for wired networks or WLAN-based for wireless networks.
- **Types of NICs**: Ethernet NICs support communication using twisted-pair cables or fiber-optic links.
- **Roles in Ethernet**: NICs are responsible for framing data, adding MAC addresses, and ensuring proper transmission over the network.

---

### **3. Ethernet Frame Structure**

- **Frame Components**: An Ethernet frame consists of several fields:
  - **Destination MAC Address**: The address of the receiving device.
  - **Source MAC Address**: The address of the sending device.
  - **EtherType**: Identifies the protocol used (e.g., IPv4, ARP).
  - **Payload**: The actual data being transmitted.
  - **FCS (Frame Check Sequence)**: Ensures error detection in the transmission.
- **Frame Format**: Understanding how the frame is structured helps troubleshoot network issues and ensure efficient data delivery.

---

### **4. MAC Addressing**

- **MAC Address**: Every Ethernet device has a unique MAC address, which is used to identify it on a network.
- **Static vs. Dynamic Addressing**: Static addresses are manually assigned, while dynamic addresses are learned via protocols like ARP (Address Resolution Protocol).
- **Role in Communication**: MAC addresses are used to direct data packets to specific devices on the local network.

---

### **5. Full-Duplex vs. Half-Duplex Communication**

- **Half-Duplex**: Data can travel in only one direction at a time. It is used in older Ethernet technologies.
- **Full-Duplex**: Data can travel simultaneously in both directions, improving network efficiency. Most modern Ethernet networks operate in full-duplex mode.

---

### **6. Types of Ethernet Cables**

- **Copper Cables**: Such as Cat5e and Cat6 cables, are commonly used for Ethernet networking. They are cheaper but more prone to interference.
- **Fiber Optic Cables**: These offer higher bandwidth and longer transmission distances, ideal for large-scale networks.

---

### **7. IPv4 and IPv6 Addressing**

- **IPv4**: The standard 32-bit addressing format, often written as four octets (e.g., 192.168.1.1). It is widely used but has a limited address space.
- **IPv6**: A newer 128-bit format designed to overcome the limitations of IPv4 by providing a larger address space and better routing efficiency.

---

### **8. ARP (Address Resolution Protocol)**

- **ARP Functionality**: ARP is used to map IP addresses to MAC addresses, enabling devices to communicate effectively within a local network.
- **ARP Command**: By using the `arp -a` command, you can view the MAC addresses associated with IP addresses in your local network.

---

### **9. Practical Ethernet Setup**

- **Network Configuration**: Two devices are connected to an Ethernet switch using Cat5e or Cat6 cables. Both devices are assigned IP addresses within the same subnet.
- **Data Transfer**: File transfers are performed between the two devices to verify connectivity and observe Ethernet performance.

---

### **10. Using Wireshark for Packet Analysis**

- **Packet Capturing**: Wireshark is used to capture and analyze Ethernet frames as they travel across the network.
- **Frame Inspection**: Inspecting captured frames helps visualize how the data is framed, including destination/source MAC addresses and protocol types.

---

### **11. Ethernet Switch and MAC Address Table**

- **Switch Functionality**: Switches are responsible for forwarding Ethernet frames based on MAC addresses. Each port on a switch learns the MAC addresses of connected devices.
- **MAC Address Table**: The switch builds a table that maps MAC addresses to specific ports, enabling efficient frame forwarding.
