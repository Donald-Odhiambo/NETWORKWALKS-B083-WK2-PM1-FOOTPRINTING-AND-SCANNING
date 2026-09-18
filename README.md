# Authorized Footprinting & Network Scanning Assessment

<p align="center">
  <img src="https://img.shields.io/badge/Assessment-Authorized%20Educational-blue?style=for-the-badge" alt="Authorized Educational Assessment">
  <img src="https://img.shields.io/badge/Focus-Reconnaissance%20%26%20Network%20Discovery-green?style=for-the-badge" alt="Reconnaissance and Network Discovery">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Completed">
</p>

<p align="center">
  <strong>NetworkWalks Academy Cybersecurity Internship Programme</strong><br>
  Week 2 | Batch B083
</p>

---

## Project Overview

This project documents an authorized educational cybersecurity assessment completed as part of the NetworkWalks Academy Cybersecurity Internship Programme.

The assessment covered:

- Reconnaissance and footprinting
- DNS and domain information gathering
- Web technology fingerprinting
- HTTP header review
- Web Application Firewall detection
- Public search-engine reconnaissance
- Local network host discovery
- Network topology visualization
- Security observations and recommendations

## Project Documentation

### Full Assessment Report

<p align="center">
  <a href="https://drive.google.com/file/d/1N-Nau5_j6_YSk2wRmvupe3Io3m_Gfmeg/view?usp=sharing">
    <img src="https://img.shields.io/badge/Read%20Full%20Assessment%20Report-4285F4?style=for-the-badge&logo=google-drive&logoColor=white" alt="Read Full Assessment Report">
  </a>
</p>

The full report contains the detailed methodology, evidence, observations, risk analysis, limitations, recommendations, and lessons learned.

### Supporting Evidence

- [View reconnaissance evidence](https://drive.google.com/file/d/123sFguPTMiCoJmABuAs27TpCon6pCoTu/view?usp=sharing)
- [View network discovery evidence](https://drive.google.com/file/d/1AbHHvQfjYI6jQk_yx3a0JZXJ7QtWQaVY/view?usp=sharing)

> Make sure all Google Drive files are set to **Anyone with the link → Viewer** before sharing this repository.

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

## Scope and Ethics

All activities in this project were performed for authorized educational purposes only.

Testing was limited to:

- The approved assessment domain.
- Devices and infrastructure controlled by the assessor.
- The authorized local network.

The following activities were not performed:

- Exploitation.
- Password cracking.
- Credential attacks.
- Denial-of-service testing.
- Malware deployment.
- Persistence.
- Privilege escalation.
- Data modification.
- Unauthorized access.
- Intrusive vulnerability validation.

Do not use the techniques described in this project against systems or networks without explicit written permission.

## Objectives

The objectives of this assessment were to:

- Collect publicly available information about the approved domain.
- Identify domain registration and DNS information.
- Resolve the domain to its associated IP address.
- Identify publicly visible web technologies.
- Review HTTP response headers.
- Check for indicators of a Web Application Firewall.
- Enumerate publicly available DNS records.
- Visualize relationships using Maltego.
- Review publicly indexed information using GHDB.
- Identify active devices on the authorized local network.
- Document available IP and MAC-address information.
- Generate a local network topology diagram.
- Document observations, risks, limitations, and recommendations.

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

Publicly available and low-impact information was collected from the approved domain.

The process included:

- Domain analysis.
- DNS resolution.
- HTTP response review.
- Technology fingerprinting.
- WAF detection.
- Relationship mapping.
- Search-engine reconnaissance.

Detailed reconnaissance evidence is available in the [reconnaissance documentation](https://drive.google.com/file/d/123sFguPTMiCoJmABuAs27TpCon6pCoTu/view?usp=sharing).

### 2. Network Discovery

The local network configuration was first identified using Windows network commands. Zenmap was then used to perform host discovery against the authorized local subnet.

The scan was intended to identify active hosts only. It was not used for exploitation or intrusive vulnerability validation.

View the [network discovery evidence](https://drive.google.com/file/d/1AbHHvQfjYI6jQk_yx3a0JZXJ7QtWQaVY/view?usp=sharing).

### 3. Evidence Collection

Evidence was collected through:

- Command output.
- Screenshots.
- Network topology diagrams.
- Tool results.
- Written observations.

Sensitive or unnecessary information should be sanitized before publication.

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

> These observations are not confirmed vulnerabilities. Further authorized validation would be required.

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

<img width="1536" height="1024" alt="Risk" src="https://github.com/user-attachments/assets/d057c30e-c4d0-4188-90e5-6bda8df84e4c" />


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

- Exploitation.
- Password cracking.
- Credential attacks.
- Denial-of-service testing.
- Malware deployment.
- Persistence.
- Privilege escalation.
- Data modification.
- Unauthorized access.
- Intrusive vulnerability validation.

Technology fingerprints, DNS results, WAF indicators, and search-engine results may be incomplete or may change over time.

## Lessons Learned

- Reconnaissance should precede deeper security testing.
- Different tools provide different views of the attack surface.
- A detected technology or endpoint is not automatically a vulnerability.
- Passive and active reconnaissance have different levels of interaction.
- Network visibility supports asset management and defensive monitoring.
- Evidence, limitations, risk, and recommendations are essential parts of professional security work.
- Authorization must be confirmed before performing security testing.

## Future Improvements

Future versions of this project may include:

- Automated reconnaissance report generation.
- Asset inventory tracking.
- DNS monitoring.
- HTTP security-header comparison.
- Vulnerability validation in a controlled lab.
- Network segmentation analysis.
- Detection engineering using network logs.
- A Python-based reconnaissance documentation tool.

## Author

**Donald Oketch**

Cybersecurity student and aspiring penetration tester.

- LinkedIn: [Donald Oketch](http://www.linkedin.com/in/oketch-donald-odhiambo-0a6823429)
- GitHub: [Donald-Odhiambo](https://github.com/Donald-Odhiambo)
