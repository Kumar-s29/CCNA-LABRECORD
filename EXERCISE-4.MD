# **Exercise 4: IP Addressing**

**Author**: Kumara Swamy S

### **1. Introduction to IP Addressing**

- **IP Address**: An identifier assigned to each device connected to a network. It is used for identifying devices and routing data between them. Each device on a network must have a unique IP address to communicate properly.
- **Types of IP Addresses**:
  - **IPv4**: A 32-bit address written in four octets (e.g., 192.168.1.1). It is the most widely used IP format today.
  - **IPv6**: A 128-bit address written in hexadecimal format, used to address the limitations of IPv4, such as address space exhaustion.

---

### **2. Structure of an IPv4 Address**

- **Format**: IPv4 addresses are written in **dotted decimal** notation, consisting of four octets (each ranging from 0 to 255). This format makes it easy to represent and manage.
  - Example: 192.168.1.1
- **Subnet Mask**: A 32-bit address used to divide the IP address into the **network** and **host** portions. This is essential for routing and identifying specific networks.
  - Example: 255.255.255.0
- **Network Address**: The part of the IP address that identifies the network. It is used by routers to send data to the correct network.
- **Host Address**: The part of the IP address that identifies a specific device on the network, such as a computer or printer.

---

### **3. Subnetting**

- **Subnetting**: Dividing a larger network into smaller, more manageable sub-networks (subnets). This helps optimize network performance and security.
- **Purpose**:
  - Efficient use of IP addresses by breaking large networks into smaller subnets.
  - Enhanced security and organization by isolating different segments of the network.
- **Subnet Mask Calculation**:
  - Subnet masks define which portion of the IP address is used for the network and which is used for hosts.
  - For example, the subnet mask **255.255.255.0** means that the first three octets (192.168.1) represent the network, and the last octet (0) is used for host addresses.
- **Example**: If a network uses the IP range **192.168.1.0/24**, the **/24** indicates that the first 24 bits are used for the network, and the remaining bits can be used for hosts.

---

### **4. IP Address Classes**

- **Class A** (1.0.0.0 to 127.255.255.255): Supports a large number of hosts, typically used for very large networks such as those operated by ISPs.
- **Class B** (128.0.0.0 to 191.255.255.255): Suitable for medium-sized networks, such as those used by businesses or educational institutions.
- **Class C** (192.0.0.0 to 223.255.255.255): Typically used for smaller networks, including home and small office networks.
- **Class D** (224.0.0.0 to 239.255.255.255): Used for multicast addresses, where data is sent to multiple receivers simultaneously.
- **Class E** (240.0.0.0 to 255.255.255.255): Reserved for experimental use and future applications.

---

### **5. Private and Public IP Addresses**

- **Private IP Addresses**: Used within private networks and not routable on the internet. These addresses are used to prevent the exhaustion of public IP addresses.
  - Example ranges:
    - Class A: 10.0.0.0 – 10.255.255.255
    - Class B: 172.16.0.0 – 172.31.255.255
    - Class C: 192.168.0.0 – 192.168.255.255
- **Public IP Addresses**: Assigned by the ISP and can be routed on the internet. These addresses allow devices to be accessible from anywhere on the internet.

---

### **6. NAT (Network Address Translation)**

- **NAT**: A method used to map private IP addresses to a single public IP address. This allows multiple devices to share one public IP, conserving IP addresses and improving security.
- **Types of NAT**:
  - **Static NAT**: Maps one private IP address to one public IP address. This is typically used when a specific device must be accessible from outside the network.
  - **Dynamic NAT**: Maps a range of private IP addresses to a pool of public IP addresses. This is used when there are more private addresses than public addresses.
  - **PAT (Port Address Translation)**: A type of dynamic NAT that maps multiple private IP addresses to a single public IP address using different port numbers. This is often used in home and office networks.

---

### **7. IPv6 Addressing**

- **IPv6**: Uses a 128-bit address, written in eight groups of four hexadecimal digits, allowing a virtually unlimited number of unique addresses.
  - Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
- **Advantages over IPv4**:
  - Larger address space, which solves the problem of address exhaustion.
  - Built-in security features, such as IPsec, that help protect data during transmission.
  - No need for NAT due to the vast number of available addresses, simplifying network management.

---

### **8. IP Address Allocation Methods**

- **Static IP Addressing**:
  - A fixed IP address manually assigned to a device. Ideal for devices that need a consistent IP, such as servers, routers, and printers.
- **Dynamic IP Addressing (DHCP)**:
  - IP addresses are automatically assigned by a **DHCP server**. This method is typically used for devices that do not require a permanent IP address, such as laptops and smartphones.

---

### **9. Practical Applications of IP Addressing**

- **Assigning IP Addresses**: Proper allocation and subnetting of IP addresses ensure efficient use of the address space and avoid conflicts, improving network performance.
- **Network Security**: Understanding IP addressing helps in setting up firewalls, routers, and access control lists (ACLs) for securing the network. It is crucial for preventing unauthorized access.
- **Troubleshooting**: Knowing how to manage IP addresses assists in diagnosing network connectivity issues, such as misconfigured subnets or incorrect IP assignments.
