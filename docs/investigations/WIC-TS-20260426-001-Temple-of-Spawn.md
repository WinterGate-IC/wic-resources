# WINTERGATE INTELLIGENCE COLLECTIVE
## Formal Findings: Trust & Safety Violation

**Case ID:** WIC-TS-20260426-001
**Date:** April 26, 2026
**Status:** CONFIRMED / ACTION TAKEN

---

## 1. EXECUTIVE SUMMARY

This document serves as the formal record of findings regarding the removal of a previously designated Trusted Space and its associated account from the WinterGate Intelligence Collective ecosystem.

The decision was based on direct evidence linking the space to an ongoing, coordinated cyberattack campaign targeting WIC infrastructure.

---

## 2. THE CLAIM MADE BY THE REMOVED PARTY

Within their own Terms of Service channel, the group made the following claim:

> *"On Roblox, the most popular spawnist game was unmoderated and com clans + nazis would run rampant in it, so they wanted to make their own game/community that was actually moderated and not a cashgrab like that one so spawnists wouldn't be subject to harassment and grooming."*

**Summary of Claim:** Their community was created as a genuinely moderated, safe alternative to an unmoderated, harmful environment.

---

## 3. THE ALLEGATION SUPPORTED BY WIC EVIDENCE

WinterGate Intelligence Collective does not dispute the desire for a moderated safe space. However, the actions observed directly contradict the claim of responsible moderation.

**Allegation:** The space was not actively moderated against malicious actors, and the server owner had prior knowledge of attack coordination occurring across both Discord and X (Twitter) platforms.

---

## 4. THE IRONY: EVIDENCE OF CONTRADICTION

| The Claim | The Evidence |
|-----------|--------------|
| "Actually moderated" | A malicious Discord invite link was posted on **X (Twitter)** by attacker `bleedo / returningtsert` on **April 15, 2026** and remained active for **16 days** during an active cyberattack campaign against WIC. |
| "Safe space for spawnists" | The Temple of Spawn server owner (`nevs ⛧ [SPWN]`) admitted prior knowledge of the malicious actors (`bleedo`, `yesoma`) by name. |
| "Not affiliated with attackers" | The X post containing the malicious link was removed **ONLY AFTER** WIC reported the issue to `nevs`, not during the 16-day attack window. This demonstrates `nevs` has direct influence over the attacker's X account. |
| "No control over external platforms" | The attacker's X post was removed following communication with `nevs`, proving coordination between the server owner and the attacker. |

---

## 5. THE SUSPICIOUS REMOVAL TIMELINE

| Date | Event |
|------|-------|
| April 15, 2026 | Attacker `bleedo / returningtsert` posts malicious Discord invite link on X |
| April 15-26, 2026 | Link remains active; attack campaign escalates (199,596 attempts) |
| April 15, 2026 | Haven Trust development environment accessed; attacker claims "breach" |
| April 26, 2026 | WIC formally reports the issue to Temple of Spawn owner `nevs ⛧ [SPWN]` |
| April 26, 2026 (immediate) | X post is **REMOVED** |

**Critical Finding:** The X post was removed **only after** WIC reported to `nevs`, not before, despite the 16-day attack window. This strongly indicates coordination between the server owner and the attacker.

---

## 6. OWNER'S ADMISSIONS & BEHAVIOR

When confronted, `nevs ⛧ [SPWN]` stated:

- *"i already have bleedo, yesoma, and all their associates i know of banned from my server"*
- *"im not in it since bleedo doesnt like me"*

**Analysis of Behavior:**

| Behavior | Interpretation |
|----------|----------------|
| Admitted prior knowledge of `bleedo` | Confirmed awareness of the attacker |
| Acknowledged `bleedo` by name | Knew the exact individual behind the attack |
| X post removed after report to `nevs` | Demonstrates direct influence over attacker |
| Claimed "not in it" | Contradicted by ability to get X post removed |
| Created server name distinction | Attempt at plausible deniability ("Temple" vs "Tempel") |

**Conclusion:** The server owner has direct influence over the attacker and used that influence to remove evidence **only after being caught**, not in good faith.

---

## 7. FORENSIC EVIDENCE CORRELATION

During the same 16-day window (April 10 - April 26, 2026), WIC infrastructure was subjected to:

