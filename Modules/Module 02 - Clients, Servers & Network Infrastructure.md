# Module 2: Hosts, Network Infrastructure & ISP Connectivity

**Date:** 2026-06-02 | **Status:** 🟢 Complete

## 🎯 Core Objective

Understand how hosts provide and consume network services, how network infrastructure moves traffic, and how local networks connect to the Internet.

---

## 🖥️ Hosts, Clients & Servers

- A **[Hosts](../Concepts/Hosts.md)** is a device that participates directly in network communication.
    
- A **Client** requests a service.
    
- A **Server** provides a service.
    
- A single host can act as a client and server simultaneously.
    
- A server can provide multiple services, such as web, email, and file services.
    

```text
Client ────── Request ──────> Server
Client <───── Response ───── Server
```

---

## 🔗 Peer-to-Peer Networks

In a **[Peer-to-Peer (P2P)](../Concepts/Peer-to-Peer%20(P2P).md)** network, devices can act as both clients and servers.

**Advantages:**

- Easy to set up.
    
- Low cost.
    
- Simple for small networks.
    
- Useful for basic file and printer sharing.
    

**Disadvantages:**

- No centralized administration.
    
- Less secure.
    
- Limited scalability.
    
- Device performance can decrease when providing and consuming services simultaneously.
    

---

## 🏗️ Network Infrastructure

|Component|Function|
|---|---|
|**End Device**|Source or destination of traffic|
|**Switch**|Connects devices within a LAN|
|**Router**|Connects different networks|
|**Firewall**|Controls traffic according to security rules|
|**Network Media**|Carries network signals|

A message typically travels through several devices before reaching its destination.

```text
Source
  ↓
Switch
  ↓
Router
  ↓
Other Networks
  ↓
Router
  ↓
Switch
  ↓
Destination
```

---

## 🌐 Internet Service Providers

A **Internet Service Provider (ISP)** provides connectivity between a local network and the Internet.

Common access methods include:

- **Cable:** Uses coaxial cable infrastructure.
    
- **DSL:** Uses telephone lines.
    
- **Fiber:** Uses fiber-optic infrastructure.
    
- **Cellular:** Uses mobile carrier networks.
    
- **Satellite:** Uses satellite communication.
    
- **Dial-up:** Uses traditional telephone infrastructure.
    

---

## 🔌 Home Network Connectivity

A typical home network uses a router to connect multiple devices to an ISP.

The router may provide:

- Wired Ethernet connections.
    
- Wi-Fi connectivity.
    
- Local IP addressing.
    
- Basic network security.
    
- A connection to the ISP.
    

```text
Devices
   ↓
Home Router
   ↓
ISP
   ↓
Internet
```

---

## 🧠 Exam Highlights

⚠️ **Watch out for**

- A **host** can be a client, server, or both.
    
- A **switch** primarily connects devices within a LAN.
    
- A **router** connects different networks.
    
- P2P does not require a dedicated server.
    
- An ISP connects the local network to the Internet.
    

💡 **Key Takeaways**

- **Client → requests services.**
    
- **Server → provides services.**
    
- **Switch → connects local devices.**
    
- **Router → connects networks.**
    
- **ISP → provides Internet connectivity.**