# Exercise 6: Building and Securing a Small Network

**Author: Kumara Swamy S**

---

## 1. Introduction to Building a Small Network

- **Small Network**: A network that connects a limited number of devices, typically within a single location, such as a home or small office. It can be as simple as connecting a few computers or devices in a local environment.
- **Objective**: To design and implement a small network with secure communication between devices, ensuring reliable access to shared resources and the internet. This network should be robust enough to support necessary tasks while being secure from external threats.

---

## 2. Key Components of a Small Network

- **Router**: The central device that connects the local network to the internet and routes traffic between devices. It manages both external and internal network traffic efficiently.
- **Switch**: A device that connects multiple devices within the network, allowing them to communicate directly with each other. It helps in improving network performance by reducing traffic.
- **Devices**: Computers, printers, smartphones, etc., that are connected to the network for communication and resource sharing. These devices can interact with the network for various tasks such as file sharing or printing.
- **Firewall**: A security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It protects the network from unauthorized access and attacks.

---

## 3. Steps to Build a Small Network

- **Step 1: Planning the Network**
  - Decide the number of devices to connect. Plan out the devices that will be part of the network, considering whether you need wired or wireless connections.
  - Choose the appropriate IP addressing scheme (e.g., using **private IP ranges** like 192.168.x.x). This helps in organizing the network and ensures efficient management of device connections.
- **Step 2: Configuring the Router**
  - Set up the router for internet connectivity. Make sure the router is configured to provide an internet connection to all devices in the network.
  - Configure **DHCP** on the router to automatically assign IP addresses to devices. DHCP ensures that IP addresses are assigned dynamically without the need for manual configuration.
- **Step 3: Setting up the Switch**
  - Connect multiple devices to the switch for internal communication. A switch helps to establish a connection between multiple devices within the local network.
  - Ensure proper configuration of VLANs (if applicable) for segmentation of network traffic. VLANs allow you to separate network traffic logically, improving performance and security.
- **Step 4: Connecting Devices**
  - Physically connect the devices (PCs, printers, etc.) to the network using **Ethernet cables** or **Wi-Fi**. Ensure a stable and secure connection for each device to work properly within the network.
  - Ensure that each device gets an IP address (either statically or via DHCP). A stable IP assignment ensures devices can communicate without interruptions.

---

## 4. Securing the Small Network

- **Step 1: Change Default Credentials**
  - Change the default username and password on the router and switch to prevent unauthorized access. Default credentials are easy targets for attackers, so it's essential to update them immediately.
- **Step 2: Set Up a Firewall**

  - Enable the firewall on the router to block any unauthorized external access. A firewall is critical in preventing outside attacks.
  - Implement rules for allowing only trusted inbound and outbound traffic. This will help in controlling the traffic flow and prevent unauthorized connections.

- **Step 3: Use WPA2 or WPA3 for Wi-Fi Security**

  - Set up strong Wi-Fi encryption (WPA2 or WPA3) to protect wireless communications. This encryption ensures that your network's data transmission is secure.
  - Use a complex password to prevent unauthorized access to the Wi-Fi network. A strong password adds an additional layer of security to prevent easy access.

- **Step 4: Implementing VLANs (Virtual LANs)**

  - If needed, create separate VLANs for different types of traffic (e.g., guest network, internal network). VLANs help in segregating traffic, which improves security and reduces the risk of internal breaches.
  - This limits the broadcast domain and improves security by isolating devices. For example, the guest network should not have access to the internal network.

- **Step 5: Update Firmware Regularly**
  - Regularly update the router, switch, and device firmware to fix vulnerabilities and enhance security. This is essential for ensuring that the network devices stay protected against new threats.
- **Step 6: Disable Unused Ports**
  - Disable unused ports on the switch and router to minimize attack surfaces. Unused ports can be exploited by attackers to gain unauthorized access to the network.

---

## 5. Testing the Network

- **Ping Test**: Use the **ping** command to test connectivity between devices on the network. This ensures that the devices can communicate and there are no connectivity issues.
- **Speed Test**: Perform an internet speed test to ensure that the router is providing adequate bandwidth. It helps in determining whether the network is delivering the expected performance.
- **Security Testing**: Use network security tools like **Wireshark** or **Nmap** to identify potential vulnerabilities in the network. Regular security assessments ensure that your network remains secure over time.

---

## 6. Troubleshooting Common Network Issues

- **Device Not Connecting**: Check physical connections, ensure devices are on the same IP range, and troubleshoot DHCP settings. Network misconfigurations often cause devices to fail to connect.
- **Slow Internet**: Check for bandwidth usage, possible interference in the Wi-Fi signal, or network congestion. Identifying the root cause will help in optimizing the network performance.
- **Firewall Blocking**: Ensure that the firewall is not incorrectly blocking legitimate traffic by reviewing firewall rules. Misconfigured firewalls can unintentionally block critical traffic.
