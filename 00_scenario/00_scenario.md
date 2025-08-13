# 00 — Scenario

## 🧠 Scenario
Your SOC has received multiple suspicious IP addresses, domain names, and file hashes from a trusted partner organization.  
You’ve been tasked with validating these Indicators of Compromise (IOCs), enriching them with additional threat intelligence,  
and integrating this enriched data into your security operations for proactive defense.

## 🎯 Objective
- Collect IOCs from a provided dataset or simulated feed.
- Validate IOCs using multiple threat intelligence sources.
- Enrich IOCs with contextual data such as threat actor attribution, malware family, and observed attack patterns.
- Store the enriched data in a centralized threat intelligence platform for SOC use.

## 💻 Lab Environment

| Component | Purpose |
|-----------|---------|
| **Kali Linux VM** | Primary analyst workstation with `MISP` and `VirusTotal` CLI tools installed. |
| **MISP Instance** | Local or cloud-based MISP deployment for storing and correlating threat intelligence. |
| **Threat Intel Feeds** | Simulated IOC dataset plus live threat feeds (as applicable). |
| **WHOIS / Passive DNS Tools** | For domain ownership and resolution history queries. |

## 🔐 Threat Simulation Summary
A simulated partner feed has delivered a mixed set of malicious and benign IOCs.  
Your role is to differentiate legitimate threats from false positives, enrich confirmed malicious indicators,  
and prepare them for operational use in detection and prevention systems.

## 🛡 Blue Team Focus
- Threat intelligence validation workflows.
- IOC enrichment for increased detection fidelity.
- Centralized storage and sharing of intel in a SOC context.
- Leveraging MISP for correlation and automation.

## ⚠️ Disclaimer
This lab uses simulated data for training purposes.  
No real malicious files or live attacks will be executed in your environment.  
All external lookups should be performed on safe, known-clean data unless explicitly permitted for controlled testing.
