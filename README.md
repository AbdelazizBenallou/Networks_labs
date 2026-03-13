```markdown
# 📡 Network Labs | Enterprise Networking & Security Scenarios

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![CCNA](https://img.shields.io/badge/Level-CCNA%20200--301-blue)](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/associate/ccna.html)
[![Packet Tracer](https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-orange)](https://www.netacad.com/courses/packet-tracer)
[![Status](https://img.shields.io/badge/Status-Active-green)](.)

> **Networking is not learned by reading alone — it is learned by configuring, breaking, and fixing.**  
> A hands-on collection of enterprise-grade networking labs designed to bridge the gap between theory and real-world implementation.

---

## 📑 Table of Contents

- [Overview](#overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Repository Structure](#-repository-structure)
- [Prerequisites & Installation](#-prerequisites--installation)
- [Usage](#-usage)
- [Lab Example](#-lab-example)
- [Security Focus](#-security-focus)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## 🌐 Overview

This repository is a **comprehensive networking labs collection** designed for students, CCNA candidates, and junior network engineers. Each lab simulates **real production scenarios** using **Cisco Packet Tracer**, focusing on core enterprise technologies such as VLANs, Inter-VLAN Routing, DHCP, NAT, SSH, and Wireless LAN configurations.

Unlike theoretical guides, this project emphasizes **practical configuration, troubleshooting, and security hardening**.

---

## 🚀 Features

- **🏗 Real-World Topologies:** Simulations based on enterprise network designs.
- **🔒 Security Hardening:** Labs include SSH configuration, 802.1X authentication, and NAT security.
- **📄 Detailed Requirements:** Each lab comes with a `requirements.txt` outlining specific IP schemes and configuration goals.
- **🔄 Automated Verification:** Steps included to verify connectivity (Ping, Traceroute, DHCP leases).
- **📚 Learning Resources:** Includes references to official CCNA cert guides.

---

## 🛠 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Simulation** | Cisco Packet Tracer (v8.x+) |
| **Networking** | VLANs, VTP, STP, EtherChannel |
| **Routing** | Inter-VLAN Routing, Static Routing, DHCP |
| **Services** | NAT (Static/Dynamic/PAT), SSH, DNS |
| **Wireless** | WLC, 802.1X, WLAN Security |
| **Security** | Access Control, Secure Management |

---

## 🗂 Repository Structure

```text
Networks_labs/
├── Books/                  # Recommended CCNA Study Guides
├── IP Services/            # NAT, PAT, SSH Configurations
│   ├── NAT/
│   └── SSH/
├── switching/              # VLANs, VTP, Layer 3 Switching
│   ├── vlan_labs/
│   └── vtp_labs/
├── wireless/               # WLC, 802.1X, WLAN Security
│   ├── small_project_conf/
│   └── Tps_wireless_exp/
├── LICENSE
└── README.md
```

---

## 📥 Prerequisites & Installation

### Prerequisites
Before downloading the labs, ensure you have:
1.  **Cisco Packet Tracer** installed (Recommended version **8.x or later**).
2.  Basic understanding of **OSI & TCP/IP models**.
3.  Knowledge of **IP addressing and Subnetting**.

### Installation
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AbdelazizBenallou/Networks_labs.git
    ```
2.  **Navigate to a lab folder:**
    ```bash
    cd Networks_labs/switching/vlan_labs/lab_1
    ```
3.  **Open the `.pkt` file** in Cisco Packet Tracer.

---

## 🎯 Usage

1.  **Read the Requirements:** Open the `requirements.txt` file in the lab folder to understand the IP addressing scheme and configuration goals.
2.  **Configure Devices:** Access the CLI of routers and switches to implement the required services (VLANs, DHCP, NAT, etc.).
3.  **Verify Connectivity:** Use PC command prompts to ping across VLANs or test internet access.
4.  **Troubleshoot:** If connectivity fails, use `show` commands to diagnose interface status, routing tables, or ACLs.

---

## 🛡 Security Focus

As part of modern network engineering, security is integrated into several labs:
- **SSH Configuration:** Replacing insecure Telnet with encrypted remote management.
- **802.1X Authentication:** Implementing port-based network access control in wireless labs.
- **NAT/PAT:** Configuring network address translation to hide internal IP structures.

---

## 🤝 Contributing

Contributions are welcome! You can help by:
- ➕ Adding new labs (Routing, Security, Automation).
- 🐛 Fixing errors in existing `.pkt` files.
- 📝 Improving documentation or translating lab instructions.
- 🔒 Suggesting security hardening improvements.

Feel free to **fork** the repository and submit a **pull request**.

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```text
Copyright (c) 2025 Abdelaziz Benallou
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

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
