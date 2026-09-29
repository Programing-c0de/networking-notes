# Module 05: Understanding protocols and standards
**Date:** 2026-06-11 | **Status:** 🟢 Completed


## 🎯 Core Objective:
Understanding the difference between TCP/IP and the OSI model, and how they are related to enable network communication.

---


## 🔑 Key Concepts & Pillars

### 📡 1. Protocols
* A **protocol** is a set of rules that devices agree on before communication.

It defines:
1. **Method** – How communication occurs (text, voice, signals, etc.)
2. **Language/Format** – The structure and meaning of the data being exchanged.
3. **Confirmation** – How devices acknowledge that data was received correctly.

### 💡 2. Why do protocols matter?
* Protocols ensure devices communicate in a predictable and reliable way.
* Without agreeing on the same protocols, devices cannot understand each other or exchange data successfully.

**Analogy:** Just as people speaking different languages cannot communicate effectively, computers using different protocols cannot communicate properly.
### 🌐 3. TCP/IP Model

The **TCP/IP model** groups networking protocols into layers that work together to deliver data across networks.

**Benefits**
- Simplifies protocol design
- Encourages interoperability
- Supports future upgrades
- Provides a common networking framework
---

## 🏢 OSI Layers

| Layer            | Function                                                              |
| ---------------- | --------------------------------------------------------------------- |
| **Application**  | Provides network services to applications (HTTP, FTP, DNS).           |
| **Presentation** | Translates, encrypts, and compresses data.                            |
| **Session**      | Establishes, manages, and terminates communication sessions.          |
| **Transport**    | Provides reliable data delivery and segmentation (TCP/UDP).           |
| **Network**      | Handles logical addressing and routing (IP).                          |
| **Data Link**    | Transfers frames between devices on the same network (MAC addresses). |
| **Physical**     | Transmits bits across the physical medium (cables, radio signals).    |
 

📖 **OSI MODEL** provides a general framework for networking functions.

---

## 🔀 TCP/IP ↔️ OSI Mapping

| TCP/IP Layer   | Corresponding OSI Layer(s)           |
| -------------- | ------------------------------------ |
| Application    | Application + Presentation + Session |
| Transport      | Transport                            |
| Internet       | Network                              |
| Network Access | Data Link + Physical                 |
  

📘 **TCP/IP Model Overview** shows interaction between TCP/IP protocols

---


### ⚠️ Watch out for
- TCP/IP has **4 layers**, while OSI has **7 layers**.
- The **OSI model** is a reference model; **TCP/IP** is the model used on the Internet.
- OSI explains **how networking works**; TCP/IP explains **how the Internet actually communicates**.

### 💡 Key Takeaways
- Protocols are rules for communication.
- The OSI model is conceptual.
- TCP/IP is practical and widely implemented.
- Every layer has a specific responsibility.