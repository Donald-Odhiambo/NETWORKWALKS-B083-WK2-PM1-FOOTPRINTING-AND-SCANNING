# NETWORKWALKS-B083-WK2-PM1-FOOTPRINTING-AND-SCANNING

# Authorized Footprinting and Network Scanning Assessment

This project documents an authorized educational cybersecurity assessment completed as part of the NetworkWalks Academy Cybersecurity Internship Programme.

The assessment covered:

- Reconnaissance and footprinting
- DNS and domain information gathering
- Web technology fingerprinting
- HTTP header review
- WAF detection
- Public search-engine reconnaissance
- Local network host discovery
- Network topology visualization
- Security observations and recommendations

## Disclaimer

All activities in this project were performed for authorized educational purposes only.

Testing was limited to:

- The approved assessment domain
- Devices and infrastructure controlled by the assessor
- The authorized local network

No exploitation, credential attacks, denial-of-service testing, malware deployment, persistence, privilege escalation, or unauthorized access was performed.

Do not use these techniques against systems or networks without explicit written permission.

## Project Information

| Field | Details |
|---|---|
| Program | NetworkWalks Cybersecurity Internship |
| Batch | B083 |
| Week | 02 |
| Project | Footprinting and Network Scanning |
| Assessment type | Authorized educational security assessment |
| Assessment date | 17 September 2026 |
| Report version | 1.0 |
| Tester | Donald Oketch |

## Objectives

The objectives of this assessment were to:

1. Collect publicly available information about the approved domain.
2. Identify domain registration and DNS information.
3. Resolve the domain to its associated IP address.
4. Identify publicly visible web technologies.
5. Review HTTP response headers.
6. Check for indicators of a Web Application Firewall.
7. Enumerate publicly available DNS records.
8. Visualize relationships using Maltego.
9. Review publicly indexed information using GHDB.
10. Identify active devices on the authorized local network.
11. Document available IP and MAC-address information.
12. Generate a local network topology diagram.
13. Document observations, risks, limitations, and recommendations.

## Tools Used

| Tool | Purpose |
|---|---|
| Kali Linux | Security testing environment |
| WHOIS | Domain registration analysis |
| WhatWeb | Web technology fingerprinting |
| nslookup | DNS resolution |
| curl | HTTP header review |
| Wafw00f | WAF detection |
| DNSRecon | DNS record enumeration |
| Maltego | Relationship and infrastructure mapping |
| GHDB | Search-engine reconnaissance |
| Zenmap/Nmap | Local network discovery |
| Windows Command Prompt | Local network configuration |

## Methodology

### 1. Reconnaissance

Publicly available and low-impact information was collected from the approved domain. The process included domain analysis, DNS resolution, HTTP response review, technology fingerprinting, WAF detection, relationship mapping, and search-engine reconnaissance.

### 2. Network Discovery

The local network configuration was first identified using Windows network commands. Zenmap was then used to perform host discovery against the authorized local subnet.

The scan was intended to identify active hosts only. It was not used for exploitation or intrusive vulnerability validation.

### 3. Evidence Collection

Evidence was collected through command output, screenshots, topology diagrams, and written observations. Sensitive or unnecessary information should be sanitized before publication.

## Key Observations

The assessment identified the following observations:

- Publicly detectable web technologies were present.
- Domain and DNS infrastructure information was publicly observable.
- The domain resolved to a public hosting address.
- HTTP response information and a WordPress REST API path were observable.
- A possible ModSecurity WAF indicator was detected.
- DNS, mail, and service records could be reviewed publicly.
- Relationships between domain and infrastructure components could be visualized using Maltego.
- Multiple active hosts were discovered on the authorized local network.
- A network topology diagram was generated using Zenmap.

These observations are not confirmed vulnerabilities. Further authorized validation would be required.

## Risk Summary

| Observation | Preliminary Risk |
|---|---|
| Publicly detectable web technology information | Medium |
| Public IP address exposure | Low |
| Technical HTTP information exposure | Low |
| Detectable WAF technology | Low |
| Publicly enumerable DNS infrastructure | Medium |
| Multiple active local network devices | Medium |
| Possible search-engine exposure | Medium |
| Public infrastructure relationships | Low/Medium |

<img width="1513" height="1600" alt="Piechart_Risk" src="https://github.com/user-attachments/assets/ab78fc74-368d-4bba-b928-e7e3b1cfb057" />


## Recommendations

### Web Application Security

- Keep WordPress, plugins, themes, and supporting components updated.
- Remove unused plugins and themes.
- Maintain an accurate software inventory.
- Review whether detailed version information needs to be publicly exposed.
- Compare observed technologies with official security advisories.

### HTTP Security

- Review unnecessary server and framework disclosure headers.
- Configure appropriate security headers.
- Review publicly accessible WordPress API responses.
- Ensure administrative functions require strong authentication and authorization.

### DNS and External Attack Surface

- Remove obsolete DNS records and unused subdomains.
- Review SPF, DKIM, and DMARC configuration.
- Restrict DNS zone transfers.
- Maintain an inventory of public-facing assets.
- Periodically review publicly exposed services.

### WAF and Monitoring

- Keep the WAF enabled and updated.
- Monitor blocked and allowed requests.
- Tune WAF rules to reduce false positives.
- Harden the origin server in addition to using a WAF.
- Conduct future WAF testing only with written authorization.

### Local Network Security

- Maintain an approved inventory of local devices.
- Investigate unknown or unexpected hosts.
- Disable unused services and interfaces.
- Segment sensitive devices where possible.
- Use strong Wi-Fi security and administrator credentials.
- Repeat authorized discovery scans periodically.

## Limitations

This project was limited to reconnaissance and host discovery.

The following activities were not performed:

- Exploitation
- Password cracking
- Credential attacks
- Denial-of-service testing
- Malware deployment
- Persistence
- Privilege escalation
- Data modification
- Unauthorized access
- Intrusive vulnerability validation

Technology fingerprints, DNS results, WAF indicators, and search-engine results may be incomplete or change over time.

## Lessons Learned

- Reconnaissance should precede deeper security testing.
- Different tools provide different views of the attack surface.
- A detected technology or endpoint is not automatically a vulnerability.
- Passive and active reconnaissance have different levels of interaction.
- Network visibility supports asset management and defensive monitoring.
- Evidence, limitations, risk, and recommendations are essential parts of a professional security report.
- Authorization must be confirmed before performing security testing.

## Future Improvements

Future versions of this project may include:

- Automated reconnaissance report generation
- Asset inventory tracking
- DNS monitoring
- HTTP security-header comparison
- Vulnerability validation in a controlled lab
- Network segmentation analysis
- Detection engineering using network logs
- A Python-based reconnaissance documentation tool

## Author

Donald Oketch

Cybersecurity student and aspiring penetration tester.

- LinkedIn: (www.linkedin.com/in/oketch-donald-odhiambo-0a6823429)
- GitHub: [Donald-Odhiambo](https://github.com/Donald-Odhiambo)
