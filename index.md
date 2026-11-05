---
layout: default
title: Salman Sainudeen — SOC Analyst & Penetration Tester
description: >-
  Junior SOC analyst and penetration tester. Wazuh home SOC lab, Active Directory attack and defence lab,
  PortSwigger web security labs. Open to SOC and VAPT roles in India, the Gulf or remote.
---

# Salman Sainudeen

**Penetration Testing & SOC** · Kerala, India — currently in Al‑Khobar, Saudi Arabia · open to junior SOC, VAPT and pentest roles (India, Gulf or remote)

I'm a cybersecurity graduate working towards my first security role. I finished an eight-month **Advanced Penetration Testing diploma at eHackify** (web, network, API and mobile VAPT, Active Directory attack chains, SOC fundamentals). Most of what I know came from building labs and breaking them — and writing down what went wrong.

## Projects

### Home SOC lab — Wazuh on Docker
Wazuh (manager, indexer, dashboard) deployed with the official single-node Docker compose on an Arch VM, with agents sending logs and detection rules on top.
The interesting part was the failure: the dashboard returned 500 because the disk hit 100% and the indexer's health check failed. Found it by reading `docker compose logs wazuh.indexer`, fixed it by clearing space, and learned how OpenSearch disk watermarks (85 / 90 / 95%) quietly break a cluster.
First detection: failed Windows logons (4625) caught from a Windows agent. [Read the write-up →](first-detection-4625.html)

### Active Directory attack & defence lab
Windows Server 2019 domain with three clients. Ran Kerberoasting, AS-REP Roasting, DCSync and SMB relay with Impacket and CrackMapExec — then wrote the defender's side: GPO hardening, logging, tiered administration.

### Web security
PortSwigger Web Security Academy labs across SQL injection, XSS, CSRF and SSRF. Write-ups below as they're published.

### Guardrailed AI recon agent
An AI reconnaissance agent that can run security tools but **can't go out of scope or run anything destructive** — the policy is enforced *outside* the model (allowlist, scope file, command validation, audit log). The interesting part is the security layer that resists prompt injection. [Read the write-up →](recon-agent.html)

## Write-ups
See [Write-ups](writeups.html).

## Learning now
LetsDefend SOC Analyst path · OverTheWire (Bandit) · PortSwigger Apprentice · completed picoCTF · working towards eJPT, then OSCP.

## Events
Attending **Black Hat MEA 2026** (Riyadh, December 2026).

## Contact
salmansainudeen@gmail.com · [LinkedIn](https://www.linkedin.com/in/salmansainudeen) · [GitHub](https://github.com/salmansainudeen)
