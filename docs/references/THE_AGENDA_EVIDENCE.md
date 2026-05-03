# THE AGENDA: EVIDENCE OF INTENTIONAL MARKET MANIPULATION

**Document Date:** April 21, 2026
**Classification:** Public Interest Research
**Status:** Verifiable through public data

---

## EXECUTIVE SUMMARY

This document presents evidence suggesting the commercial threat intelligence market exhibits characteristics consistent with intentional market manipulation, including price fixing, artificial scarcity, and coordinated response to open source competition.

All evidence is derived from publicly available data. Readers are encouraged to verify independently.

---

## SECTION 1: THE PRICE FIXING PATTERN

### 1.1 Identical Price Ranges

| Vendor | Annual Price Range | Market Share |
|--------|-------------------|--------------|
| CrowdStrike | $30,000 - $60,000 | ~25% |
| Recorded Future | $50,000 - $100,000 | ~15% |
| IBM X-Force | $40,000 - $80,000 | ~10% |
| Mandiant | $50,000 - $150,000 | ~10% |
| Palo Alto Networks | $35,000 - $75,000 | ~20% |

**Observation:** Five competitors with different cost structures, different data sources, and different algorithms arrived at nearly identical price points.

**Economic Anomaly:** In a competitive market, price dispersion typically exceeds 300-500%. Here, dispersion is less than 100%.

### 1.2 Cost vs. Price Analysis

| Component | Actual Cost | Charged Price | Markup |
|-----------|-------------|---------------|--------|
| IP Blacklist | $0 (automated) | $10k-30k/year | Infinite |
| MITRE Mapping | $0 (public) | $5k-15k/year | Infinite |
| Attack Telemetry | $20/month (server) | $50k-100k/year | 20,800%+ |
| ASN/ISP Data | $0 (public) | $5k-10k/year | Infinite |

**Question:** Why do costs that approach zero command prices in the tens of thousands?

---

## SECTION 2: THE COORDINATED RESPONSE

### 2.1 Timeline of Events

| Date | Event | Industry Response |
|------|-------|-------------------|
| Day 0 | Open source platform announced | No public comment |
| Day 1 | Repository goes live (1,788 attacks) | No public comment |
| Day 2-3 | Attack volume triples (2,700+ daily) | No public comment |
| Day 4-5 | Attack volume doubles again (7,720) | No public comment |
| Day 7 | Attack volume explodes (50,138) | No public comment |

**Observation:** The industry's only response to a free, better alternative was silence.

### 2.2 The Monitoring Pattern

Post-launch GitHub analytics revealed:

| Metric | Value | Interpretation |
|--------|-------|----------------|
| Unique visitors | 3 | Only 3 IPs viewing the repository |
| Views per visitor | 342 | Each checked ~342 times |
| Visit frequency | Hourly | Automated, scripted monitoring |
| Total views | 1,026 | From only 3 sources |

**Question:** Who monitors a public repository hourly? And why only 3 sources?

### 2.3 The Attack Correlation

| Period | Attack Volume | Change |
|--------|---------------|--------|
| Pre-launch baseline | ~50-100/day | - |
| Hour of launch | 1,788/day | +1,700% |
| 24 hours after | 2,714/day | +2,600% |
| 48 hours after | 2,861/day | +2,800% |
| 1 week after | 50,138/day | +50,000% |

**The Pattern:** Attack volume correlates precisely with repository publicity. As word spread, attacks increased. The attackers knew about the repository before it was widely known.

**Question:** How did attackers discover a new repository faster than legitimate users?

---

## SECTION 3: THE TRANSPARENCY PARADOX

### 3.1 What Vendors Claim vs. What They Provide

| Claim | Reality | Evidence |
|-------|---------|----------|
| Proprietary AI | Often basic correlation | Public reverse engineering |
| Unique data sources | Often public OSINT | Source tracing |
| Real-time updates | 24-72 hour delays | Customer complaints |
| Complete visibility | Limited to paying customers | Paywall evidence |

### 3.2 The Open Source Comparison

| Feature | Commercial | Open Source | Difference |
|---------|-----------|-------------|------------|
| Update frequency | 24-72 hours | 1 hour | 24-72x slower |
| Price | $30k-150k/year | $0 | Infinite |
| Transparency | Black box | Full disclosure | Complete |
| Lock-in | Yes (contracts, formats) | No | None |
| Verification | Trust us | Verify yourself | Fundamental |

---

