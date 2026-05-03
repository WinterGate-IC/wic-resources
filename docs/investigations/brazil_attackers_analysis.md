# Brazil Attacker Analysis - DPOS/SRA Connection

**Date:** April 19, 2026
**Analyst:** WinterGate IC Threat Intelligence

---

## Summary

Analysis of Brazil-based attackers targeting WinterGate IC infrastructure reveals a concentrated threat from Rio de Janeiro, with one primary attacker showing consistent Command Injection patterns matching known DPOS tactics.

---

## Primary Attacker (Confirmed)

| Attribute | Value |
|-----------|-------|
| IP Address | `186.233.118.22` |
| Location | Rio de Janeiro, Brazil (RJ) |
| ISP | Golden Link (AS266181) |
| Attack Count | 133+ |
| Primary Method | Command Injection |
| Secondary Method | SSH Brute Force, SSH Rapid Attack |
| Risk Score | 50 (MEDIUM) |
| Last Active | 2026-04-16 00:42:59 UTC |
| Role | PRIMARY HAVEN API EXPLOITER |

**Pattern:** Consistent Command Injection attempts targeting API write endpoints. Matches tactics observed in DPOS-coordinated attacks.

---

## Secondary Confirmed IPs

| IP | Location | ISP | Attacks | Method |
|----|----------|-----|---------|--------|
| `191.0.96.73` | Rio de Janeiro, Brazil | V tal (AS7738) | 309+ | Command Injection/SSH |
| `189.206.155.253` | Nuevo León, Mexico | Alestra | 80+ | Command Injection |

*Note: `191.0.96.73` was documented in attack evidence but not currently in the database (may have been purged or rotated).*

---

## Suspicious Brazil IPs (Same Region/ISP Patterns)

The following IPs share geographic proximity or ISP characteristics with confirmed attackers:

### Same ISP (Golden Link - AS266181)

| IP | Location | Risk | Method |
|----|----------|------|--------|
| `186.233.118.22` | Rio de Janeiro | 50 | Command Injection (CONFIRMED) |
| (No other Golden Link IPs currently in database) | | | |

### Same ISP (V tal - AS7738)

| IP | Location | Risk | Method |
|----|----------|------|--------|
| `191.0.96.73` | Rio de Janeiro | N/A | Documented but not in DB |
| `187.107.88.97` | Brazil | 45 | SSH Brute Force |

### Other Brazil IPs with Suspicious Activity

| IP | Location | ISP | Attacks | Method | Suspicion Level |
|----|----------|-----|---------|--------|-----------------|
| `191.101.59.100` | Brazil | Unknown | 5 | Unknown | LOW |
| `187.107.88.97` | Brazil | V tal | 4 | SSH Brute Force | MEDIUM |
| `203.145.34.240` | Brazil | Unknown | 1 | From IPSet | LOW |
| `203.205.37.233` | Brazil | Unknown | 1 | From IPSet | LOW |

---

## Geographic Distribution of Brazil Attackers

- **Rio de Janeiro area**: 2 confirmed attackers (186.233.118.22, 191.0.96.73)
- **Other Brazil regions**: 168 low-volume attackers (1-5 attempts each)
- **Concentration**: The vast majority (99%) of Brazil IPs show only 1 attack

---

## Threat Assessment

### DPOS Connection

The attack patterns observed from Rio de Janeiro IPs match documented DPOS tactics:

| Tactic | Observed |
|--------|----------|
| Command Injection | ✅ Yes |
| Coordinated timing | ✅ Yes (April 16, 00:42-00:43 UTC) |
| Multiple country coordination | ✅ Yes (Brazil, Mexico, US, China, Russia) |
| API targeting | ✅ Yes (Safe Haven API) |

### Suspected Leadership IPs

Based on attack volume, timing, and method:

| IP | Suspicion | Reasoning |
|----|-----------|-----------|
| `186.233.118.22` | HIGH | Primary exploiter, consistent method |
| `191.0.96.73` | HIGH | Highest attack count (309+), documented leader role |
| `189.206.155.253` | MEDIUM-HIGH | Mexican coordinator, significant volume |

---

## Current Status

- ✅ All confirmed attacking IPs permanently blacklisted
- ✅ Command Injection attempts blocked
- ✅ API endpoint secured
- ✅ No successful breaches

---

## Recommendations

1. Monitor Rio de Janeiro IP ranges (186.233.x.x, 191.0.x.x) for new activity
2. Watch for Command Injection attempts from Brazil/Mexico corridors
3. Track ISP patterns (Golden Link, V tal, Alestra) for repeat offenders
4. Update blacklist with any new IPs sharing these characteristics

---

*WinterGate IC - Where the shadows end, and the people stand.*
