# DPOS Leadership IP Analysis

**Subject:** Degeneracy Police Order State (DPOS) - Neo-Nazi Hate COM Clan
**Date:** April 19, 2026
**Classification:** Threat Intelligence - Defensive Purposes Only

---

## Executive Summary

Analysis of attack patterns against WinterGate IC infrastructure on April 16, 2026, reveals coordinated activity consistent with DPOS (Degeneracy Police Order State) and SRA (Spam Report Army) operational tactics. Two IPs from Rio de Janeiro, Brazil, exhibit characteristics suggesting leadership or coordination roles within the attack network.

---

## Suspected Leadership IPs

### Primary Suspect: `191.0.96.73`

| Attribute | Value |
|-----------|-------|
| Location | Rio de Janeiro, Brazil |
| ISP | V tal (AS7738) |
| Attack Count | 309+ |
| Role | SUSPECTED DPOS LEADER / CLAN LEADER |
| Method | Command Injection + SSH Brute Force |
| Confidence | HIGH |

**Justification:**
- Highest attack volume from any Brazil IP
- Coordinated timing with other attackers
- Targeted API endpoints specifically
- Pattern matches documented DPOS tactics

### Secondary Suspect: `186.233.118.22`

| Attribute | Value |
|-----------|-------|
| Location | Rio de Janeiro, Brazil |
| ISP | Golden Link (AS266181) |
| Attack Count | 133+ |
| Role | PRIMARY HAVEN API EXPLOITER |
| Method | Command Injection |
| Confidence | HIGH |

**Justification:**
- Consistent Command Injection attempts
- Same geographic region as primary suspect
- Coordinated attack timing
- ISP different but same city suggests collaboration

---

## Coordination Evidence

| Indicator | Value |
|-----------|-------|
| Attack window | 00:42-00:43 UTC (synchronized) |
| Multiple countries | Brazil, Mexico, US, China, Russia |
| Common method | Command Injection across all primary attackers |
| Target | Safe Haven API endpoint |

---

## DPOS Profile

**Known as:** Degeneracy Police Order State
**Nature:** Neo-Nazi hate COM clan
**Tactics:**
- Coordinated reporting campaigns
- API abuse and exploitation
- Command Injection attempts
- Cross-country attack coordination

**Targeting pattern:** Safe Haven communities, Discord servers, anti-harassment infrastructure

---

## SRA Connection

The Spam Report Army (SRA) appears to have coordinated with DPOS in this attack:
- Rapid-fire SSH brute force patterns
- Mass reporting-style API flooding
- Coordinated timing with DPOS Command Injection attempts

---

## Current Defensive Status

| IP | Status |
|----|--------|
| `191.0.96.73` | Permanently blacklisted (documented, not currently in active DB) |
| `186.233.118.22` | ✅ Permanently blacklisted |
| `189.206.155.253` | ✅ Permanently blacklisted |
| All accomplice IPs | ✅ Permanently blacklisted |

**Result:** All attacks FAILED. Infrastructure SECURE.

---

## Ongoing Monitoring

WinterGate IC continues to monitor:
- Rio de Janeiro IP ranges (186.233.x.x, 191.0.x.x)
- V tal (AS7738) and Golden Link (AS266181) ISP ranges
- Command Injection patterns targeting API endpoints
- Coordinated multi-country attack windows

---

## Legal Note

This documentation is for defensive security telemetry only. IP addresses are publicly routable and were collected from automated attack logs. No personal identifying information is included. All data is used exclusively to protect WinterGate IC infrastructure and partner communities.

---

*WinterGate Intelligence Collective - Where the shadows end, and the people stand.*
