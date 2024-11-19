# **Exercise 4: IP Addressing**

**Author**: Kumara Swamy S

### **1. Introduction to IP Addressing**

- **IP Address**: An identifier assigned to each device connected to a network. It is used for identifying devices and routing data between them.
- **Types of IP Addresses**:
  - **IPv4**: A 32-bit address written in four octets (e.g., 192.168.1.1).
  - **IPv6**: A 128-bit address written in hexadecimal format, used to address the limitations of IPv4.

---

### **2. Structure of an IPv4 Address**

- **Format**: IPv4 addresses are written in **dotted decimal** notation, consisting of four octets (each ranging from 0 to 255).
  - Example: 192.168.1.1
- **Subnet Mask**: A 32-bit address used to divide the IP address into the **network** and **host** portions.
  - Example: 255.255.255.0
- **Network Address**: The part of the IP address that identifies the network.
- **Host Address**: The part of the IP address that identifies a specific device on the network.

---

### **3. Subnetting**

- **Subnetting**: Dividing a larger network into smaller, more manageable sub-networks (subnets).
- **Purpose**:
  - Efficient use of IP addresses.
  - Enhanced security and organization.
- **Subnet Mask Calculation**:
  - Subnet masks define which portion of the IP address is used for the network and which is used for hosts.
  - For example, the subnet mask **255.255.255.0** means that the first three octets (192.168.1) represent the network, and the last octet (0) is used for host addresses.
- **Example**: If a network uses the IP range **192.168.1.0/24**, the **/24** indicates that the first 24 bits are used for the network, and the remaining bits can be used for hosts.

---

### **4. IP Address Classes**

- **Class A** (1.0.0.0 to 127.255.255.255): Supports a large number of hosts.
- **Class B** (128.0.0.0 to 191.255.255.255): Suitable for medium-sized networks.
- **Class C** (192.0.0.0 to 223.255.255.255): Typically used for smaller networks.
- **Class D** (224.0.0.0 to 239.255.255.255): Used for multicast addresses.
- **Class E** (240.0.0.0 to 255.255.255.255): Reserved for experimental use.

---

### **5. Private and Public IP Addresses**

- **Private IP Addresses**: Used within private networks and not routable on the internet.
  - Example ranges:
    - Class A: 10.0.0.0 – 10.255.255.255
    - Class B: 172.16.0.0 – 172.31.255.255
    - Class C: 192.168.0.0 – 192.168.255.255
- **Public IP Addresses**: Assigned by the ISP and can be routed on the internet.

---

### **6. NAT (Network Address Translation)**

- **NAT**: A method used to map private IP addresses to a single public IP address. It is commonly used in home and office networks to allow multiple devices to access the internet using a single public IP address.
- **Types of NAT**:
  - **Static NAT**: Maps one private IP address to one public IP address.
  - **Dynamic NAT**: Maps a range of private IP addresses to a pool of public IP addresses.
  - **PAT (Port Address Translation)**: A type of dynamic NAT that maps multiple private IP addresses to a single public IP address using different port numbers.

---

### **7. IPv6 Addressing**

- **IPv6**: Uses a 128-bit address, written in eight groups of four hexadecimal digits.
  - Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- **Advantages over IPv4**:
  - Larger address space.
  - Built-in security (IPsec).
  - No need for NAT due to the vast number of available addresses.

---

### **8. IP Address Allocation Methods**

- **Static IP Addressing**:
  - A fixed IP address manually assigned to a device.
  - Ideal for servers, printers, and other devices that require a consistent IP address.
- **Dynamic IP Addressing (DHCP)**:
  - IP addresses are automatically assigned by a **DHCP server**.
  - Used for devices that do not require a permanent IP address (e.g., laptops, smartphones).

---

### **9. Practical Applications of IP Addressing**

- **Assigning IP Addresses**: Proper allocation and subnetting of IP addresses ensure efficient use of the address space and avoid conflicts.
- **Network Security**: Understanding IP addressing helps in setting up firewalls, routers, and access control lists (ACLs) for securing the network.
- **Troubleshooting**: Knowing how to manage IP addresses assists in diagnosing network connectivity issues.

---