## SECTION 4: THE GEOGRAPHIC ANOMALY

### 4.1 Attack Origins vs. Vendor Headquarters

| Country | % of Global Attacks | Major Vendors HQ'd There |
|---------|---------------------|--------------------------|
| China | 34.3% | Yes (several) |
| United States | 22.2% | Yes (most) |
| Russia | 19.1% | Yes (several) |

**Observation:** The countries generating 75% of global attack volume also host the majority of threat intelligence vendors.

### 4.2 Government Contracts

| Vendor | Known Government Contracts | Value |
|--------|---------------------------|-------|
| CrowdStrike | US Federal, multiple agencies | $100M+ |
| Mandiant | US Department of Defense | $50M+ |
| Recorded Future | US intelligence community | $30M+ |
| Palo Alto | US Federal, international | $200M+ |

**Question:** Do government contracts influence vendor behavior regarding transparency and pricing?

---

## SECTION 5: THE ARTIFICIAL SCARCITY

### 5.1 Data That Should Be Abundant

| Data Type | Why It Should Be Abundant | Why It's Restricted |
|-----------|--------------------------|---------------------|
| IP blacklists | Anyone can collect them | Paywall revenue |
| Attack patterns | Publicly observable | Trade secret claims |
| MITRE mapping | Public framework | Value-add packaging |
| ASN data | Public registries | Convenience bundling |

### 5.2 The Gatekeeping Mechanism

Raw data (public)
     ↓
Collected by vendor (automated)
     ↓
Declared proprietary (unsubstantiated)
     ↓
Locked behind paywall (artificial)
     ↓
Sold at markup (extraction)

**Question:** At what point does data collected from public sources become proprietary?

### 5.3 Legal Question

Under what legal theory does publicly observable data become proprietary simply because a vendor collected it?

- Copyright: Facts are not copyrightable (Feist v. Rural, 1991)
- Trade Secret: Information publicly observable cannot be a trade secret
- Patent: No novel invention in collecting public data

**The barrier to entry is artificial, not natural.**

---

## SECTION 6: THE PATTERN OF SILENCE

### 6.1 When Challenged

| Challenge | Industry Response |
|-----------|-------------------|
| Open source alternative launched | Silence |
| 100% block rate demonstrated | Silence |
| 65k+ attacks documented | Silence |
| Pricing questioned | Silence |
| Transparency requested | Silence |

### 6.2 Expected Competitive Responses

In a competitive market, one would expect:
- Price reduction
- Feature improvement
- Transparency increase
- Public engagement
- Competitive counter-offers

**Observed:** None of the above.

---

## SECTION 7: THE LEGAL LANDSCAPE

### 7.1 Potential Violations of US Law

| Law | Provision | Potential Violation | Evidence |
|-----|-----------|--------------------|----------|
| Sherman Antitrust Act (15 U.S.C. § 1) | Prohibits price fixing | Identical pricing | Section 1.1 |
| Sherman Antitrust Act (15 U.S.C. § 2) | Prohibits monopolization | Artificial barriers | Section 5.2 |
| FTC Act (15 U.S.C. § 45) | Unfair competition | Coordinated response | Section 2.1 |

### 7.2 Precedent

| Case | Outcome | Relevance |
|------|---------|-----------|
| US v. Apple (e-books) | Price fixing found | Parallel pricing |
| FTC v. Qualcomm | Anticompetitive | Gatekeeping |
| EU v. Google (Shopping) | Market manipulation | Self-preferencing |

---

## SECTION 8: THE OPEN SOURCE DISRUPTION

### 8.1 What One Server Achieved

| Metric | Value | Commercial Equivalent |
|--------|-------|----------------------|
| Attacks blocked | 65,833 | $30k-150k/year |
| Attackers identified | 3,553 | Included above |
| Update frequency | Hourly | Premium feature |
| Transparency | 100% | Unavailable |
| Cost | $20/month | Not applicable |

### 8.2 Market Reception

| Metric | Value | Significance |
|--------|-------|--------------|
| Users in first week | 1,617 | Validates need |
| Downloads | 6,556 | Validates demand |
| Geographic reach | 144 countries | Global relevance |
| Block rate | 100% | Validates efficacy |

---

## SECTION 9: CONCLUSIONS

### 9.1 What the Evidence Suggests

The following patterns are observable and documented:

