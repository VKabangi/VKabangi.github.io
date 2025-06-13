---
title: "SNMP Enumeration with onesixtyone"
last_modified_at: 2025-06-11T11:45:00+03:00
categories:
  - Labs
tags:
  - SNMP
  - Enumeration
  - onesixtyone
  - HackTheBox
layout: single
read_time: true
author_profile: false
---

## 🔧 What is `onesixtyone`?

**`onesixtyone`** is a fast and lightweight SNMP scanner used to enumerate SNMP-enabled devices on a network by brute-forcing community strings.

SNMP (Simple Network Management Protocol) is commonly used by network devices (like routers, switches, and printers) to expose information for monitoring. However, if SNMP is misconfigured (e.g., using the default `"public"` community string), attackers can access sensitive system information without authentication.

---

## 🧰 Key Features of `onesixtyone`

- 🔍 Fast brute-force of SNMP community strings across IP ranges  
- 🚀 High-speed scanning on UDP port 161  
- 🎯 Helps identify vulnerable SNMP services  
- 📡 Lightweight and ideal for mass discovery

---

## 🧪 Example Usage

```bash
onesixtyone -c community.txt 10.10.10.0/24
