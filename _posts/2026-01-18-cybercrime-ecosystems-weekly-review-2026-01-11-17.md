---
layout: post
title: "Cybercrime ecosystems: news of the week (11–17 January 2026)"
date: 2026-01-18 09:00:00 +0100
categories:
  - Cybercrime
  - Threat Intelligence
tags:
  - Cybercrime ecosystems
  - Infostealers
  - RaaS
  - Initial access brokers
  - Botnets
  - Residential proxies
  - Telecom
lang: en
---

**AI GENERATION: This weekly review was generated automatically and edited**

This weekly review covers **Sunday 11 January to Saturday 17 January 2026**. The goal is not to list incidents, but to extract what they reveal about **cybercrime ecosystems**: shared services, upstream enablers, and the way markets (credentials, access, infrastructure) connect to downstream monetisation (extortion, fraud, disruption).

Building on last week’s review of botnets and access markets, this week’s analysis highlights how the same infrastructures now surface inside enterprises through residential proxy services.

---

## 1) Residential proxies as an attack surface: Kimwolf “inside the enterprise”

This week, **Infoblox** published a detailed analysis of *Kimwolf* that is particularly valuable from an ecosystem perspective: it frames Kimwolf less as a “classic botnet” and more as an operator **abusing residential proxy services** to probe corporate environments.

Key points:

- Infoblox observed Kimwolf-related DNS activity across customer environments and notes that **nearly 25%** of their cloud customers queried a Kimwolf domain since 1 October (which they interpret as evidence that many organisations have endpoints enrolled in proxy services that Kimwolf targets/abuses).  
- The report explicitly connects Kimwolf’s activity to **residential proxy providers** and the way their SDK footprint can be leveraged as an entry point for probing internal networks.

Source:  
- Infoblox (Jan 13, 2026): *“Kimwolf howls from inside the enterprise”*  
  https://www.infoblox.com/blog/threat-intelligence/kimwolf-howls-from-inside-the-enterprise/

Why it matters for “ecosystem” analysis: the real story is the **market layer** (proxy services and SDK distribution) becoming an implicit part of adversary infrastructure. The defensive problem is not only “patch vulnerable devices”, but also “identify and govern the presence of residential proxy tooling on endpoints”.

---

## 2) RaaS fragmentation and churn: Vect appears as a new affiliate platform

In its **January 6–12** intelligence report (overlapping the start of our week), **Red Piranha** described *Vect* as a newly emerged **Ransomware-as-a-Service** platform and provided ecosystem-level signals:

- affiliate recruitment and an entry fee (reported as **$250 in Monero**),
- dedicated negotiation portal and leak site,
- positioning against “builder reuse” narratives (claiming custom development).

Source:  
- Red Piranha: *Threat Intelligence Report January 6 to January 12, 2026*  
  https://redpiranha.net/news/threat-intelligence-report-january-6-january-12-2026

Why it matters: Vect is a good illustration of **low-friction entry** and **rapid brand turnover** in the ransomware market. Even if a given “brand” remains small, the ecosystem is resilient because the supply chain is standardised: access acquisition, exfiltration tooling, hosting, negotiation portals, leak publishing, and affiliate recruitment are increasingly modular.

---

## 3) “New” ransomware as downstream symptom: Karma (MedusaLocker family)

On **16 January 2026**, **CYFIRMA** highlighted “Karma (MedusaLocker)” as a ransomware strain they found while monitoring underground forums and described it as belonging to the **MedusaLocker** family, using hybrid crypto and adding a “.KARMA” extension.

Source:  
- CYFIRMA: *Weekly Intelligence Report – 16 January 2026*  
  https://www.cyfirma.com/news/weekly-intelligence-report-16-january-2026/

Why it matters: the recurring emergence of “new” strains is often less important than what it implies about the ecosystem’s upstream dependencies: affiliates, builders, access brokers, and the persistent availability of commodity tooling. Treating each new label as a standalone phenomenon is usually the wrong analytical unit; the correct unit is the **service stack** that enables it.

---

## 4) Infostealers as upstream “credit supply” for ransomware and access markets

A major ecosystem insight this week comes from a newly released PDF report by **GuidePoint Security** (GRIT 2026), which is unusually explicit about the role of infostealers and coordinated law enforcement disruption.

Key points discussed in the report:

- infostealers are described as a major **upstream component** of the ransomware ecosystem, feeding credential supply that can be repackaged and sold for initial access;
- it cites **Operation Secure** (Jan–Apr 2025) as a multi-country action against infrastructure tied to numerous infostealer variants;
- it also discusses **Operation Endgame** and the seizure of malware infrastructure at scale, framing these as **ecosystem-level disruption** rather than isolated arrests.

Source:  
- GuidePoint Security: *GRIT 2026 Ransomware and Cyber Threat Report* (PDF)  
  https://www.guidepointsecurity.com/wp-content/uploads/2026/01/GRIT-2026-Ransomware-and-Cyber-Threat-Report.pdf

Why it matters: this is a strong reminder that the ransomware economy behaves like a market with an upstream “commodity”—**credentials and authenticated sessions**—whose availability shapes the cost and scalability of downstream campaigns. Disrupting infostealer infrastructure is a way to attack the ransomware ecosystem **at its supply layer**.

---

## 5) Telecom remains a high-value ecosystem node

Even though the underlying telecom report was published slightly earlier, it remained widely referenced in January coverage: telecoms continue to be treated as high-value targets because they combine **critical infrastructure roles** with large-scale **subscriber data** and complex third-party dependencies.

Source:  
- Cybersecurity Dive (citing Cyble’s telecom threat landscape findings):  
  https://www.cybersecuritydive.com/news/telecom-ransomware-spike-cyble/809224/

Why it matters: telecom is not only a “victim sector”; it can function as an ecosystem **hub**—supporting downstream fraud (subscriber data), enabling further compromise (interconnections), and providing strategic leverage for extortion.

---

## Takeaways (ecosystem lens)

1. **Residential proxy services are increasingly part of adversary infrastructure**, sometimes indirectly via SDK footprints and consumer endpoints present inside organisations.  
2. **RaaS churn is a feature, not a bug**: new brands emerge continuously because the supply chain is modular and reusable.  
3. **Infostealers remain the key upstream substrate**: credentials and sessions are the commodity that connects malware distribution to initial access brokers and ransomware affiliates.  
4. **Sector “hubs” matter**: telecom exemplifies how some industries create disproportionate downstream value for multiple criminal business models.

---

**AI GENERATION: This weekly review was generated automatically and edited**
