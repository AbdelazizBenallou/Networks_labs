# 📡 Network Labs – Practical Networking with Cisco Packet Tracer

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Cisco Packet Tracer](https://img.shields.io/badge/Cisco-Packet%20Tracer-orange.svg)](https://www.netacad.com/courses/packet-tracer)
[![Level](https://img.shields.io/badge/Level-CCNA%20200--301-blue.svg)](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/associate/ccna.html)

## 📖 Overview

**Network Labs** is a comprehensive, hands-on networking collection designed to bridge the gap between theoretical concepts and practical implementation. Built for **CCNA (200-301) candidates**, networking students, and junior engineers, this repository provides real-world scenarios using **Cisco Packet Tracer**.

Each lab is structured to simulate enterprise environments, focusing on configuration, troubleshooting, and verification. As the philosophy of this project states:

> **"Networking is not learned by reading alone — it is learned by configuring, breaking, and fixing."**

---

## 🎯 Learning Objectives

By completing these labs, you will master:
*   **Design & Configuration:** Multi-VLAN networks, Layer 2 & Layer 3 switching.
*   **IP Services:** DHCP (Server & Router-based), NAT (Static, Dynamic, PAT), SSH.
*   **Wireless Networking:** WLC configuration, 802.1X authentication, Multi-VLAN WLAN.
*   **Troubleshooting:** Connectivity verification, ping tests, and service validation.

---

## 🗂 Repository Structure

```text
Networks_labs.git/
├── Networks_labs-main/
│   ├── Books/                  # Recommended CCNA Study Materials
│   ├── IP Services/            # NAT & SSH Labs
│   │   ├── NAT/
│   │   │   ├── NAT(PAT)/
│   │   │   ├── NAT(static PAT)/
│   │   │   └── NAT(Static)/
│   │   └── SSH/
│   ├── switching/              # VLAN & VTP Labs
│   │   ├── vlan_labs/
│   │   │   ├── lab_1/          # Layer 3 Switching & SVI
│   │   │   ├── lab_2/          # DHCP Server & SSH
│   │   │   └── lab_3/          # Router on Stick
│   │   └── vtp_labs/
│   └── wireless/               # Wireless LAN Controller & Security
│       ├── small_project_conf/
│       └── Tps_wireless_exp/
├── LICENSE
└── README.md
```

---

## 🧪 Lab Scenarios & Requirements

### 🔀 Switching Labs

#### **Lab 1: Layer 3 Switching & Inter-VLAN Routing**
*   **Device:** Cisco 3650 Layer 3 Switch.
*   **Core Task:** Configure SVI (Switch Virtual Interface) for Inter-VLAN routing.
*   **Addressing Scheme:**
    *   `VLAN 1`: 10.1.1.254/24
    *   `VLAN 10`: 10.1.10.254/24
    *   `VLAN 20`: 10.1.20.254/24
    *   `VLAN 30`: 10.1.30.254/24
    *   `VLAN 100`: 10.1.100.254/24
*   **Management IPs:**
    *   Switch 1: `10.1.1.1/24` | Switch 2: `10.1.1.2/24` | Switch 3: `10.1.1.3/24`
*   **Endpoints:**
    *   PC1 (VLAN 10): `10.1.10.10/24`
    *   PC2 (VLAN 20): `10.1.20.10/24`
    *   PC3 (VLAN 30): `10.1.30.10/24`
    *   Server 1 (VLAN 100): `10.1.100.10/24`
*   **Verification:** Full connectivity ping tests between PCs and Switches. Trunking configured between switches.

#### **Lab 2: DHCP Services & Secure Management**
*   **Core Task:** Implement DHCP Server on a static IP server and secure switch management.
*   **DHCP Pools:**
    *   **VLAN 1:** Network `10.1.1.0/24`, Excluded `1-100`, Gateway `10.1.1.254`
    *   **VLAN 10:** Network `10.1.10.0/24`, Excluded `1-100`, Gateway `10.1.10.254`
    *   **VLAN 20:** Network `10.1.20.0/24`, Excluded `1-100`, Gateway `10.1.20.254`
    *   **VLAN 30:** Network `10.1.30.0/24`, Excluded `1-100`, Gateway `10.1.30.254`
*   **Security:** Configure **SSH** on the multi-layer switch for remote access.
*   **Verification:** Clients must obtain IPs automatically; SSH access verified.

#### **Lab 3: Router on a Stick**
*   **Core Task:** Inter-VLAN routing using Router Sub-interfaces.
*   **Switch Configuration:** Multi-layer switch operates strictly at **Layer 2** (No `ip routing`).
*   **Router Configuration:**
    *   Sub-interfaces created for VLAN 1, 10, and 20.
    *   DHCP Pools configured directly on the Router.
*   **Addressing:**
    *   VLAN 1: `10.1.1.254/24`
    *   VLAN 10: `10.1.10.254/24`
    *   VLAN 20: `10.1.20.254/24`
*   **Verification:** End-to-end ping success across VLANs via the router.

#### **VTP Labs**
*   **Focus:** VLAN Trunking Protocol configuration to propagate VLAN databases across switches efficiently.

---

### 🌐 IP Services Labs

#### **NAT Configurations**
*   **Static NAT:** One-to-one mapping for specific internal hosts.
*   **Dynamic NAT:** Pool-based address translation.
*   **PAT (Port Address Translation):** Overloading a single public IP for multiple internal hosts.
*   **Static PAT:** Specific port forwarding configurations.

#### **SSH Lab**
*   **Focus:** Secure remote management configuration replacing Telnet.
*   **File:** `Ssh_Config.pkt`

---

### 📶 Wireless Networking Labs

#### **Small Project Configurations**
*   **802.1X:** Authentication protocol implementation.
*   **ESA/BSA:** Enterprise vs. Basic Service Area configurations.
*   **Multi-VLAN Wireless:** Segregating wireless traffic across multiple VLANs.
*   **WLC (Wireless LAN Controller):** Centralized management of access points.

#### **Wireless Experiments (Tps_wireless_exp)**
*   **Lab 2-5:** Progressive scenarios covering WLAN basics, DHCP integration with wireless clients, and advanced WLC setups.

---

## 📘 Recommended Resources

Located in `/Books/`, the following texts are recommended to complement these labs:
1.  **CCNA 200-301 Official Cert Guide, Volume 1**
2.  **CCNA 200-301 Official Cert Guide, Volume 2**

---

## 🛠 Prerequisites

Before starting these labs, ensure you have:
*   **Software:** Cisco Packet Tracer installed (Recommended version **8.x** or later).
*   **Knowledge:**
    *   Understanding of OSI & TCP/IP models.
    *   Proficiency in IP addressing and Subnetting.
    *   Basic Cisco IOS command line familiarity.

---

## 🚀 Getting Started

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/yourusername/Networks_labs.git
    ```
2.  **Navigate to a Lab:**
    ```bash
    cd Networks_labs-main/switching/vlan_labs/lab_1
    ```
3.  **Read Requirements:**
    Open `requirements.txt` to understand the specific objectives and IP schemes.
4.  **Open Packet Tracer:**
    Load the `.pkt` file and begin configuration.
5.  **Verify:**
    Use `ping`, `show ip interface brief`, and `show run` to validate your work.

---

## 🤝 Contributing

Contributions are welcome! You can help by:
*   Adding new lab scenarios.
*   Improving documentation or `requirements.txt` clarity.
*   Fixing errors in existing `.pkt` files.
*   Translating lab instructions into other languages.

Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the **MIT License**.

**Copyright (c) 2025 Abdelaziz Benallou**

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

### 📬 Contact & Support
For questions regarding specific lab configurations or licensing, please refer to the repository issues page or contact the author.

**Happy Networking!** 🌐

## 👨‍💻 Author

**Abdelaziz Benallou**  
*Network Engineer & Security Enthusiast*

[![GitHub](https://img.shields.io/badge/GitHub-@AbdelazizBenallou-black?style=for-the-badge&logo=github)](https://github.com/AbdelazizBenallou)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](YOUR_LINKEDIN_URL)

---

<p align="center">
  <i>If you find this project helpful, please consider giving it a ⭐️ star!</i>
</p>
```
