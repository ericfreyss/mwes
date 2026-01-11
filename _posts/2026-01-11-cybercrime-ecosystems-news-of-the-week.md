---
layout: post
title: "Weekly Cybercrime Ecosystems Update – 4–10 January 2026"
date: 2026-01-11 10:00:00 +0100
categories:
  - Cybercrime
  - Threat Intelligence
tags:
  - Cybercrime ecosystems
  - Botnets
  - Ransomware-as-a-Service
  - Infostealers
  - Telecom
lang: en
---

For several years now, I have argued that cybercrime should not be viewed as a collection of isolated tools (a botnet here, a ransomware strain there, a phishing campaign somewhere else), but as an **ecosystem** of actors, services, and infrastructures. The news cycle of the past week — from **Sunday 4 January to Saturday 10 January 2026** — provides yet another illustration of this.

Across botnets, ransomware operations, initial access brokers and sector-specific pressure on telecoms, we see the same pattern: **modular services, shared infrastructures, and long-lived criminal value chains**.

---

## 1. Kimwolf: an Android botnet plugged into residential proxy markets

Multiple analyses published this week revisited the Android botnet **Kimwolf**, showing clearly how it fits into a broader criminal ecosystem rather than acting as a standalone tool.

According to reporting based on research from Synthient, Kimwolf has infected **more than two million Android devices**, primarily Android TV boxes and similar devices exposed via Android Debug Bridge (ADB) and funneled through **residential proxy networks**. From there, the botnet can be used to:

- launch large-scale DDoS attacks,  
- sell residential proxy bandwidth,  
- push unwanted application installs and other monetization software.  

