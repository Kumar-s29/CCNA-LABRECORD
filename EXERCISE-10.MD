# EXERCISE 10:

## L2 Security and WLANs

**Author**: Kumara Swamy S

---

### 1. Introduction to Layer 2 Security and WLANs

Layer 2 (L2) security focuses on securing data transmission over the data link layer, which is crucial for preventing unauthorized access and attacks in local area networks (LANs). Wireless Local Area Networks (WLANs) are commonly used in both home and enterprise environments, but they present unique challenges in terms of security due to their nature. In this exercise, we will explore the concepts of Layer 2 security, the vulnerabilities in WLANs, and the methods to secure both wired and wireless networks.

---

### 2. Overview of Layer 2 Security

- **Data Link Layer Security**: Ensures that data transmission between devices is secure and protected against unauthorized access.
- **Key Principles**:
  - Authentication: Verifying the identity of devices or users connecting to the network.
  - Encryption: Securing data to ensure that only authorized recipients can access the transmitted information.
  - Integrity: Ensuring that data has not been tampered with during transmission.

---

### 3. Layer 2 Attacks

- **MAC Address Spoofing**: Attacker impersonates a legitimate device by changing their MAC address to a valid one, gaining unauthorized access to the network.
- **ARP Spoofing (Poisoning)**: Manipulating the ARP cache to associate the attacker's MAC address with an IP address on the network, allowing for interception of data.
- **VLAN Hopping**: Exploiting VLAN configurations to send packets between VLANs without authorization, which can compromise network security.
- **Flooding Attacks**: Overloading the network by sending a high volume of traffic, causing congestion or failure of network devices.

---

### 4. WLAN Security Challenges

- **Wireless Nature of WLANs**: Wireless networks can be accessed from a distance, making them more susceptible to eavesdropping, unauthorized access, and interference.
- **Weak Encryption Protocols**: Older encryption methods like WEP (Wired Equivalent Privacy) are vulnerable to attacks, making modern encryption crucial.
- **SSID Broadcasting**: By default, WLANs broadcast their SSID (Service Set Identifier), making it easier for attackers to locate the network.
- **Rogue Access Points**: Unauthorized access points can be connected to a WLAN, tricking users into connecting to malicious networks.

---

### 5. Securing Layer 2 Networks

- **Port Security**: Limits the number of devices that can connect to a switch port and specifies which MAC addresses are allowed.
- **802.1X Authentication**: Implements port-based network access control using RADIUS servers to authenticate users before allowing access to the network.
- **Dynamic ARP Inspection**: Prevents ARP spoofing attacks by ensuring that ARP requests and replies are valid.
- **Private VLANs**: Isolates devices within the same VLAN from each other, enhancing security by limiting communication between devices.

---

### 6. WLAN Security Protocols

- **WEP (Wired Equivalent Privacy)**: An older encryption protocol that is now considered insecure due to vulnerabilities, including weak key management and short encryption keys.
- **WPA (Wi-Fi Protected Access)**: An improvement over WEP, offering stronger encryption and authentication mechanisms.
- **WPA2**: Uses AES (Advanced Encryption Standard) for encryption, providing stronger security for wireless networks.
- **WPA3**: The latest standard for wireless security, offering improved encryption, forward secrecy, and protection against offline dictionary attacks.
- **802.1X with EAP**: Provides robust authentication in WLANs using Extensible Authentication Protocol (EAP), typically backed by a RADIUS server.

---

### 7. Securing WLANs

- **Disable SSID Broadcast**: Prevents the network from being visible to unauthorized users.
- **Use Strong Encryption**: Always use WPA2 or WPA3 with AES encryption to ensure data privacy.
- **Enable MAC Filtering**: Allows only authorized devices to connect to the network by filtering based on their MAC address.
- **Secure the Router/Access Point**: Change default usernames and passwords, disable remote management, and update firmware regularly to patch vulnerabilities.
- **Guest Networks**: Implementing isolated guest networks for visitors to limit access to critical internal resources.

---

### 8. Authentication in WLANs

- **Pre-Shared Key (PSK)**: A simple method where a shared password or key is used to authenticate devices to the WLAN. Best for small, private networks.
- **Enterprise Authentication**: Involves using an authentication server (e.g., RADIUS) to validate users' credentials before granting access to the network, offering higher security for business environments.
- **EAP Methods**: Various Extensible Authentication Protocol (EAP) methods, such as EAP-TLS, EAP-TTLS, and PEAP, provide different levels of security depending on the use case and environment.

---

### 9. Best Practices for WLAN Security

- **Regularly Update Firmware**: Keep access points and routers updated to protect against newly discovered vulnerabilities.
- **Strong Password Policies**: Use long, complex passwords for network authentication and WPA2 or WPA3 encryption keys.
- **Monitor WLAN Traffic**: Use intrusion detection and prevention systems (IDPS) to detect unusual activity or unauthorized devices attempting to connect.
- **Limit Signal Range**: Reduce the range of the wireless network to prevent unauthorized access from outside the intended coverage area.

---

### 10. Troubleshooting WLAN Security

- **Verify Authentication Settings**: Ensure that the correct security protocols (e.g., WPA2 or WPA3) and encryption methods are being used.
- **Check for Interference**: WLAN performance can be affected by interference from other wireless devices; use tools like spectrum analyzers to check for conflicts.
- **Inspect Access Points**: Ensure that access points are correctly configured and that rogue access points are not present on the network.
- **Review Logs**: Regularly check logs on access points, switches, and security devices to identify potential security breaches or unusual activities.

---

### 11. Practical Applications

In today’s connected world, securing Layer 2 networks and WLANs is essential for protecting sensitive data and ensuring reliable access. The methods learned in this exercise, such as implementing security protocols like WPA2 and using 802.1X authentication, are critical for maintaining secure and robust networks in both home and enterprise environments. Effective WLAN security strategies help prevent unauthorized access, eavesdropping, and attacks, ensuring that users can safely access network resources.
