# Module 07: Ethernet & Switching
**Date:** 2026-06-20 | **Status:** 🟢 Completed

## 🎯 Core Objective
Understand how Ethernet frames are structured and how switches forward data within a LAN.

---

## 📦 Ethernet Frame

| Field | Size | Purpose |
|-------|------|---------|
| Preamble | 7 bytes | Synchronizes devices before communication. |
| Start Frame Delimiter (SFD) | 1 byte | Marks the beginning of the frame. |
| Destination MAC | 6 bytes | MAC address of the receiving device. |
| Source MAC | 6 bytes | MAC address of the sending device. |
| Type/Length | 2 bytes | Identifies the protocol or payload length. |
| Data | 46–1500 bytes | Actual payload being transmitted. |
| Frame Check Sequence (FCS) | 4 bytes | Detects transmission errors using CRC. |

---

## 🔀 Ethernet Switches

- Operate at **Layer 2 (Data Link Layer)**.
- Connect devices within the same LAN.
- Forward frames using **MAC addresses**.
- Each switch port is its own collision domain.

---

## 📋 MAC Address Table

Switches build their MAC address table by examining the **source MAC address** of every incoming frame.

When a frame arrives:

1. The switch learns the source MAC and records the incoming port.
2. If the destination MAC exists in the table, the frame is forwarded only to that port.
3. If the destination MAC is unknown, the switch performs an **unknown unicast flood**, sending the frame to every port except the one it arrived on.

---

## 📢 ARP (Address Resolution Protocol)

If a device knows the destination **IP address** but not its **MAC address**:

1. It sends an **ARP Request** (broadcast).
2. The device with the matching IP responds with an **ARP Reply** (unicast).
3. Future communication uses the discovered MAC address.

---

## 🧠 Exam Highlights

⚠️ **Watch out for**
- Switches forward frames using **MAC addresses**, not IP addresses.
- Switches operate at **OSI Layer 2**.
- ARP maps an **IP address → MAC address**.

💡 **Key Takeaways**
- Ethernet frames carry data across a LAN.
- Switches learn MAC addresses automatically.
- Unknown destination MACs are flooded.
- ARP is used only when the destination MAC is unknown.