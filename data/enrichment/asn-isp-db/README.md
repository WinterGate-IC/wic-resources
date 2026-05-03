# WinterGate ASN/ISP Threat Intelligence Database

This database contains Autonomous System (ASN) and Internet Service Provider (ISP) threat intelligence gathered from real attack data against WinterGate infrastructure.

## Database Contents

| File | Description |
|------|-------------|
| `asn_database.md` | Complete ASN threat ranking (top 100) |
| `isp_database.md` | Complete ISP threat ranking (top 100) |
| `asn_by_country.md` | Geographic distribution of ASN threats |
| `asn_isp_db.json` | Machine-readable JSON format |
| `master_isp_asn.csv` | Raw IP to ISP/ASN mapping |

## Current Statistics

| Metric | Value |
|--------|-------|
| Total ASNs Tracked | 102 |
| Total ISPs Tracked | 68 |
| Total Attackers | 3528 |
| ASN Coverage | 71.1% |

## Usage Examples

### Download Top ASNs
```bash
curl https://raw.githubusercontent.com/WinterGate-IC/wic-resources/main/asn-isp-db/asn_database.md
```

### Query Specific ASN
```bash
curl https://raw.githubusercontent.com/WinterGate-IC/wic-resources/main/asn-isp-db/master_isp_asn.csv | grep "AS13335"
```

### Get JSON Data
```bash
curl https://raw.githubusercontent.com/WinterGate-IC/wic-resources/main/asn-isp-db/asn_isp_db.json
```

---

*Data collected from real attacks. Updated continuously as new threats are detected.*
