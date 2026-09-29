# Lab 09: Build a Small LAN

**Date:** 2026-08-02 | **Status:** 🟢 Completed

## 🎯 Objective

Configure a small LAN and verify communication between hosts.

---

# 🛠️ Skills Practiced

- Configure IPv4 addresses.
- Use ping
- Use ipconfig /all
- Configure subnet masks.
- Configure default gateways.
- Verify connectivity.
- Test DNS name resolution.
- Use `tracert` to observe packet paths.

---

# 💡 Key Observations

## Why are the IPv4 addresses different?

Every host on a network requires a **unique IPv4 address**.

Hosts cannot share the same IP address because the network would not know which device should receive the traffic.

---

## Why are the subnet masks the same?

All hosts belong to the **same subnet**, so they use the same subnet mask to identify the network and host portions of an IP address.

---

## Why is the default gateway the same?

All devices on the LAN use the **router interface connected to that subnet** as their default gateway.

Whether configured manually or assigned by DHCP, every device on the subnet uses the same gateway to reach remote networks.

---

## What default gateway would the printer use?

The printer would use the same default gateway as every other device on the LAN because it belongs to the same subnet.

---

## DNS Troubleshooting

### If the IP address works but the URL does not

The most likely cause is a **DNS problem**.

The client can reach the server by its IP address but cannot resolve the hostname into an IP address.

---

## Traceroute

`tracert` shows each router that forwards the packet toward the destination.

Each hop represents a router interface.

The first hop is usually the **default gateway**.

---
## Reflection Part 

The biggest facilities challenge is making sure the new location has the necessary network infrastructure, including Internet service, cabling, power, and space for networking equipment.

---


# 🧠 What I Learned

- Every host must have a unique IP address.
- Devices on the same subnet share the same subnet mask.
- Devices on the same subnet share the same default gateway.
- Routers connect different networks.
- DNS translates hostnames into IP addresses.
- `tracert` displays the path packets take through routers.