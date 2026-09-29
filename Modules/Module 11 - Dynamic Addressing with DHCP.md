# Module 11: Dynamic Host Configuration Protocol (DHCP)
**Date:** 2026-07-02 | **Status:** 🟢 Completed


## 🎯 Core Objective

Understand how IP addresses and network configuration information are automatically assigned to hosts on a network.

---

# 🌐 What is DHCP?

**Dynamic Host Configuration Protocol (DHCP)** is a network service that automatically provides IP configuration information to client devices.

A DHCP server can provide:

- IP address
- Subnet mask
- Default gateway
- DNS server information
- Lease duration

Without DHCP, network administrators would need to manually configure every device.

---

# 📌 Static vs Dynamic Addresses

## 🔒 Static IP Addresses

Static addresses are manually configured by a network administrator.

### Advantages:

- Provides a permanent address.
- Useful for servers, printers, and network devices.

### Disadvantages:

- Requires manual configuration.
- Time-consuming for large networks.
- Higher risk of configuration mistakes.
- More difficult to manage at scale.

---

## 🔄 Dynamic IP Addresses

Dynamic addresses are automatically assigned by a DHCP server from an available address pool.

### Advantages:

- Automatically configured.
- Reduces human error.
- Easier network management.
- Uses temporary leases.
- Better for large networks.

---

# 🔁 How DHCP Works (DORA Process)

DHCP uses a four-step process called **DORA**:
```
D - Discover  
O - Offer  
R - Request  
A - Acknowledge
```

---

## 1️⃣ DHCP Discover

The client broadcasts a DHCP Discover message asking for network configuration.

Example:

> "Is there a DHCP server available? I need an IP address." 
> Client → Broadcast → DHCP Server


---

## 2️⃣ DHCP Offer

The DHCP server responds with an available IP configuration.

The offer may include:

- IP address
- Subnet mask
- Default gateway
- DNS server

Example:

> "I can offer you 192.168.1.50 with this configuration." 
> DHCP Server → Client


---

## 3️⃣ DHCP Request

The client sends a request accepting the offered configuration.

Example:

> "I would like to use the IP address you offered." 
> Client → DHCP Server


---

## 4️⃣ DHCP Acknowledgement (ACK)

The DHCP server confirms the lease.

Example:

> "Confirmed. You may use this IP configuration for the lease period."
> DHCP Server → Client


---

# 🔌 DHCP Ports

DHCP uses UDP because the client does not have an IP address yet.

| Communication | Port |
|---|---|
| DHCP Server | UDP 67 |
| DHCP Client | UDP 68 |

---

# 🧠 Exam Highlights

## ⚠️ Watch Out For

- DHCP automatically assigns IP configuration.
- DHCP uses the **DORA process**:
  - Discover
  - Offer
  - Request
  - Acknowledge
- DHCP Discover uses a broadcast because the client does not know the DHCP server address.
- DHCP uses UDP ports **67 and 68**.
- Dynamic addresses are assigned using a lease.

---

## 💡 Key Takeaways

- DHCP eliminates the need for manual IP configuration.
- Static IPs are manually assigned and permanent.
- Dynamic IPs are automatically assigned and temporary.
- DHCP provides more than just an IP address; it provides complete network configuration.
- The DORA process allows clients and servers to negotiate IP assignments.




