# WinterGate IC - Attack Evidence Documentation

**Disclaimer:** This document is for **internal security purposes only** - tracking malicious abuse against our infrastructure. This is NOT doxxing, harassment, or targeting of individuals. This is standard security telemetry collected from automated attack logs.

---

## Incident Summary

On **April 16, 2026**, WinterGate IC detected a coordinated cyberattack targeting our infrastructure, specifically the Safe Haven API endpoint. The attack involved **Command Injection** and **SSH Brute Force** attempts from multiple countries.

**All attacks FAILED. All IPs are permanently blocked.**

---

## Suspected Affiliation

Based on attack patterns, timing, and methods, this appears to be related to:

- **DPOS (Degeneracy Police Order State)** - A known anti-community harassment group
- **SRA (Spam Report Army)** - A coordinated reporting/spam network

**Note:** This is threat intelligence for defensive purposes only.

---

## Primary Attacking IPs (Blocked)

| IP Address | Location | Attack Count | Method |
|------------|----------|--------------|--------|
| `186.233.118.22` | Rio de Janeiro, Brazil | 133+ | Command Injection |
| `191.0.96.73` | Rio de Janeiro, Brazil | 309+ | Command Injection/SSH |
| `189.206.155.253` | Nuevo León, Mexico | 80+ | Command Injection |

---

## Attack Timeline (UTC)

- **00:42:00 - 00:43:10** - Coordinated wave of 100+ attackers
- **Countries involved:** USA, China, Russia, Germany, Japan, Brazil, Mexico
- **Attack types:** Command Injection, SSH Brute Force, SQL Injection

---

## Attack Methods by Country

| Country | Primary Method | Attack Count |
|---------|---------------|--------------|
| United States | SSH Brute Force | 1,706 |
| China | SSH Rapid + Command Injection | 1,232 |
| Russia | Command Injection | 694 |
| Germany | SSH Brute + Command Injection | 385 |
| Japan | SSH Brute Force | 378 |
| Brazil | Command Injection | 56 |
| Mexico | Command Injection | 42 |

---

## All Attacking IPs (Blocked)

*(Full list available in `permanent_blacklist.txt`)*

Total unique attackers blocked: **3,500+**

---

## Detailed Evidence

For complete forensic details including:
- Full attack timeline with millisecond precision
- Accomplice IPs (100+ addresses)
- Command injection payload examples
- Geographic distribution analysis
- ISP and coordinate data for primary attackers

**Please see:** [`attack_evidence_dpos_sra_detailed.txt`](https://github.com/WinterGate-IC/wic-resources/blob/main/evidence/attack_evidence_dpos_sra_detailed.txt)

---

## Evidence Collected

- ✅ Attack logs with timestamps
- ✅ IP geolocation data (public GeoIP databases only)
- ✅ Command injection payloads
- ✅ Coordinated attack patterns

---

## Status

- ✅ All attacks FAILED
- ✅ All IPs permanently blacklisted
- ✅ Infrastructure secure
- ✅ Evidence preserved for defensive purposes

---

*Documentation for internal security telemetry - not intended for harassment or targeting.*

*WinterGate IC - Where the shadows end, and the people stand.*
