---
title: "SNMP Data Harvesting with snmpwalk"
last_modified_at: 2025-06-11T12:30:00+03:00
categories:
  - Labs
tags:
  - SNMP
  - Enumeration
  - snmpwalk
  - HackTheBox
layout: single
read_time: true
author_profile: false
---

## 🔧 What is `snmpwalk`?

**`snmpwalk`** is a command-line tool used to query SNMP-enabled devices for detailed information in a tree-like structure. It recursively walks through the SNMP Object Identifier (OID) tree and pulls system data from network devices such as routers, switches, and servers.

This tool is part of the **Net-SNMP** suite and is frequently used in penetration testing and network audits to extract readable SNMP data once a valid community string is identified (e.g., with `onesixtyone`).

---

## 🧰 Key Features of `snmpwalk`

- 🔄 Recursively queries SNMP-enabled hosts  
- 📦 Dumps large amounts of system-level data in plaintext  
- 🧱 Supports SNMPv1, v2c, and v3  
- 🧠 Useful for network mapping, OS fingerprinting, and data leakage discovery

---

## 🧪 Example Usage

```bash
snmpwalk -v2c -c public 10.10.10.10
