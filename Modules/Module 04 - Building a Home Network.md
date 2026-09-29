# Module 4: Building a Home Network
**Date:** 2026-06-04 | **Status:** 🟢 Completed

## 🎯 Core Objective
Understand how residential network hardware separates public and private data traffic, uses wireless frequencies, and is securely configured for the first time.

---

## 🔑 Key Concepts & Pillars

### 🏠 1. Home Network Architecture
* Typical home setups deal with **two separate networks**:
	1. **Public Network:** The incoming data stream from an ISP (Internet Service Provider).
	2. **Private LAN:** Your internal home network (PCs, Smart TVs, Phones).
* [Modem](../Concepts/Modem.md): Converts incoming provider signals (like Coaxial cable or DSL) into standard Ethernet data that your local home devices can read.
* [Wireless Router (Integrated)](../Concepts/Wireless%20Router%20(Integrated).md): A multi-functional hardware box that combines three separate networking devices into one unit:
	1. **A Router:** Separates the local LAN from the external Internet.
	2. **A Switch:** Connects local wired devices together via LAN ports.
	3. **A Wireless Access Point (WAP):** Connects your wireless devices to the same local LAN using radio waves.

### 📶 2. Wireless Frequencies & Wi-Fi Standards
* Home networks use the **unlicensed** radio frequency spectrum, meaning anyone can use them without a government permit.
* **2.4 GHz Band:** Used by Bluetooth (low-speed, short-range peripheral connections) and older Wi-Fi.
* **5 GHz Band:** Used by modern Wi-Fi for higher speeds and less interference.
* IEEE 802.11: The global standard governing wireless local networks (Wi-Fi).
* **The Wi-Fi Alliance:** An organization that tests different manufacturers' devices to ensure they are fully interoperable (indicated by the Wi-Fi logo).

### ⚙️ 3. Essential Wireless Settings
* **SSID (Service Set Identifier):** The case-sensitive, 32-character name of your wireless network. 
* **SSID Broadcast:** Tells the router to announce its name to the world. Turning this off does *not* secure a network; strong encryption is always required.
* **Network Mode:** Determines which wireless technologies are allowed to connect.
	* *Single Mode:* Only allows one standard (e.g., 802.11ac). Maximizes speed but blocks older devices.
	* *Mixed Mode / Legacy Mode:* Allows older standards to connect to the same router, ensuring backwards compatibility.

---

## 🛠️ Hands-on Configuration & Setup Steps
To set up a home router for the first time:
1. Connect a PC to a **LAN Port** via an Ethernet patch cable (never the Internet port).
2. The computer will automatically grab a local IP address using a local DHCP server built into the router.
3. Open a browser, enter the router's IP gateway, and configure the basic settings.

⚠️ **Security Design Rules:** Never leave default SSIDs or passwords active, and never use the router's brand name as the network name.

---

## 🧠 Exam Highlights (Mental Anchors)
* ⚠️ **Watch out for:** The **Internet (WAN) port** is the *only* port on a home router that sits on a completely different network by default. All the LAN Ethernet ports and wireless clients share the exact same local network space.
* 💡 **Key Takeaway:** Turning off SSID broadcasting is *security through obscurity*—it hides the name from basic view but does not encrypt or protect your data packet headers.