# BREACH ATTEMPT ANALYSIS: What They Actually Want

**Date:** April 22, 2026
**Issued By:** WinterGate Intelligence Collective
**Data Source:** 73,421 attack records

---

## EXECUTIVE SUMMARY

This is not a DDoS. This is a coordinated, persistent breach campaign.

**Key Findings:**

| Finding | Value |
|---------|-------|
| Breach attempts | 98.9% of all attacks |
| DDoS attempts | 0.9% of all attacks |
| Primary target | SSH access (98.7%) |
| Primary methods | Command Injection (59.4%), SSH Brute Force (38.9%) |
| Attacker success rate | 0% |

---

## WHAT THEY WANT

### Target Analysis

| Target | Attempts | Percentage |
|--------|----------|------------|
| SSH Access | 72,482 | 98.7% |
| Other | 939 | 1.3% |

**They want direct access to the server. Period.**

### Attack Classification

| Classification | Attempts | Percentage | Intent |
|----------------|----------|------------|--------|
| Code Execution (Breach Attempt) | 44,059 | 60.01% | Take control |
| Credential Theft (Breach Attempt) | 28,551 | 38.89% | Gain access |
| DDoS / Rate Attack | 662 | 0.9% | Disruption |
| Reconnaissance | 40 | 0.05% | Mapping |

**98.9% of all attacks are directed at breaching the system.**

---

## HOW THEY TRY

### Method Breakdown

| Method | Attempts | Percentage | What It Does |
|--------|----------|------------|--------------|
| Command Injection | 43,615 | 59.4% | Execute arbitrary code on server |
| SSH Brute Force | 28,551 | 38.89% | Guess passwords to gain access |
| SSH Rapid Attack | 662 | 0.9% | Rate-based disruption |
| SQL Injection | 444 | 0.6% | Database manipulation |

### By Country

| Country | Primary Method | Secondary | Strategy |
|---------|---------------|-----------|----------|
| China | Command Injection (70.3%) | SSH Brute (28.4%) | Code execution first |
| Russia | Command Injection (50.8%) | SSH Brute (47.5%) | Balanced approach |
| United States | Command Injection (69%) | SSH Brute (28.7%) | Code execution first |

---

## WHEN THEY ATTACK

### Time Distribution (UTC)

| Time Period | Attempts | Percentage |
|-------------|----------|------------|
| Evening (18-23) | 27,291 | 37.17% |
| Night (00-05) | 18,227 | 24.83% |
| Morning (06-11) | 15,604 | 21.25% |
| Afternoon (12-17) | 12,299 | 16.75% |

**Peak attacks occur during evening UTC hours, coordinated across time zones.**

---

## SUCCESS RATE

| Metric | Value |
|--------|-------|
| Total breach attempts | 72,610 |
| Successful breaches | 0 |
| Success rate | 0% |

**Every single attempt failed.**

---

## WHAT THIS MEANS

### They Are Not Trying to DDoS

| Evidence | Conclusion |
|----------|------------|
| Only 0.9% rate-based attacks | Not a volume attack |
| 98.9% code execution + credential theft | Targeted breach attempt |
| 72,482 attempts on SSH | Specific goal: access |

### They Want Control

| If They Succeeded | What Would Happen |
|-------------------|-------------------|
| Command Injection success | Full server compromise |
| SSH Brute Force success | Persistent backdoor access |
| Either success | Server becomes part of botnet |

### They Are Coordinated

| Evidence | Implication |
|----------|-------------|
| Same-second timing across countries | Military-grade coordination |
| Persistent returnees (77%) | Dedicated campaign |
| Method preferences by country | Specialized roles |

---

## CONCLUSION

The attackers are not trying to knock the server offline.

They are trying to **get in**.

Every command injection is an attempt to execute code. Every SSH brute force is an attempt to steal credentials. Every attack is aimed at gaining persistent access.

**They have failed 73,421 times.**

The server remains uncompromised. The blacklist keeps growing. The data keeps publishing.

They want in. They cannot get in.

---

## VERIFICATION

All claims can be independently verified:

| Data Source | Location |
|-------------|----------|
| Attack Logs | /trap-logs/latest.md |
| IP Blacklist | /blacklists/permanent_blacklist.txt |
| Live Dashboard | https://wintergate.org/jail |

---

*Document prepared: April 22, 2026*
*Data current as of: April 22, 2026*

*"Where the shadows end, and the people stand."*

*73,421 attempts. 0 successes. The math speaks for itself.*