See for instance [SecurityWeek’s coverage](https://www.securityweek.com/kimwolf-android-botnet-grows-through-residential-proxy-networks/) and a summary at [Cypro.se](https://www.cypro.se/2026/01/05/kimwolf-android-botnet-infects-over-2-million-devices-via-exposed-adb-and-proxy-networks/).

Brian Krebs provides additional context in a piece on **“Who Benefited from the Aisuru and Kimwolf Botnets?”**, tracing overlaps in code, infrastructure and monetization between Kimwolf and the earlier Aisuru botnet, and showing how both fed into **proxy, DDoS and traffic-fraud markets** rather than operating in isolation: [KrebsOnSecurity – Kimwolf botnets](https://krebsonsecurity.com/category/breadcrumbs/).

This is a textbook ecosystem pattern:

- Kimwolf itself as **infrastructure-as-a-service**,  
- existing **residential proxy providers** whose networks are hijacked or abused,  
- downstream **criminal clients** paying for bandwidth, installs or DDoS capability,  
- external services such as DNS-over-TLS or blockchain-based naming, used to increase resilience.

Kimwolf is thus not just “another botnet”, but a **meta-actor** embedded in several interconnected criminal markets.

---

## 2. Medusa: a RaaS platform leveraging third-party services

On the ransomware side, the **Medusa** operation continued to make headlines. On **5 January 2026**, Dexpose reported a Medusa attack against *Resource Corporation of America*, a U.S. healthcare revenue optimisation company, with the group threatening to leak sensitive data if negotiations failed:

> [Medusa Ransomware Targets Resource Corporation of America](https://www.dexpose.io/medusa-ransomware-targets-resource-corporation-of-america/) (Dexpose, 5 Jan 2026).

This is only the latest in a long series of incidents involving Medusa, which operates as **Ransomware-as-a-Service (RaaS)** since at least 2021. A joint FBI/CISA/MS-ISAC advisory in March 2025 already highlighted its activity and RaaS model:

- [Advisory warns of Medusa ransomware activity](https://www.aha.org/news/headline/2025-03-14-advisory-warns-medusa-ransomware-activity).

Analysts such as Darktrace have also shown how Medusa affiliates increasingly abuse **Remote Monitoring and Management (RMM) tools** — Atera, AnyDesk, ScreenConnect, TeamViewer, etc. — for persistence, lateral movement and data exfiltration:

- [Under Medusa’s Gaze: How Darktrace Uncovers RMM Abuse in Ransomware Campaigns](https://www.darktrace.com/blog/under-medusas-gaze-how-darktrace-uncovers-rmm-abuse-in-ransomware-campaigns).

Here again, we are looking at an ecosystem:

1. **Core operators** developing and maintaining the Medusa codebase and leak infrastructure.  
2. **Affiliates** renting access to the ransomware in exchange for a revenue share.  
3. **Initial access brokers (IABs)** selling compromised access obtained via other malware or vulnerabilities.  
4. **Abuse of legitimate services** (RMM tools, VPNs, cloud storage) as ready-made infrastructure.

Medusa is less a single “group” than a **platform around which many other services are orchestrated**.

---

## 3. Emerging RaaS operations: Ripper and BQTLock

Ransomware-as-a-Service is not limited to well-known names. CYFIRMA’s **Weekly Intelligence Report – 9 January 2026** describes a newer ransomware called **Ripper**, which encrypts files with RSA/AES, appends a `.ripper12` extension and targets multiple file types across Windows environments:

- [CYFIRMA – Weekly Intelligence Report – 09 January 2026](https://www.cyfirma.com/news/weekly-intelligence-report-09-january-2026/).

In parallel, other vendors have been tracking **BQTLock**, a RaaS family that emerged in mid-2025 and has continued to evolve. Red Piranha’s **Threat Intelligence Report – December 30, 2025 to January 5, 2026** includes a dedicated section on BQTLock as an “emerging Ransomware-as-a-Service (RaaS) platform”, noting its hybrid encryption (AES-256 + RSA-4096) and `.bqtlock` file extension:

- [Red Piranha – Threat Intelligence Report December 30, 2025 – January 5, 2026](https://redpiranha.net/news/threat-intelligence-report-december-30-2025-january-5-2026).

More detailed technical analyses (SOC Prime, Cynet, others) emphasise its **double-extortion model**, anti-analysis features, and ties to the **ZeroDayX1** cluster:

- [BQTLOCK Ransomware Detection – SOC Prime](https://socprime.com/blog/bqtlock-ransomware-detection/).  
- [CyOps Analysis: BQTLock Ransomware – Cynet](https://www.cynet.com/blog/cyops-analysis-bqtlock-ransomware/).  
- [BQT.Lock cyberattack group – Wikipedia](https://en.wikipedia.org/wiki/BQT.Lock_cyberattack_group).

Taken together, these reports show:

- a **diverse RaaS landscape**, with a few dominant “brands” and a long tail of regional or sector-specific families;  
- a high degree of **standardisation of TTPs**, often described in MITRE ATT&CK terms;  
- reliance on shared **ecosystem services**: crypters, bulletproof hosting, IABs, leak-site infrastructure, and so on.

---

## 4. Zestix / Sentap: an infostealer-fuelled initial access broker

One of the most striking stories of the week concerns a single threat actor operating under the aliases **“Zestix”** and **“Sentap”**. According to a report by Hudson Rock, summarised by several media outlets, this actor used **credentials harvested by commodity infostealers** to access cloud storage and collaboration platforms at around **50 global enterprises** across sectors such as aviation, robotics, utilities, government infrastructure and defence.

SecurityWeek reports:

> A threat actor known as Zestix and Sentap has hacked dozens of global enterprises using credentials exfiltrated via information stealers.  
> — [SecurityWeek – Dozens of Major Data Breaches Linked to Single Threat Actor](https://www.securityweek.com/dozens-of-major-data-breaches-linked-to-single-threat-actor/).

Other outlets echo the findings:

- [Infosecurity Magazine – MFA Failure Enables Infostealer Breach at 50 Enterprises](https://www.infosecurity-magazine.com/news/mfa-failure-infostealer-breach-50/).  
- [The Register – One criminal stole info from 50 orgs thanks to no MFA](https://www.theregister.com/2026/01/06/50_global_orgs_hacked/).  
- [Cryptika – Threat actors hacked global companies via leaked cloud credentials from infostealer infections](https://www.cryptika.com/threat-actors-hacked-global-companies-via-leaked-cloud-credentials-from-infostealer-infections/).

The key points:

- No zero-days or exotic techniques — **just valid usernames and passwords** from infostealer logs.  
- Many credentials were **years old**, yet still worked.  
- Most victims **had not enforced MFA** on exposed services.

This case underlines the central role of **infostealers and IABs** as the “glue” of cybercrime ecosystems:

1. Infostealer campaigns capture vast numbers of credentials and sessions.  
2. Logs are monetised in markets and by specialised brokers like Zestix/Sentap.  
3. These access vectors are then reused across ransomware, espionage and fraud operations.

---

## 5. Telecom: a high-value node in the global ecosystem

On **9 January 2026**, several outlets relayed findings from Cyble’s **Telecommunications Sector Threat Landscape Report 2025**, which paints a worrying picture of sustained pressure on telecom operators:

- [Cyble – Telecommunications Sector Threat Landscape Report 2025](https://cyble.com/resources/research-reports/telecommunications-sector-threat-landscape-report-2025/).  
- [Cybersecurity Dive – Telecom sector sees steady rise in ransomware attacks](https://www.cybersecuritydive.com/news/telecom-ransomware-spike-cyble/809224/).  
- [SC Media – Telecom firms faced constant cyber threats in 2025, says Cyble](https://www.scworld.com/brief/telecom-firms-faced-constant-cyber-threats-in-2025-says-cyble).

Key figures from the report:

- **444 incidents** against telecoms in 2025 (breaches, leaks, ransomware, access sales, hacktivism).  
- **90 ransomware attacks**, involving at least 34 distinct groups.  
- Subscriber databases and network access being traded on underground markets.

For many threat actors, compromising a telecom provider is not just about ransom revenue. It can also yield:

- access to **large subscriber datasets** (targets for SIM-swapping, phishing, fraud),  
- opportunities for **network-level visibility or interception**,  
- a stepping-stone to other organisations through trusted interconnections.

This positions telecoms as **critical nodes** in the wider criminal ecosystem: attacking them can support multiple business models at once (extortion, espionage, data brokerage, fraud).

---

## 6. What this week tells us about cybercrime ecosystems

Taken together, the events of 4–10 January 2026 reinforce several structural lessons:

1. **Infrastructures matter more than individual tools.**  
   Kimwolf shows how a botnet becomes a multi-purpose infrastructure feeding DDoS, proxies and traffic fraud. Medusa functions as a RaaS platform around which multiple actors and services organise themselves.

2. **“Commodity” malware powers high-impact campaigns.**  
   The Zestix/Sentap story shows that widely available **infostealers** and their logs remain a cornerstone of many serious breaches. The real value lies not in novelty, but in the **systematic exploitation of accumulated data**.

3. **RaaS diversification continues.**  
   Ripper and BQTLock illustrate a RaaS market with both dominant families and a continuous stream of new entrants — many of them regionally or ideologically anchored, all of them drawing on shared services (cryters, IABs, leak infrastructure).

4. **Critical sectors act as hubs.**  
   Telecom operators exemplify how certain sectors sit at the **intersection** of many criminal interests: subscriber data, network access, interconnection with other industries. Attacks against them ripple through the ecosystem.

5. **Time scales are long.**  
   Just as credentials from old breaches still fuel new intrusions, infrastructures like botnets and proxy networks can survive or re-emerge even after partial takedowns. Ecosystems persist and adapt faster than most linear incident-response models assume.

---

## Conclusion

The week’s news does not just tell us that “another botnet was discovered” or “yet another ransomware attack occurred”. It confirms that **contemporary cybercrime is best understood as an ecosystem**:

- a mesh of **services** (RaaS, MaaS, IABs, proxy providers),  
- **technical infrastructures** (botnets, RMM tools, cloud services),
- **markets and forums** where data and access rights are traded,  
- and a diverse set of **actors** that plug in and out of these components.

For defenders, policymakers and researchers, this implies:

- going beyond case-by-case analysis to identify **shared dependencies** and recurring services;  
- designing responses that **disrupt chains**, not just individual operators;  
- investing in **cross-disciplinary approaches** (technical, economic, criminological) to map and weaken these ecosystems.

It is at this scale — the scale of **cybercrime ecosystems** — that our understanding and our counter-measures need to operate.

