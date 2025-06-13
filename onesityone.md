---
title: "SNMP Enumeration with onesixtyone"
last_modified_at: 2025-06-11T10:45:00+03:00
categories:
  - Labs
tags:
  - SNMP
  - Enumeration
  - onesixtyone
  - HackTheBox
---

This post documents an SNMP enumeration lab using the tool `onesixtyone`, part of the Network Fundamentals module on Hack The Box.

All vulnerable networks leak data in some form — SNMP is one such quiet and underestimated service. During this challenge, `onesixtyone` helped identify exposed community strings in the target network. Once accessed, tools like `snmpwalk` allowed full visibility into the system — user accounts, interface configs, and network topology.

The scan uncovered useful system-level metadata using the public community string and validated the importance of securing SNMP v1/2c with stronger credentials or disabling it entirely.

One day, in a quiet terminal session, we typed:

```bash
onesixtyone -c community.txt 10.10.10.0/24
