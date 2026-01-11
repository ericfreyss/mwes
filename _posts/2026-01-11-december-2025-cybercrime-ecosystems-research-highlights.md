---
layout: post
title: "Cybercrime ecosystems: research and policy highlights from December 2025"
date: 2026-01-11
categories:
- cybercrime
- research
tags:
- cybercrime-ecosystems
- DeFi
- AI
- compliance
- fraud
lang: en
---

**AI GENERATION: This monthly research review was generated automatically and edited**

In December 2025, a number of academic papers and policy reports added useful pieces to our understanding of how cybercrime operates as an ecosystem.  
This short review focuses on five contributions that are particularly relevant to those studying criminal infrastructures, criminal business models, and systemic responses.

## DeFi crime and DAO governance: quantifying indirect losses

Kitzler, Paquet-Clouston and Haslhofer published an open-access article in *The Journal of Finance and Data Science* analysing the economic impact of crime events in the Decentralized Finance (DeFi) ecosystem, with a specific focus on DAOs and their governance tokens.[^kitzler]  

Using granular trading data for 22 major DeFi crime events between 2020 and 2022, they apply a dynamic difference-in-differences design to estimate how these incidents affect governance token prices, trading volumes and market capitalisation. The headline numbers are striking:

- The DeFi ecosystem has suffered more than 10 billion USD in **direct** losses from crime events.
- In about half of the events, governance token prices fall significantly, with an average drop in the order of **14 %** in the aftermath of the incident.
- Roughly two thirds of events are associated with a spike in trading volume, indicating “flight” or speculative behaviour around the affected assets.
- When they translate these dynamics into aggregate market-cap effects, they estimate **indirect losses** of more than 1.3 billion USD on DAO governance tokens – around **three quarters of total losses** once both direct and indirect effects are taken into account.   

From an ecosystem perspective, the key contribution is methodological. The paper shows how event-study techniques and counterfactual governance assets can be used to quantify not just victim-side losses, but the way crime events propagate across the wider DeFi governance layer. That approach is reusable for other parts of the crypto-crime ecosystem (bridges, CEX tokens, L2 governance, etc.).

