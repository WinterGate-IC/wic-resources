# WINTERGATE INTELLIGENCE COLLECTIVE · OFFICIAL RESOURCE REPOSITORY

## Overview

The WinterGate Intelligence Collective (WIC) is an open-source threat intelligence platform dedicated to identifying, tracking, and mitigating cyber threats targeting civil society, independent media, and human rights defenders. This repository serves as the central hub for all WIC resources, including intelligence reports, investigation data, threat feeds, configuration files, and automation scripts.

**Mission:** Where the shadows end, and the people stand.

This repository contains declassified threat intelligence, incident reports, campaign analysis, MITRE ATT&CK mappings, IP blacklists, enrichment data, and forensic evidence collected from our global honeypot network. All data is provided for research, defensive security, and threat hunting purposes.

---

## Repository Status

**Current state:** Fully reorganized and actively maintained.

All assets have been moved into a logical, categorized structure for easier navigation. Some datasets (IP blacklists, enrichment databases) are published directly here, while live real-time threat intelligence is served from our main infrastructure due to GitHub storage limitations.

---

## Repository Structure

- docs/ - Reports and analysis
  - threat-intel/ - Intelligence summaries and assessments
  - investigations/ - Detailed incident investigations
  - analysis/ - Campaign and pattern analysis
  - incidents/ - Incident response reports
  - references/ - External reference materials
  - learning/ - Learning resources and documentation
  - validation/ - MITRE ATT&CK validation reports
  - inventory/ - Asset inventory and tracking
  - abuse/ - Provider abuse reports
  - hardening/ - Security hardening documentation

- data/ - All data assets
  - archives/ - Historical attack archives (72h rolling + monthly)
  - blacklists/ - IP blacklists (published here)
  - enrichment/ - ASN, ISP, country, and IP range databases
  - forensic/ - Forensic evidence and collected data
  - exports/ - Data exports from various sources
  - signatures/ - Detection signatures and rules
  - trap-logs/ - Real-time trap logs (historical)
  - enriched/ - Enriched IP data

- configs/ - Configuration files
  - tiered_response/ - Tiered response configurations

- mitre-data/ - MITRE ATT&CK framework data

- scripts/ - Automation and utility scripts

---

## Live Intelligence Data Access

Real-time threat intelligence is served from our secure infrastructure:

| Resource | URL |
|----------|-----|
| Latest Threat Report | https://wintergate.org/intel/latest.md |
| Attackers JSON | https://wintergate.org/intel/attackers.json |
| IP Blacklist | https://wintergate.org/intel/permanent_blacklist.txt |
| 72-Hour Archives | https://wintergate.org/intel/archives/72h/ |
| Monthly Archives | https://wintergate.org/intel/archives/monthly/ |

**API Documentation:** https://wintergate.org/docs/api/

---

## Published Datasets in This Repository

- **IP Blacklists:** `/data/blacklists/` - Plain text format, one IP per line
- **Enrichment Data:** `/data/enrichment/` - ASN, ISP, country, IP range databases
- **MITRE Data:** `/mitre-data/` - Complete MITRE ATT&CK framework
- **Signatures:** `/data/signatures/` - Detection signatures and rules
- **Forensic Evidence:** `/data/forensic/` - Collected forensic data
- **Attack Archives:** `/data/archives/` - Historical attack data

---

## Note on Live Data

Live threat intelligence data is served from https://wintergate.org/intel/ due to GitHub storage limitations for large, frequently updating datasets. This repository contains static resources, published blacklists, documentation, configurations, and historical archives.

Future WIC services will integrate with this structure as the primary resource hub.

---

## Related Services

- Main Website: https://wintergate.org
- Cyber Jail: https://wintergate.org/jail
- Safe Havens: https://wintergate.org/safe-havens.html
- Datasets Hub: https://wintergate.org/datasets.html
- DOCMAN API: https://wintergate.org/docs/api/

---

## License & Usage

All data and code in this repository are provided for defensive security research, threat hunting, and educational purposes. Proper attribution is appreciated but not required.

---

**WinterGate Intelligence Collective · Where the shadows end, and the people stand.**
