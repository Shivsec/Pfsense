# pfSense Firewall Setup and Configuration 🔐

## Overview
pfSense is an open-source firewall and router platform with a rich feature set, including **Unified Threat Management (UTM)**, **load balancing**, and **multi-WAN** support. In this project, I demonstrate a step-by-step guide on installing and configuring pfSense to protect and manage a network securely.

## Key Features
- **Firewall Configuration**: Setting up basic firewall rules.
- **Multi-WAN Failover & Load Balancing**: Configuring multiple WAN interfaces for redundancy.
- **DMZ Setup**: Isolating public-facing services from the internal network.
- **pfBlocker-NG**: IP/DNS-based filtering for enhanced network protection.
- **SNORT Integration**: Intrusion detection and prevention system (IDS/IPS).

## Installation and Setup

### 1. Prepare Installation Media
- Download pfSense [here](https://www.pfsense.org/download/) and create a bootable USB with Rufus or Etcher.
- Boot the device using the installation media.

### 2. Install pfSense on Bare Metal
1. Select language and keymap settings.
2. Choose the partition scheme (UFS/ZFS).
3. Follow the prompts to install and reboot.

### 3. Initial Network Configuration
- Access the pfSense web interface via `https://192.168.1.1`.
- Change the default LAN IP (e.g., `172.16.80.1`) and configure the **DHCP range**.

### 4. Configuring Multi-WAN and Load Balancing
- Assign WAN interfaces (`Interfaces > Assignments`) and set up **firewall rules** for traffic control.
- Create **Gateway Groups** for WAN failover and load balancing in `System > Routing`.

### 5. DMZ Configuration
- Isolate public servers using a separate DMZ network.
- Set up firewall rules to restrict inbound traffic.

### 6. pfBlocker-NG and SNORT Setup
- Install pfBlocker-NG and configure **GeoIP blocking** and custom lists.
- Set up Snort for **intrusion detection** and real-time protection.

## Conclusion
This project demonstrates the setup and configuration of a pfSense firewall to secure a network, with additional features like **multi-WAN**, **DMZ**, **pfBlocker-NG**, and **IDS/IPS** integration. This project enhances security, improves network management, and showcases real-world networking skills.
