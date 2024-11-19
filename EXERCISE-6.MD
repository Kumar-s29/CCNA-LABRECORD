# Exercise 6: Building and Securing a Small Network

**Author**: Kumara Swamy S

---

## 1. Introduction to Building a Small Network

- **Small Network**: A network that connects a limited number of devices, typically within a single location, such as a home or small office.
- **Objective**: To design and implement a small network with secure communication between devices, ensuring reliable access to shared resources and the internet.

---

## 2. Key Components of a Small Network

- **Router**: The central device that connects the local network to the internet and routes traffic between devices.
- **Switch**: A device that connects multiple devices within the network, allowing them to communicate directly with each other.
- **Devices**: Computers, printers, smartphones, etc., that are connected to the network for communication and resource sharing.
- **Firewall**: A security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules.

---

## 3. Steps to Build a Small Network

- **Step 1: Planning the Network**
  - Decide the number of devices to connect.
  - Choose the appropriate IP addressing scheme (e.g., using **private IP ranges** like 192.168.x.x).
- **Step 2: Configuring the Router**
  - Set up the router for internet connectivity.
  - Configure **DHCP** on the router to automatically assign IP addresses to devices.
- **Step 3: Setting up the Switch**
  - Connect multiple devices to the switch for internal communication.
  - Ensure proper configuration of VLANs (if applicable) for segmentation of network traffic.
- **Step 4: Connecting Devices**
  - Physically connect the devices (PCs, printers, etc.) to the network using **Ethernet cables** or **Wi-Fi**.
  - Ensure that each device gets an IP address (either statically or via DHCP).

---

## 4. Securing the Small Network

- **Step 1: Change Default Credentials**
  - Change the default username and password on the router and switch to prevent unauthorized access.
- **Step 2: Set Up a Firewall**

  - Enable the firewall on the router to block any unauthorized external access.
  - Implement rules for allowing only trusted inbound and outbound traffic.

- **Step 3: Use WPA2 or WPA3 for Wi-Fi Security**

  - Set up strong Wi-Fi encryption (WPA2 or WPA3) to protect wireless communications.
  - Use a complex password to prevent unauthorized access to the Wi-Fi network.

- **Step 4: Implementing VLANs (Virtual LANs)**

  - If needed, create separate VLANs for different types of traffic (e.g., guest network, internal network).
  - This limits the broadcast domain and improves security by isolating devices.

- **Step 5: Update Firmware Regularly**

  - Regularly update the router, switch, and device firmware to fix vulnerabilities and enhance security.

- **Step 6: Disable Unused Ports**
  - Disable unused ports on the switch and router to minimize attack surfaces.

---

## 5. Testing the Network

- **Ping Test**: Use the **ping** command to test connectivity between devices on the network.
- **Speed Test**: Perform an internet speed test to ensure that the router is providing adequate bandwidth.
- **Security Testing**: Use network security tools like **Wireshark** or **Nmap** to identify potential vulnerabilities in the network.

---

## 6. Troubleshooting Common Network Issues

- **Device Not Connecting**: Check physical connections, ensure devices are on the same IP range, and troubleshoot DHCP settings.
- **Slow Internet**: Check for bandwidth usage, possible interference in the Wi-Fi signal, or network congestion.
- **Firewall Blocking**: Ensure that the firewall is not incorrectly blocking legitimate traffic by reviewing firewall rules.
