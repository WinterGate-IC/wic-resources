# INVESTIGATION CONCLUSION: Sustained Cyber Attack Campaign Analysis

**Case ID:** WIC-2026-04  
**Investigation Period:** April 12 - April 22, 2026  
**Status:** Active (ongoing)  
**Classification:** Public Disclosure  
**Related Case:** DPOS/SRA Coordinated Attack Investigation

---

## IN-DEPTH EXECUTIVE SUMMARY

This investigation concludes a 9.15-day sustained, coordinated cyber attack campaign targeting open-source threat intelligence infrastructure. The campaign began on April 12, 2026, and remains active at the time of this writing. Total attacks exceeded 75,000 with a peak of 55,524 attacks on a single day (April 21, 2026).

**Campaign Duration:** 9.15 days (219.5 hours)  
**Total Attacks:** 75,000+  
**Peak Daily Attacks:** 55,524 (April 21, 2026)  
**Unique Attackers:** 375+  
**Geographic Origin:** China, Russia, United States (66.61% of all attacks)  
**Primary Vectors:** Command Injection (59.4%), SSH Brute Force (38.9%)  
**Attacker Success Rate:** 0%  

### Context: The DPOS/SRA Connection

This campaign exhibits identical patterns to the previously documented DPOS/SRA coordinated attack investigation. Key similarities include:

- Same-second coordinated attacks across multiple countries
- Precise burst timing (5-10 minute intervals between waves)
- Synchronized attack windows (21:00-23:00 UTC peak)
- Persistent returnees with escalating intensity
- Multi-country orchestration without decentralized botnet patterns

The behavioral signature suggests professional orchestration rather than opportunistic scanning. Attack patterns indicate either a hired botnet service or directly employed attackers with significant resources.

### Professional Attribution Indicators

| Indicator | Evidence | Interpretation |
|-----------|----------|----------------|
| Same-second coordination | 4 countries attacking simultaneously at 18:58:07 UTC | Professional orchestration |
| Sustained duration | 9.15 days continuous activity | Paid campaign (not opportunistic) |
| Escalation pattern | Volume increased 2,000% after public launch | Reactive, targeted response |
| Geographic concentration | 66.61% from 3 countries | Coordinated, not random |
| Persistent returnees | Attackers active 7+ days | Dedicated resources |
| Burst precision | 5-10 minute intervals | Scripted, automated, professional |

### The Hired Botnet Hypothesis

Multiple observations suggest this is a paid service or hired force rather than a single actor:

1. **Multi-country coordination** - Coordinated timing across China, Russia, and US suggests either multiple hired sources or a botnet-for-hire service with global distribution

2. **Professional infrastructure** - 72 attacks per second bursts, same-second timing, and sustained 9-day campaign require significant resources beyond typical hobbyist capabilities

3. **Reactive escalation** - Attack volume precisely tracked repository visibility, indicating real-time monitoring and response typical of paid services with SLAs

4. **Method diversity** - Mix of Command Injection, SSH Brute Force, and burst attacks suggests different tools or teams assigned different vectors

5. **Persistent retry** - Even after port 22 closure, attackers continued targeting the same port without scanning for the new port, suggesting automated scripts that were not updated - common in rented botnet services where customers cannot modify the tooling

### The Economics of the Attack

If this is a hired service, estimated costs:

| Service Type | Estimated Daily Cost | 9-Day Total |
|--------------|---------------------|-------------|
| Basic botnet rental | $500-1,000 | $4,500-9,000 |
| Professional DDoS/botnet | $2,000-5,000 | $18,000-45,000 |
| Coordinated multi-vector | $5,000-10,000 | $45,000-90,000 |

**Someone has spent significant resources attempting to breach a $20/month server.**

### Why They Have Failed

| Security Layer | Implementation | Why It Works |
|----------------|----------------|--------------|
| Port 22 closure | Firewall-level blocking | Automated scripts cannot adapt |
| Password auth disabled | Key-only SSH | Brute force impossible |
| Custom honeypot | Non-standard responses | No known vulnerabilities |
| ipset blacklist | Kernel-level IP blocking | 3,500+ IPs blocked |
| Rate limiting | Per-IP thresholds | Burst attacks mitigated |

### Current Status

At the time of this writing, the attack remains active. In the last 30 minutes alone, 2,313 attacks were recorded from 146 unique attackers. The attackers continue targeting port 22 despite it being closed, suggesting automated scripts that have not been updated.

### The Irony

The attackers have spent an estimated $4,500-$90,000 attempting to breach infrastructure that costs $20/month to operate. Every failed attempt has been logged, analyzed, and published to GitHub for public use. Their attacks have directly contributed to a threat intelligence repository that has been cloned over 6,500 times and is now used by defenders worldwide.

