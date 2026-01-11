---
layout: post
title: "From botnets to criminal ecosystems: ten years of expansion and a profound transformation of crime"
date: 2025-11-22 10:00:00 +0100
categories:
  - Cybercrime
  - Criminal ecosystems
tags:
  - Botnets
  - Cybercrime
  - Criminal ecosystems
  - Phishing
  - ShinyHunters
lang: en
original_lang: fr
original_url: "https://eric.freyssi.net/2025/11/22/des-botnets-aux-ecosystemes-criminels-dix-ans-dextension-et-une-transformation-profonde-de-la-delinquance/"
---

When I defended my doctoral thesis in November 2015, I sought to define a model for all the malware of the time that was, in one way or another, connected to its operator. I advocated in particular the following idea: botnets should not be viewed as mere networks of compromised machines, but as socio-technical assemblages made of actors, infrastructures, economic flows, and organizational constraints. This perspective, combining technical analysis with an understanding of human dynamics, led to discussions of *systems* rather than isolated tools, and of *criminal ecosystems* rather than discrete threats. I also insisted on the need for a proactive posture aimed at disrupting the criminal organization as a whole — not merely its visible manifestations.

Ten years later, this perspective has lost none of its relevance ([Freyssinet, *Revue des Mines*, 2025](https://revue-mines.org/les-ecosystemes-cybercriminels/)). What has changed, however, is the scale of the phenomenon. The ecosystem dynamics observed in botnets have spread across cybercrime and have even taken root in certain segments of so-called “traditional” crime. Those wishing to explore this further may refer to Benoît Dupont’s book (*La cybercriminalité, approche écosystémique de l’espace numérique*, 2024), which develops the notion of project-based delinquency.

## From cyber threats to criminal ecosystems

Beginning in the 2010s, cybercrime underwent a profound reconfiguration. Operations fragmented into a multitude of specialized roles: malware developers, initial access operators, infrastructure managers, data resellers, money launderers, technical service providers. As Benoît Dupont describes, cybercrime is articulated through a service marketplace where skills can be recruited, rented, or replaced as needed.

This segmentation, combined with extensive outsourcing, enabled the emergence of genuine criminal value chains (van Wanberg et al., 2017, [doi:10.1007/s10610-017-9336-3](https://doi.org/10.1007/s10610-017-9336-3)), where each function can be rented, replaced, or automated.

This modularity has become the norm. Cybercrime groups (Nurse & Bada, 2019, [arXiv:1901.01914](https://arxiv.org/pdf/1901.01914)) no longer execute the full chain themselves: they select, purchase, or combine services — bulletproof hosting, crypters, ready-to-use kits, proxies, initial access, laundering. The resilience of these structures rests precisely on their ability to rapidly recompose when any element is disrupted.

## Online scams: the organization behind the volume

Online scams illustrate this evolution perfectly. They are no longer the work of isolated individuals but of organizations that combine social engineering, infrastructure, automation, and financial logistics. Analyses by Europol ([online fraud schemes](https://www.europol.europa.eu/crime-areas/online-fraud-schemes)), UNODC, and other bodies show that these networks function like criminal enterprises: recruitment via social networks, task segmentation, behavioral scripts, encrypted messaging, guides and tutorials, internal platforms, rapid conversion of proceeds.

Beyond the variety of schemes, the structure itself matters: fraud is embedded in a modular, distributed, and organized environment — an ecosystem. And at the heart of this ecosystem lies one technique that recurs systematically and has its own sub-ecosystem: phishing.

## Phishing: an industrialized activity

Often presented as a simple social engineering trick, phishing today is one of the most structured subsystems of digital crime. Research (Alkhalil et al., 2021, [Frontiers in Computer Science](https://www.frontiersin.org/articles/10.3389/fcomp.2021.563060/full)) shows that phishing relies on a clear distribution of roles: kit design, covert hosting, target databases, automation of sending, credential harvesting, resale or reuse of collected data.

This segmentation is supported by a flourishing phishing-as-a-service (PhaaS) market. Criminal marketplaces distribute kits integrating cloned pages, anti-detection modules, cloaking systems, anti-bot measures, real-time dashboards, automatic updates, and integrations with Telegram or other messaging platforms.

Meanwhile, botnets have long held a central place in this ecosystem — as noted as early as OECD (2010) ([link](https://www.oecd.org/en/publications/the-role-of-internet-service-providers-in-botnet-mitigation_5km4k7m9n3vj-en.html)):

1. **as sending platforms** (Zhuang et al., 2008, [USENIX LEET’08](https://www.usenix.org/conference/leet-08/characterizing-botnets-email-spam-records)), enabling large-scale phishing distribution while bypassing anti-spam mechanisms;  
2. **as support infrastructures**, hosting or relaying phishing pages using distributed fast-flux networks.

Recent judicial operations have highlighted the robustness of these ecosystems.  
The dismantling of **QakBot** in 2023 ([US DOJ](https://www.justice.gov/usao-cdca/pr/qakbot-malware-disrupted-international-cyber-takedown)) revealed an infrastructure used for sophisticated phishing campaigns relying on the diversion of existing conversations and payload delivery to other groups.  
**Emotet**, before that, demonstrated the ability of a network to combine phishing propagation, access-for-rent services, and distribution of malicious payloads ([CERT-FR, 2021](https://www.cert.ssi.gouv.fr/cti/CERTFR-2020-CTI-010/)).

In all these cases, phishing is not an isolated operation: it is the entry point into a system — an essential link in a broader ecosystem of tools, infrastructure, skills, and markets.

## A dynamic extending beyond the digital world

This ecosystem logic now extends beyond cybercrime. Drug trafficking, for instance, has structured itself around similar practices ([UNODC 2024, Synthetic Drugs](https://www.unodc.org/roseap/uploads/documents/Publications/2024/Synthetic_Drugs_in_East_and_Southeast_Asia_2024.pdf)): recruitment, segmentation, digital logistics, social networks, cryptocurrencies, subcontracting of technical or operational tasks. The point is not that these phenomena are identical, but that they share comparable organizational mechanisms.

Another UNODC report on Southeast Asia ([TOC Convergence Report, 2024](https://www.unodc.org/roseap/uploads/documents/Publications/2024/TOC_Convergence_Report_2024.pdf)) confirms that criminals have adopted advanced technologies — malware, cryptocurrencies, generative AI — to reinforce capabilities, automate tasks, diversify methods, and facilitate the laundering of massive sums. These innovations allow activities to shift between jurisdictions, continuously adapt, and more effectively circumvent enforcement measures.

These groups rely heavily on clandestine marketplaces, particularly on Telegram, where services, stolen data, fraud tools, laundering solutions, and forced labor are exchanged. These platforms sustain and expand a resilient transnational criminal ecosystem.

The colossal scale of this criminal economy has led to the industrialization of fraud operations. Small, dispersed groups have been replaced by larger, more structured organizations, often based in industrial parks, special economic zones, casinos, or hotels. These sites host multiple actors engaging in diverse illicit activities targeting victims worldwide.

## More nebulous organizations: the example of ShinyHunters

Among recent evolutions, the case of **ShinyHunters** ([Wikipedia](https://en.wikipedia.org/wiki/ShinyHunters)), active since 2019, illustrates how certain cybercrime groups operate through distributed value chains. The group became visible following massive data thefts (Tokopedia, Unacademy, Wattpad, Nitro PDF), followed by resale or extortion on markets such as BreachForums.

In 2024, ShinyHunters appeared at the center of the **Snowflake** incident ([Wikipedia](https://en.wikipedia.org/wiki/Snowflake_data_breach)), involving exfiltration of data from multiple companies, including Ticketmaster and Santander, using compromised Snowflake accounts. Public analyses indicate the use of infostealer-derived credentials, the absence of MFA on some accounts, and the sale of terabytes of customer data.

Since 2025, several threat-intelligence reports have attributed to the group the theft of data from hundreds of Salesforce instances, via compromise of OAuth tokens linked to Drift/Drift Email (see [Salesloft](https://en.wikipedia.org/wiki/Salesloft), [Drift](https://en.wikipedia.org/wiki/Drift_(company)), [token-based auth](https://en.wikipedia.org/wiki/Token-based_authentication)). The attackers claimed roughly **1.5 billion records**, initiating an extortion campaign. Salesforce publicly confirmed the incident on the third-party supplier side and refused to negotiate.

Public analyses include:  
- Google Cloud TI: [UNC5537 Snowflake data theft](https://cloud.google.com/blog/topics/threat-intelligence/unc5537-snowflake-data-theft-extortion?hl=en)  
- Push Security: [Snowflake breach explained](https://www.pushsecurity.com/blog/snowflake-breach-explained)  
- BleepingComputer: [ShinyHunters claims 1.5B Salesforce records](https://www.bleepingcomputer.com/news/security/shinyhunters-claims-15-billion-salesforce-records-stolen-in-drift-hacks/)  
- Google Cloud: [voice-phishing and data extortion](https://cloud.google.com/blog/topics/threat-intelligence/voice-phishing-data-extortion?hl=en)  
- Ars Technica: [Salesforce won’t pay extortion](https://arstechnica.com/security/2025/10/salesforce-says-it-wont-pay-extortion-demand-in-1-billion-records-breach/)

Judicial investigations confirm the existence of a distributed ecosystem: the arrest and conviction of an alleged member in 2024 did not end the group’s activities, and arrests in France in 2025 linked to the administration of BreachForums suggest the existence of several circles operating under the same banner.

To add further complexity, while ShinyHunters appears distinct from groups like **Lapsus$** ([Wikipedia](https://en.wikipedia.org/wiki/Lapsus$)) or **Scattered Spider** ([Wikipedia](https://en.wikipedia.org/wiki/Scattered_Spider)), several analyses point to an opportunistic alliance emerging in 2024–2025 under the name **Scattered Lapsus$ Hunters (SLH)** — a “super-group” or “federated brand” used by different actors, notably on Telegram.

A diagram from Flare illustrates the entanglement of members of ShinyHunters, Lapsus$, Scattered Spider, and The Com (Source: [Flare](https://flare.io/)).

This type of organization — fluid identities, absence of stable hierarchy, capacity to recompose despite arrests — confirms the need to view these threats as ecosystems, where specialized roles, distributed infrastructure, compromised access, and data markets intersect.

## Thinking and acting “at the ecosystem level”

For judicial actors and researchers alike, this transformation requires sustained adaptation:

1. **Develop a systemic reading of threats.**  
   A phishing campaign or botnet is never isolated; it is the expression of a distributed system supported by many actors, services, and infrastructures.

2. **Target dependencies rather than operators alone.**  
   Effective response lies in identifying intermediaries, rented services, and the technical and economic flows that enable the organization.

3. **Disrupt chains, not just symptoms.**  
   Neutralizing a server or arresting an individual is often insufficient if the ecosystem can immediately recompose. Effective action must target anchor points: hosting, proxies, specialized providers, financial flows, recruitment mechanisms. This is precisely what coordinated international operations such as *Endgame* seek to achieve ([Endgame](https://en.wikipedia.org/wiki/Endgame_(cyber_operation))).

4. **Mobilize interdisciplinarity.**  
   Technical analysis must be complemented by criminology, psychology, the economics of crime, and data analysis — precisely the ambition of the *Defmal* programme of the PEPR Cybersécurité (workshop of 12 March 2025).

5. **Build anticipatory capabilities.**  
   Proactivity is no longer a luxury but a condition for effectiveness. Understanding criminal ecosystems means understanding where they can be weakened — and acting before they reconfigure. It also means detecting them as early as possible, when they are building their infrastructures and coordination mechanisms.

Ten years after completing my thesis, botnets thus appear not as relics of the past, but as an analytical model that sheds light on a wide array of contemporary criminal phenomena. They are no longer merely compromised machines: they are structures, actors, relationships.

Ecosystems.

And it is at that scale that we must think and act.
