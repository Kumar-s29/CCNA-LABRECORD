# **Exercise 3: Communicating Between Networks**

**Author**: Kumara Swamy S

---

### **1. Introduction to Network Communication**

- Communication between networks involves transferring data from one network to another.
- Routers play a critical role in this process, forwarding packets based on destination IP addresses.

---

### **2. Role of Routers**

- **Function**: Routers connect multiple networks, making decisions about where to send data packets.
- **Routing Table**: A router uses a routing table to find the best path to route packets.

---

### **3. IP Addressing and Subnetting**

- **IP Addressing**: Each device on a network has a unique IP address (IPv4 or IPv6).
- **Subnetting**: Divides larger networks into smaller subnets, each with its own unique IP range.
- **Subnet Mask**: Helps identify the network portion and the host portion of an IP address.

---

### **4. Default Gateway**

- The **Default Gateway** routes traffic from a local network to other networks (e.g., the internet).
- It is typically the router connected to the external network.

---

### **5. Routing Between Different Networks**

- **Inter-Network Communication**: Devices in different networks cannot directly communicate unless connected by a router.
- The router forwards data packets between networks by looking at destination IPs and determining the best route.

---

### **6. Routing Protocols**

- **Dynamic Routing**: Routers automatically update their routing tables using protocols like:
  - **RIP (Routing Information Protocol)**: A distance-vector protocol based on hop count.
  - **OSPF (Open Shortest Path First)**: A link-state protocol based on path cost.
  - **BGP (Border Gateway Protocol)**: Used for routing between different autonomous systems (e.g., between ISPs).
- **Static Routing**: Routes are manually configured and remain constant unless changed.

---

### **7. NAT (Network Address Translation)**

- **Purpose**: Allows multiple devices on a private network to share a single public IP address when accessing the internet.
- **Types of NAT**:
  - **Static NAT**: One-to-one mapping between local and global IP addresses.
  - **Dynamic NAT**: Multiple local IPs mapped to a pool of public IPs.
  - **PAT (Port Address Translation)**: Multiple devices share a single public IP, distinguished by port numbers.

---

### **8. Testing Communication Between Networks**

- **Ping Command**: Used to test connectivity between devices across different networks.
- **Traceroute Command**: Traces the path that packets take to reach their destination, showing each hop along the way.
