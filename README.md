## Cyber Threat Intelligence (CTI) Analysis & MITRE ATT&CK Mapping Lab

### Overview
This repository documents a hands-on Cyber Threat Intelligence (CTI) laboratory
focused on threat classification, MITRE ATT&CK mapping, and intelligence-driven
forensic analysis.

The activity was developed as part of the
Digital Forensics & Cyber Threat Intelligence microcredential (Week 6).

The original reports were written in Portuguese, as the course was taught in Portuguese.
This repository aims to demonstrate analytical reasoning, structured threat intelligence,
and professional reporting methodology in a controlled academic context.

---

### Objectives
- Understand the Cyber Threat Intelligence (CTI) lifecycle
- Distinguish between Strategic, Tactical, Operational, and Technical intelligence
- Map real-world attacks to the MITRE ATT&CK framework
- Correlate attacker behavior with forensic artefacts
- Identify Indicators of Compromise (IoCs) and attacker TTPs
- Analyze real CTI advisories and threat reports
- Support forensic investigations using intelligence-driven approaches

---

### Lab Scope & Methodology

The laboratory consists of two main activities:

Activity A – MITRE ATT&CK Mapping
A real-world cyberattack case study was analyzed and mapped to the MITRE ATT&CK
framework. The attack narrative was broken down into phases, techniques, and
sub-techniques.

Activity B – Threat Actor Profiling (CTI Advisory Analysis)
A CTI advisory was analyzed to identify:
- Threat actor profile
- Victim sectors
- Initial access vectors
- Malware and tooling
- MITRE ATT&CK techniques
- Campaign objectives and motivation

---

## CTI Types Covered

### Strategic Intelligence
- High-level analysis focused on threat trends, actor motivations, and geopolitical impact
- Used for risk assessment and security decision-making at management level

### Tactical Intelligence
- Analysis of adversary Tactics, Techniques, and Procedures (TTPs)
- Mapped to the MITRE ATT&CK framework
- Supports detection engineering and forensic investigations

### Operational Intelligence
- Information about active campaigns, infrastructure, and attack timelines
- Supports threat hunting and incident response

### Technical Intelligence
- Indicators of Compromise (IoCs), including:
  - IP addresses
  - Domains
  - File hashes
- Used for detection, enrichment, and triage

---

## MITRE ATT&CK Mapping (Activity A)

The analyzed attack was decomposed into the following phases:

1. Initial Access
   - Technique: T1078 – Valid Accounts
   - Evidence: Compromised VPN credentials

2. Discovery / Credential Access
   - Technique: T1552.001 – Credentials in Files
   - Evidence: PowerShell script containing hard-coded credentials

3. Privilege Escalation
   - Technique: T1555 – Credentials from Password Stores
   - Evidence: Access to privileged access management (PAM) secrets

4. Lateral Movement
   - Techniques: T1021 / T1078
   - Evidence: Use of valid accounts to access critical systems

5. Exfiltration
   - Technique: T1567 – Exfiltration Over Web Services
   - Evidence: Download of internal data via web services

6. Persistence (Inference)
   - Possible Techniques: T1053 / T1547
   - Included as investigative hypotheses due to lack of explicit evidence

### Each technique includes:
- Evidence source
- Forensic artefacts to collect
- Example commands and logs
- Confidence level (High / Medium)

---

## Threat Actor Profiling (Activity B)

A CTI advisory was analyzed to identify:

### Threat Actor
- Ransomware group using double extortion tactics

### Motivation
- Financial gain

### Victim Sectors
- Critical infrastructure
- Healthcare
- Technology
- Government
- Enterprise services

### Initial Access Vectors
- Drive-by compromise (T1189)
- Social engineering with malicious PowerShell execution (T1204.004)

### Malware & Tools Identified
- Cobalt Strike
- SystemBC
- Interlock RAT
- NodeSnake RAT
- Lumma Stealer
- Berserk Stealer
- AzCopy
- WinSCP

---

### Forensic & Intelligence Value

This activity demonstrates how CTI enhances forensic investigations by:
- Guiding evidence collection
- Prioritizing artefact analysis
- Correlating technical indicators with adversary behavior
- Distinguishing confirmed facts from analytical inferences

---

### Ethical Considerations

- All analysis was performed using public reports and academic materials
- No live systems or real victims were targeted
- Activities were conducted strictly for educational purposes
- The objective is to improve defensive and investigative capabilities

---