| Metric | Value |
|--------|-------|
| Total Attacks | 199,596 |
| Primary Attacking IP | 207.180.222.68 (Contabo VPS) |
| Attack Methods | SSH Brute Force (T1110), Command Injection (T1202) |
| APT Patterns Detected | APT28, APT29, Lazarus (90% confidence) |
| Successful Breaches | 0 |

The X post was shared on **April 15**. The attack campaign escalated on **April 15-16** and continued through **April 26**. The post was removed **only after** WIC reported to `nevs`.

---

## 8. THE HAVEN TRUST INCIDENT

| Attribute | Detail |
|-----------|--------|
| Incident Date | April 15, 2026 |
| Target | Haven Trust API (development environment) |
| Attacker | `bleedo / returningtsert` |
| Attacker Claim | "breach" via unsecured admin panel |
| Actual Access | Development environment only |
| WIC Response | Database restored from backup (minutes) |
| Vulnerability | Patched immediately |
| Attacker's Video Evidence | Archived by WIC |
| Attacker's X Post | Tagged WIC; archived |
| **Status** | **TERMINATED / CONTAINED / NO PRODUCTION IMPACT** |

The attacker's "breach" claim was exaggerated. No production data was accessed. No user data was exposed. The environment was restored and secured within minutes.

---

## 9. RISK ASSESSMENT

| Factor | Score (0-100) | Justification |
|--------|----------------|---------------|
| Prior Knowledge of Malicious Actors | 95 | Owner admitted knowing `bleedo` by name |
| Delay in Taking Action | 95 | Link remained active for 16 days during attack |
| Influence Over Attacker | 90 | X post removed only after report to owner |
| Attempt at Cover-Up | 90 | Removal timing indicates evidence suppression |
| Potential Attack Vector Validity | 85 | Server hosted coordination discussion |
| Risk to WIC Community | 82 | Active attack coordination linked to space |

**Overall Risk Level:** HIGH

---

## 10. ACTION TAKEN BY WIC

- Trusted Space designation revoked (**Temple of Spawn**)
- User account removed from WIC ecosystem (**nevs ⛧ [SPWN]**)
- Formal notification sent to the server owner
- Evidence archived to GitHub for public record
- Abuse report filed with hosting provider (Contabo)
- Public trust & safety announcement published
- Attacker's failed "breach" claim publicly refuted with archived evidence

---

## 11. DISPOSITION

| Metric | Result |
|--------|--------|
| Total attacks blocked | 199,596 (100%) |
| Successful breaches | 0 |
| Data loss | 0 |
| Service disruption | 0 |
| Haven Trust production impact | 0 |
| Attacker infrastructure | REPORTED / PENDING TERMINATION |
| X post coordination link | REMOVED (only after report to owner) |
| Trusted Space | REVOKED |
| Owner account | REMOVED |
| Evidence | ARCHIVED PUBLICLY |

---

## 12. CONCLUSION

The removed party claimed to provide a "moderated safe space." The evidence demonstrates:

1. A malicious coordination link remained active for 16 days during an active cyberattack against WIC
2. The server owner (`nevs ⛧ [SPWN]`) admitted prior knowledge of the attacker (`bleedo`) by name
3. The X post was removed **only after** WIC reported to the owner, not during the 16-day attack window
4. The owner has direct influence over the attacker's X account, contradicting claims of "not being involved"
5. The removal timing strongly indicates evidence suppression, not good faith moderation

**The removal was not based on ideology. It was based on:**

- Demonstrated failure of moderation
- Direct link to an active cyberattack campaign
- Owner's prior knowledge of malicious actors
- Suspicious removal timing indicating cover-up
- Measurable risk to community safety

**The decision stands.**

---

**Issued By:**
WinterGate Intelligence Collective
Security & Trust Division

`Stat crux dum volvitur orbis`

---

## ATTACHMENTS

- Complete forensic evidence (GitHub)
- MITRE ATT&CK mapping
- Abuse report to Contabo
- Haven Trust incident evidence (video + X post)
- X public disclosure record
- Discord trust announcement (Temple of Spawn revocation)
- Formal notice to nevs ⛧ [SPWN]
- Full Discord conversation log
- X post removal timeline analysis
- Evidence of owner's influence over attacker's X account
- Group association documentation (DPOS, Enclave, UTTP, Spawniism, SRA)
