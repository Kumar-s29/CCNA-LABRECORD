# EXERCISE 7:

## Switching Concepts, VLANs, and InterVLAN Routing

**Author**: Kumara Swamy S

---

### 1. Introduction to Switching Concepts

Switches are integral to modern networks, enabling efficient communication within a Local Area Network (LAN). They use MAC addresses to forward frames between devices and support segmentation for enhanced performance and security. Virtual Local Area Networks (VLANs) extend this segmentation by logically grouping devices, even if they are connected to different switches.

InterVLAN Routing facilitates communication between VLANs by using Layer 3 functionality or external routers.

---

### 2. Features of Switches

- **Layer 2 Functionality**: Operates at the Data Link Layer, forwarding frames based on MAC addresses.
- **MAC Address Table**: Maintains a record of connected devices and their MAC addresses for efficient frame forwarding.
- **Collision Domains**: Each port represents its own collision domain, reducing traffic collisions.
- **Full-Duplex Communication**: Ensures simultaneous data transmission and reception, improving throughput.

---

### 3. Understanding VLANs

- **Definition**: VLANs are logical groups of devices within the same physical network.
- **Advantages**:
  - Enhances security by isolating sensitive data.
  - Reduces broadcast domains, minimizing network congestion.
  - Facilitates efficient network management and scalability.
- **Types of VLANs**:
  - **Data VLAN**: Segregates user-generated data traffic.
  - **Voice VLAN**: Prioritizes VoIP traffic for better quality.
  - **Default VLAN**: The pre-configured VLAN on switches, typically VLAN 1.

---

### 4. VLAN Configuration Commands

- **Creating a VLAN**:

```

Switch(config)# vlan <VLAN-ID>
 Switch(config-vlan)# name <VLAN-Name>

```

- **Assigning Ports to VLANs**:

```

Switch(config)# interface <interface-id>
 Switch(config-if)# switchport mode access
 Switch(config-if)# switchport access vlan <VLAN-ID>

```

- **Verifying VLAN Configuration**:

```

Switch# show vlan brief

```

---

### 5. InterVLAN Routing

InterVLAN routing allows communication between devices in different VLANs. There are two main methods:

- **Router-on-a-Stick**:
- A single router interface is used to handle multiple VLANs.
- Subinterfaces are created for each VLAN.
- Example Configuration:

  ```
  Router(config)# interface <interface-id>.<subinterface-number>
  Router(config-subif)# encapsulation dot1Q <VLAN-ID>
  Router(config-subif)# ip address <IP-address> <subnet-mask>
  ```

- **Layer 3 Switch**:
- Uses switched virtual interfaces (SVIs) for routing.
- Example Commands:
  ```
  Switch(config)# interface vlan <VLAN-ID>
  Switch(config-if)# ip address <IP-address> <subnet-mask>
  Switch(config-if)# no shutdown
  ```

---

### 6. Troubleshooting VLANs and InterVLAN Routing

- **Common Issues**:
- Misconfigured VLANs or subinterfaces.
- Incorrect trunking protocols or missing VLANs in trunk links.
- Duplicate IP addresses in different VLANs.
- **Troubleshooting Tools**:
- `show vlan brief`: Verifies VLAN existence and port assignments.
- `show ip interface brief`: Confirms interface statuses and IP configurations.
- `ping`: Tests connectivity between VLANs.

---

### 7. Practical Applications

Understanding switching concepts, VLANs, and InterVLAN routing is essential for designing scalable, secure, and efficient networks. These principles are widely applied in corporate environments, data centers, and educational institutions to manage traffic effectively and enhance security.

```

```