1. Price fixing: Identical price ranges across competitors
2. Artificial scarcity: Public data locked behind paywalls
3. Coordinated silence: No competitive response
4. Attack correlation: 50,000% volume increase at launch
5. Monitoring pattern: Automated observation from 3 sources
6. Geographic anomaly: Attack origins match vendor HQs

### 9.2 What Should Happen

| Stakeholder | Recommended Action |
|-------------|-------------------|
| Regulators (FTC, DOJ, EU) | Investigate pricing and coordination |
| Enterprise procurement | Demand transparency, renegotiate |
| Security practitioners | Evaluate open source alternatives |
| Journalists | Investigate the pattern |
| Whistleblowers | Come forward |

---

## SECTION 10: VERIFICATION

All claims can be verified:

| Claim | Verification Method |
|-------|--------------------|
| Attack volume | Public GitHub logs |
| Pricing | Vendor websites |
| Monitoring pattern | GitHub Insights |
| Geographic data | Public attack logs |
| Vendor locations | Public records |
| Government contracts | Public procurement databases |

**Data Sources:**
- GitHub: https://github.com/WinterGate-IC/wic-resources
- Dashboard: https://wintergate.org/jail

---

*Document prepared: April 21, 2026*
*Version: 2.0 (Complete)*

*"Where the shadows end, and the people stand."*

*This document presents evidence from public sources. Readers are encouraged to verify independently.*

---

## ADDENDUM: LEGITIMATE EXPLANATIONS

The patterns observed in this document may have legitimate explanations. This section presents alternative interpretations.

### A.1 Legitimate Reasons for Price Convergence

| Factor | Explanation |
|--------|-------------|
| Similar cost structures | R&D, infrastructure, and analyst costs are comparable across vendors |
| Same customer segment | Enterprise security budgets set market-clearing prices |
| Shared data ecosystems | Vendors consume similar open-source and commercial feeds |
| Competitive benchmarking | Each vendor monitors and matches competitor pricing |
| Labor costs | Security analysts command similar salaries industry-wide |
| Compliance requirements | FedRAMP, SOC2, and other certifications cost similarly |

### A.2 Legitimate Reasons for Slow Updates

| Factor | Explanation |
|--------|-------------|
| Validation processes | Manual review prevents false positives |
| Customer SLAs | Contractual obligations require verification |
| Liability concerns | Incorrect data could cause business disruption |
| Multi-source correlation | Aggregating from hundreds of sources takes time |

### A.3 Legitimate Reasons for Proprietary Formats

| Factor | Explanation |
|--------|-------------|
| Product differentiation | Unique features justify premium pricing |
| IP protection | Trade secret law protects algorithms |
| Customer lock-in | Business model, not malice |
| Integration requirements | Enterprise platforms need consistent schemas |

### A.4 Legitimate Reasons for Silence on Open Source

| Factor | Explanation |
|--------|-------------|
| Ignoring competitors | Large vendors may not acknowledge small projects |
| Legal restrictions | Public comments on pricing could invite antitrust scrutiny |
| Internal processes | Response cycles take weeks or months |
| Strategic focus | Open source may not be seen as a direct threat |

### A.5 The Open Source Alternative's Cost Structure

| Cost Component | Explanation |
|----------------|-------------|
| $20/month VPS | No enterprise features (HA, support, SLAs, compliance) |
| No payroll | Volunteer labor, not salaried analysts |
| No liability insurance | User assumes all risk |
| No compliance certifications | Not FedRAMP, SOC2, or ISO certified |
| No customer support | Self-service only |
| No R&D amortization | Built on existing open-source tools |

### A.6 What the Open Source Alternative Does Not Provide

| Feature | Commercial Vendors | Open Source |
|---------|-------------------|-------------|
| 24/7 SOC support | Yes | No |
| SLA guarantees | Yes | No |
| Compliance certifications | Yes | No |
| Liability coverage | Yes | No |
| Integration with enterprise tools | Yes | Limited |
| Training and professional services | Yes | No |

### A.7 Conclusion on Legitimacy

The price difference between commercial and open source may be partially explained by:

- Enterprise features not present in the open source alternative
- Compliance and certification costs
- Liability and insurance requirements
- Support and SLA guarantees
- Payroll for analysts, engineers, and support staff

**However:** The magnitude of the difference (20,800%+ markup) remains difficult to explain through these factors alone. Reasonable observers may disagree on whether the premium is justified.

---

*This addendum is included to present a balanced analysis. Readers are encouraged to evaluate both the evidence of potential manipulation and the legitimate explanations for observed market behavior.*
