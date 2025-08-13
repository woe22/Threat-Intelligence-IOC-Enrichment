# 01 — IOC Collection and Validation

---

## Scenario

In this module, I collected and validated Indicators of Compromise (IOCs) from safe, lab-provided sources. The goal was to simulate how a SOC analyst reviews, verifies, and records IOCs before they are escalated or used for detections. The examples used were non-malicious and reserved for training purposes.

---

## What I Did

```bash
# Collected sample IOCs (safe examples)
198.51.100.23
203.0.113.77
malicious-demo[.]test
suspicious-svc[.]example

# Refanged domain names for lookup
# Example: malicious-demo[.]test -> malicious-demo.test

# Validated IP addresses
whois 198.51.100.23
dig +short -x 198.51.100.23

# Checked domain WHOIS and DNS
whois malicious-demo.test
dig +short malicious-demo.test

# Created a structured CSV for IOC validation results
# Columns: indicator,type,sources,summary,initial_verdict
```

- Collected IOCs from lab sources and confirmed they were safe examples
- Performed WHOIS lookups and reverse DNS queries on IP addresses
- Checked WHOIS and DNS resolution for domains
- Maintained a structured CSV log of all validation results

---

## What I Learned

- WHOIS and DNS queries are quick ways to verify IOC context and status
- Reserved ranges and test domains are useful for safe training
- Refanging is necessary before any DNS or WHOIS lookups on domains
- Structuring IOC records in CSV format supports repeatability and sharing in SOC workflows

---

## Why It Matters

In real-world SOC operations, raw threat feeds often contain outdated or irrelevant IOCs. Verifying indicators before adding them to detection pipelines helps prevent false positives and wasted effort. This process is a foundational skill for any analyst responsible for triage and threat intelligence validation.

---
