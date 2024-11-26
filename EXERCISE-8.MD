# EXERCISE 8:

## Redundant Networks

**Author**: Kumara Swamy S

---

### 1. Introduction to Redundant Networks

Redundant networks are designed to provide high availability and fault tolerance by incorporating multiple paths for data transmission. These networks ensure that if one path fails, another path takes over without disrupting the communication. Redundancy is crucial for minimizing downtime and ensuring continuous network services.

---

### 2. Importance of Redundancy

- **High Availability**: Ensures continuous network connectivity by providing alternate paths for data.
- **Fault Tolerance**: Allows networks to remain operational even when one or more components fail.
- **Load Balancing**: Distributes traffic across multiple paths, improving network performance and efficiency.
- **Minimized Downtime**: Redundant systems allow network services to stay online even during maintenance or failures.

---

### 3. Redundant Network Topologies

- **Mesh Topology**:
  - Each device is connected to every other device, providing multiple paths.
  - Offers the highest level of redundancy but can be expensive to implement.
- **Star Topology with Redundant Links**:
  - Central devices (e.g., switches or routers) are connected to multiple devices.
  - Redundant links between the central device and other devices ensure no single point of failure.
- **Ring Topology with Redundant Links**:
  - Devices are connected in a closed loop with redundant paths.
  - Provides redundancy without the complexity of a mesh topology.

---

### 4. Redundancy Protocols

- **Spanning Tree Protocol (STP)**:
  - Prevents loops in the network by blocking redundant paths and ensuring only one active path between devices.
  - STP dynamically adjusts to network changes, allowing for path recovery if a failure occurs.
  - Variants include RSTP (Rapid Spanning Tree Protocol) and MSTP (Multiple Spanning Tree Protocol) for faster convergence.
- **Hot Standby Router Protocol (HSRP)**:
  - Allows multiple routers to work together, providing a virtual router for higher availability.
  - If the active router fails, the standby router takes over.
- **Virtual Router Redundancy Protocol (VRRP)**:
  - Similar to HSRP, but allows for the use of multiple routers in an active-standby configuration.
  - VRRP increases reliability and avoids single points of failure.
- **Gateway Load Balancing Protocol (GLBP)**:
  - Distributes traffic among multiple routers to ensure load balancing and redundancy.
  - Helps in preventing bottlenecks while providing fault tolerance.

---

### 5. Configuring Redundant Network Devices

- **Configuring STP on a Switch**:

```

Switch(config)# spanning-tree mode rapid-pvst
 Switch(config)# spanning-tree vlan <VLAN-ID> root primary

```

- **Configuring HSRP on Routers**:

```

Router(config)# interface <interface-name>
 Router(config-if)# standby <group-number> ip <virtual-ip-address>
 Router(config-if)# standby <group-number> priority <priority-value>

```

- **Configuring VRRP on Routers**:

```

Router(config)# interface <interface-name>
 Router(config-if)# vrrp <group-number> ip <virtual-ip-address>
 Router(config-if)# vrrp <group-number> priority <priority-value>

```

---

### 6. Troubleshooting Redundant Networks

- **Common Issues**:
- Misconfiguration of STP or HSRP/VRRP settings.
- Incorrect VLAN assignments causing network traffic disruptions.
- Redundant path loops due to incorrect spanning-tree settings.
- **Troubleshooting Tools**:
- `show spanning-tree`: Verifies STP status and port roles.
- `show standby`: Checks HSRP status and virtual IP configuration.
- `show vrrp`: Displays VRRP status and active router information.

---

### 7. Practical Applications

Redundant networks are essential in data centers, enterprise networks, and critical infrastructure. They ensure that network services remain operational despite component failures, providing businesses with the reliability they need to operate smoothly. Proper configuration and maintenance of redundant links and protocols contribute to higher performance, enhanced fault tolerance, and minimized downtime.

```

```