**They are funding their own exposure.**

---

## SECTION 1: CAMPAIGN TIMELINE

### 1.1 Complete Attack Chronology

| Date | Total Attacks | Attackers | SSH Attacks | Phase |
|------|---------------|-----------|-------------|-------|
| April 12 | 3 | 3 | 1 | Baseline |
| April 13 | 58 | 34 | 10 | Baseline |
| April 14 | 93 | 44 | 13 | Baseline |
| April 15 | 2,714 | 200 | 1,621 | Initial Probing |
| April 16 | 2,861 | 190 | 1,451 | Initial Probing |
| April 19 | 1,788 | 56 | 959 | Launch Day Spike |
| April 20 | 7,720 | 106 | 3,024 | Viral Response |
| April 21 | 55,524 | 143 | 21,126 | Peak Assault |
| April 22 | 4,978 | 146 | 1,886 | Post-Hardening |

### 1.2 Campaign Duration

| Metric | Value |
|--------|-------|
| First attack | April 12, 2026 (22:46:20 UTC) |
| Last recorded attack | April 22, 2026 (02:15:30 UTC) |
| Total duration | 9.15 days (219.5 hours) |
| SSH attack duration | 218.5 hours |
| Status | ACTIVE (ongoing) |

---

## SECTION 2: ATTACKER ANALYSIS

### 2.1 Geographic Distribution

| Country | Total Attacks | Attackers | Percentage |
|---------|---------------|-----------|------------|
| China | 19,375 | 91 | 27.03% |
| Russia | 15,635 | 65 | 21.82% |
| United States | 12,730 | 92 | 17.76% |
| Germany | 408 | 28 | 0.57% |
| Japan | 400 | 8 | 0.56% |

Three countries generated 66.61 percent of all attack volume.

### 2.2 Most Persistent Attackers (Active 7+ Days)

| IP (Redacted) | Origin | First Seen | Days Active | Total Attacks |
|---------------|--------|------------|-------------|---------------|
| [REDACTED] | Unknown | April 13 | 8.56 days | 571 |
| [REDACTED] | Unknown | April 13 | 8.44 days | 845 |
| [REDACTED] | Russia | April 14 | 7.85 days | 1,477 |
| [REDACTED] | Russia | April 14 | 7.19 days | 1,139 |

Multiple attackers remained active for over 7 consecutive days, indicating a sustained campaign rather than opportunistic scanning.

### 2.3 Attacker Intensity

| Country | Attacks per Attacker |
|---------|---------------------|
| Russia | 240.54 |
| China | 212.91 |
| United States | 138.37 |

Russian-origin attackers demonstrated the highest intensity, averaging 240 attacks per IP.

---

## SECTION 3: COORDINATION EVIDENCE

### 3.1 Same-Second Multi-Country Attacks

| Timestamp | Countries | Attacks | Attackers |
|-----------|-----------|---------|-----------|
| 2026-04-19 18:58:07 | China, Russia, US, Unknown | 72 | 24 |
| 2026-04-19 19:01:08 | China, Russia, US, Unknown | 68 | 22 |
| 2026-04-15 22:23:40 | China, Russia, US, Germany, Japan | 45 | 7 |

Military-grade coordination across geographic boundaries. The probability of random, uncoordinated attacks producing same-second timing across 4+ countries is statistically negligible.

### 3.2 Peak Attack Window

All three primary attacking nations peaked within the same two-hour window (22:00-23:00 UTC), suggesting coordinated timing rather than independent activity.

| Country | Peak Hour (UTC) | Attacks at Peak |
|---------|-----------------|-----------------|
| China | 22:00 | 2,131 |
| Russia | 23:00 | 1,479 |
| United States | 22:00 | 1,719 |

---

## SECTION 4: THE HIRED BOTNET HYPOTHESIS

### 4.1 Evidence Summary

| Indicator | Evidence | Interpretation |
|-----------|----------|----------------|
| Professional coordination | Same-second timing across 4+ countries | Hired orchestration |
| Sustained duration | 9.15 days continuous | Paid campaign |
| Reactive escalation | Attack volume tracked repository visibility | Professional monitoring |
| Method diversity | Multiple attack vectors simultaneously | Different tools/teams |
| Automated scripts | Continued targeting of closed port 22 | Unmodified rented tooling |

### 4.2 Estimated Cost to Attacker

| Service Type | Estimated Daily Cost | 9-Day Total |
|--------------|---------------------|-------------|
| Basic botnet rental | $500-1,000 | $4,500-9,000 |
| Professional DDoS/botnet | $2,000-5,000 | $18,000-45,000 |
| Coordinated multi-vector | $5,000-10,000 | $45,000-90,000 |