[^kitzler]: Stefan Kitzler, Masarah Paquet-Clouston, Bernhard Haslhofer, “The economic impact of DeFi crime events on decentralized autonomous organizations (DAOs)”, *Journal of Finance and Data Science*, vol. 11, December 2025, article 100171, [https://doi.org/10.1016/j.jfds.2025.100171](https://doi.org/10.1016/j.jfds.2025.100171).

## AI-driven cybercrime in national context: the Ecuador case

In the *Journal of Cybersecurity and Privacy*, Varela Enríquez, Toasa and Urdaneta published an open-access article on AI-driven cybercrime in Ecuador.[^varela]  Although the geographical scope is national, the paper is interesting for anyone looking at how AI tools diffuse into cybercriminal ecosystems in emerging economies.

The authors document a sharp rise in reported cybercrime in Ecuador (around 7 % between 2023 and 2024, and close to 130 % between 2020 and 2021), and describe how AI tools are being used locally to generate **intelligent malware**, **automated phishing** and **AI-supported financial fraud**.   

Their main focus is on mitigation: they benchmark Ecuador’s institutional capacity against international frameworks such as NIST and ISO, and propose a set of measures combining standards adoption, public policy and large-scale training. In ecosystem terms, the paper underlines two points:

- The same AI-enabled attack techniques circulate globally, but **national capacity asymmetries** determine how much damage they do and which organisations become preferred entry points into global criminal infrastructures.
- For smaller or lower-income countries, adopting international governance frameworks is not enough; there is a need for dedicated funding and knowledge transfer so that institutional actors can actually implement those frameworks in environments where criminal actors may adapt faster than the state.

[^varela]: Carlos Varela Enríquez, Renato Toasa, Maryory Urdaneta, “The Use of Artificial Intelligence in Cybercrime: Impact Analysis in Ecuador and Mitigation Strategies”, *Journal of Cybersecurity and Privacy*, 5(4), 100, 2025, [https://doi.org/10.3390/jcp5040100](https://doi.org/10.3390/jcp5040100).

## Compliance asymmetries in the AI governance ecosystem

A second paper in the same issue of *Journal of Cybersecurity and Privacy* is less directly about cybercrime, but highly relevant for the structure of the “defender side” ecosystem. Finch and Butt provide a systematic review of AI governance frameworks centred on the EU AI Act, ALTAI, ISO/IEC 42001, the NIST AI RMF and OECD principles, with particular focus on **low-capacity actors** such as SMEs and public authorities.[^finch]   

Rather than proposing yet another governance model, they introduce the notion of **compliance asymmetry** inside the “compliance ecosystem”:

- Large platforms and well-resourced institutions are structurally better placed to meet the documentation, audit and lifecycle-risk requirements of the AI Act and related standards.
- SMEs and small public bodies face overlapping obligations (e.g. AI Act vs GDPR), but lack the staff and tooling to implement them in a proportionate way.
- Ethics-oriented instruments like ALTAI remain too high-level and miss a substantial portion of concrete security vulnerabilities, which further widens the gap between formal compliance and actual risk reduction.   

For cybercrime ecosystems, the implication is indirect but important: if low-capacity actors cannot realistically implement AI security and governance controls, they become **structural weak points** in the broader digital ecosystem – attractive as targets, stepping stones or infrastructure renters for criminal groups. The paper therefore complements more traditional CTI work by mapping where defensive capacity is systematically thin.

[^finch]: William Walter Finch, Marya Butt, “Gaps in AI-Compliant Complementary Governance Frameworks’ Suitability (for Low-Capacity Actors), and Structural Asymmetries (in the Compliance Ecosystem)—A Systematic Review”, *Journal of Cybersecurity and Privacy*, 5(4), 101, 2025, [https://doi.org/10.3390/jcp5040101](https://doi.org/10.3390/jcp5040101).

## Systemic fraud as an ecosystem problem: the WEF/IST framework

On the policy side, December 2025 saw the publication of *Fighting Cyber-Enabled Fraud: A Systemic Defence Approach*, a white paper from the World Economic Forum’s Partnership against Cybercrime, produced with the Institute for Security and Technology.[^wef]  

The document explicitly frames phishing and cyber-enabled fraud as **emergent properties of the digital infrastructure ecosystem**, rather than as a matter of individual user behaviour. It argues that losses (estimated at over 1 trillion USD in 2024) are driven by the way domains, hosting, messaging platforms and payment systems are provisioned and governed, and not just by the quality of end-user awareness campaigns.   

The proposed systemic defence model is organised along three pillars:

1. **Prevention** – embedding controls at the foundational layers (domain registration, hosting, messaging, payment rails) to make it harder for criminals to acquire and operate infrastructure at scale.
2. **Protection** – default-secure designs in consumer-facing products (email, browsers, messaging) so that users are shielded from large classes of fraud techniques by design, rather than by exception.
3. **Mitigation** – ecosystem-wide signal-sharing and coordinated response, with strong emphasis on AI-assisted threat detection to keep pace with AI-enabled fraud campaigns.   

For practitioners interested in cybercrime ecosystems, the report is useful because it maps **upstream control points** where interventions can have disproportionate impact: registrars, hosting providers, communications platforms, payment intermediaries, and the data-sharing mechanisms between them.

[^wef]: World Economic Forum & Institute for Security and Technology, *Fighting Cyber-Enabled Fraud: A Systemic Defence Approach*, December 2025, available via [WEF Centre for Cybersecurity](https://www.weforum.org/publications/fighting-cyber-enabled-fraud-a-systemic-defence-approach/).

## Cybercrime economy and ecosystem disruption in the MDDR 2025

Finally, Microsoft’s *Digital Defense Report 2025* (MDDR 2025), released in late 2025, provides an empirical perspective on how large-scale telemetry can be used to characterise and disrupt cybercrime ecosystems.[^mddr]  The report covers July 2024 to June 2025, but was widely discussed in December 2025 and includes two elements directly aligned with an ecosystem view:

- A dedicated chapter on **“Identity, access, and the cybercrime economy”**, which treats identity systems and access tokens as the primary substrate on which cybercrime markets now operate. Attacks increasingly rely on stolen credentials, OAuth abuse and access-broker services, rather than brute-force intrusion.   
- A case study on the **Lumma Stealer takedown**, explicitly framed as “disrupting cybercrime ecosystems”. Here, Microsoft shows how action on a single infostealer family (through C2 disruption and domain sinkholing) can significantly reduce the availability of fresh credentials in access markets, with measurable downstream impact on ransomware and other human-operated intrusions.   

The report is also notable for how it links identity-centric attacks, infostealer markets, initial-access brokers and ransomware affiliates into a single **commercial ecosystem**. For researchers, it provides data points and vocabulary that can be re-used in more formal ecosystem models.

[^mddr]: Microsoft, *Microsoft Digital Defense Report 2025*, 2025, available at [https://www.microsoft.com/security/security-insider/threat-landscape/microsoft-digital-defense-report-2025](https://www.microsoft.com/security/security-insider/threat-landscape/microsoft-digital-defense-report-2025).

## Takeaways for ecosystem-focused research

Taken together, these December 2025 publications and reports reinforce a few themes that are likely to structure research on cybercrime ecosystems over the next few years:

- **Crime externalities are systemic.** In DeFi, indirect losses borne by token holders and governance participants can exceed direct victim losses, which suggests similar under-counting in other domains where price signals are less transparent.
- **Capacity asymmetries matter as much as threat capabilities.** The Ecuador case study and the compliance-ecosystem review both show that weak institutional capacity in parts of the digital ecosystem shapes where criminals focus their efforts and how far attacks propagate.
- **Upstream control points are central.** The WEF systemic fraud framework and the MDDR case study both converge on the idea that registrars, hosting providers, communications platforms and payment systems are leverage points for disrupting entire criminal value chains.
- **Identity and data-theft malware are now core infrastructure for cybercrime.** The prominence of infostealers, access brokers and identity-centric attacks in Microsoft’s data confirms the shift from one-off intrusions to a more industrialised ecosystem where credentials and access tokens function as tradable commodities.

For anyone working on “cybercrime ecosystems” as an object of study, these contributions offer both empirical material (DeFi event studies, telemetry on identity attacks) and conceptual tools (compliance asymmetry, systemic defence pillars) that can be integrated into more formal models of how criminal and defensive infrastructures co-evolve.

**AI GENERATION: This monthly research review was generated automatically and edited**