**Estimated total spent to attack a $20/month server: $4,500 - $90,000**

### 4.3 Why a Hired Service?

Multiple observations point to professional-for-hire rather than a single actor:

1. **Multi-country coordination** - Requires either multiple hired sources or a global botnet-for-hire service

2. **Professional infrastructure** - 72 attacks per second bursts require significant resources

3. **Reactive escalation** - Real-time monitoring suggests paid service with SLAs

4. **Method diversity** - Different attack vectors suggest different tools or teams

5. **Unmodified scripts** - Continued targeting of closed port 22 suggests rented tooling that the customer cannot modify

---

## SECTION 5: RESPONSE AND HARDENING

### 5.1 Security Measures Implemented

| Measure | Implementation | Impact |
|---------|----------------|--------|
| Port 22 closure | Firewall-level blocking | 98.2% attack reduction |
| SSH port relocation | Non-standard port | Attackers cannot locate service |
| Password auth disabled | Key-only SSH | Brute force impossible |
| ipset blacklist | Kernel-level IP blocking | 3,500+ IPs blocked |

### 5.2 Impact of Hardening

| Metric | Before | After | Change |
|--------|--------|-------|--------|
| Total attacks (hourly) | 55,263 | 993 | -98.2% |
| SSH attack volume | 21,004 | 375 | -98.2% |
| Attack intensity | 378.51 | 4.4 | -98.8% |
| Maximum burst rate | 72/sec | 27/sec | -62.5% |

---

## SECTION 6: CURRENT STATUS

### 6.1 Ongoing Activity (Last 30 Minutes)

| Metric | Value |
|--------|-------|
| Attacks | 2,313 |
| Active attackers | 146 |
| Most recent | April 22, 2026 (02:15:30 UTC) |

**The attack remains active at the time of this writing.**

### 6.2 Attacker Adaptation

Attackers continue targeting port 22 despite it being closed. No scanning for the new SSH port has been detected. This suggests automated scripts that have not been updated - common in rented botnet services where customers cannot modify the tooling.

---

## SECTION 7: SUCCESS METRICS

| Metric | Value |
|--------|-------|
| Total breach attempts | 75,000+ |
| Successful breaches | 0 |
| Attacker success rate | 0% |
| Infrastructure cost | $20/month |
| Defender success rate | 100% |

---

## SECTION 8: THE IRONY

| Attacker Investment | Defender Investment |
|--------------------|--------------------|
| Estimated $4,500-90,000 | $20/month |
| 9.15 days continuous effort | 4 days initial setup |
| 75,000+ attacks launched | Automated defense |
| 0 successes | 100% block rate |

**The attackers have spent more money attacking the infrastructure than the infrastructure costs to operate.**

---

## SECTION 9: CONCLUSIONS

### 9.1 Key Findings

1. The attack campaign has been active for 9.15 days and remains ongoing
2. Total attacks exceeded 75,000 with a peak of 55,524 in a single day
3. Three countries generated 66.61 percent of all attack volume
4. Attackers demonstrated professional coordination and sustained persistence
5. Evidence suggests a hired botnet service rather than a single actor
6. Estimated attacker expenditure: $4,500 - $90,000
7. Defender success rate: 100%
8. Infrastructure cost: $20/month

### 9.2 Implications

The investigation reveals a coordinated, professional attack campaign with significant resources behind it. The attackers have demonstrated persistence, coordination, and adaptation - yet have failed to achieve any breach. The infrastructure remains uncompromised. The blacklist continues to grow. The intelligence continues to publish.

### 9.3 The DPOS Connection

This campaign exhibits identical patterns to the previously documented DPOS/SRA coordinated attack investigation. The same professional orchestration, same-second timing, and sustained persistence suggest either the same actor or the same hired service provider.

---

## SECTION 10: VERIFICATION

All data in this report can be independently verified:

| Data Source | Location |
|-------------|----------|
| Attack Logs | /trap-logs/latest.md |
| IP Blacklist | /blacklists/permanent_blacklist.txt |
| Live Dashboard | https://wintergate.org/jail |
| DPOS Investigation | /evidence/ (repository) |

---

*Document prepared: April 22, 2026*  
*Data current as of: April 22, 2026 (02:30 UTC)*  
*Case ID: WIC-2026-04*  
*Status: Active - Ongoing*

*"Where the shadows end, and the people stand."*

*This report concludes the investigation into a sustained 9.15-day cyber attack campaign. The attack remains active. All data is verifiable through public sources.*
