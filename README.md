# Awesome-Identity-Threat-Detection-n-Response

Top Identity Threat Detection & Response (ITDR) Tools Ecosystem

Curated List of SaaS Products & Open-Source GitHub Projects
Focused on Credential Compromise Detection, Lateral Movement Prevention, Privilege Abuse Detection & Identity Attack Path Analysis
Last updated: September 2026

This repository tracks notable SaaS platforms and open-source projects for Identity Threat Detection & Response (ITDR). These tools help security teams detect identity-based attacks, stop lateral movement, identify over-privileged accounts, and cut attack paths before attackers can exploit them.

Examples include Silverfort, Beyond Identity, Permiso, Semperis, Quest One Identity, Microsoft Defender for Identity, CrowdStrike Falcon Identity, SentinelOne Singularity Identity, Proofpoint Identity Threat Defense, Huntress Managed Identity, BeyondTrust, Delve Labs, Netwrix, and Veza (the category leaders).

Open-source emphasis: This section is heavily expanded with every major active project for self-hosting, custom detection logic, and transparent identity security workflows — ideal for security teams that need deep visibility into identity risk without vendor lock-in or agent-heavy deployments.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

Table of Contents

SaaS/Hosted Platforms

Open-Source GitHub Projects

How to Contribute

Disclaimer

SaaS/Hosted Platforms

Silverfort
Unified identity protection platform that extends MFA and threat detection across all corporate resources, including legacy and on-premises systems. Agentless enforcement.

Beyond Identity
Passwordless identity platform with ITDR capabilities. Uses device-bound credentials and continuous authentication to detect account takeover attempts.

Permiso
Identity threat detection for cloud infrastructure. Detects anomalous activity across AWS, Azure, GCP, Okta, and GitHub by normalizing cross-cloud logs -
2
.

Semperis
Identity protection for Active Directory and Entra ID. Provides attack path analysis, ransomware recovery, and real-time threat detection for hybrid identity environments.

Quest One Identity
Identity governance and privileged access management with ITDR capabilities. Detects and responds to identity-based threats across AD and cloud directories.

Microsoft Defender for Identity
Cloud-based identity threat detection for AD and Azure AD. Monitors on-premises signals to detect lateral movement, privilege escalation, and compromised credentials.

CrowdStrike Falcon Identity Protection
Identity threat detection integrated into the Falcon platform. Detects credential compromise, privileged account abuse, and lateral movement with threat intelligence correlation -
1
.

SentinelOne Singularity Identity
AI-powered identity security with ITDR. Detects credential-based attacks, suspicious authentication patterns, and identity-based lateral movement.

Proofpoint Identity Threat Defense
Identity threat detection and response (formerly ObserveIT). Focuses on insider threat detection, session recording, and privileged user monitoring.

Huntress Managed Identity
Managed identity threat detection for SMBs and MSPs. Provides continuous monitoring of AD and Entra ID for compromise indicators.

BeyondTrust
Privileged access management platform with identity threat analytics. Detects anomalous privileged activity and credential abuse.

Delve Labs
Identity threat detection platform focused on detecting misconfigurations and over-privileged accounts across cloud and on-premises identities.

Netwrix
Identity and data security platform with ITDR capabilities. Detects suspicious activity in AD, Entra ID, and file systems.

Veza
Identity security platform with access graph technology. Maps effective permissions across cloud and on-premises systems to identify privilege escalation paths.

Open-Source GitHub Projects

Open-ITDR (Authomize)
Open solutions from Authomize for identity threat detection and response. Python-based toolkit for detecting identity-based threats -
12
.

P0LR Espresso (Permiso)
Open-source framework for normalizing cloud runtime logs across AWS, GCP, Azure, Okta, and GitHub. Unifies identity, IP, user agent, and action fields into a consistent schema for faster threat investigation during live response -
2
.

AI Access Sentinel
ITDR platform with ML-powered anomaly detection, UEBA, risk scoring, and role mining. Features 6-factor risk scoring model (ML detection, peer comparison, high-value resource access, auth failures, rule breaches, CrowdStrike intel), Falcon ITDR webhook integration, and role discovery via ML clustering -
1
.

Identity Threat Hunter (ITH)
Cloud-native identity security analytics platform built on Google Cloud Run and Elastic Cloud with Vertex AI enrichment. Detects impossible travel, risky logins, and lateral movement with AI-generated risk explanations -
18
.

Idryx
Identity Security Graph unifying humans, service accounts, keys, and AI agents in one graph. Features 27 detectors across ITDR/NHI/agents/least-privilege, per-identity baselining, delegation graph resolution with cycle protection, Agent-BOM (CycloneDX-shaped), and alert delivery to Slack/SIEM/OTLP -
7
.

Mantissa Stance
Agentless cloud security platform with CIEM (Cloud Infrastructure Entitlement Management) engine. Features 37 collectors across AWS, GCP, and Azure, 300+ YAML policies, attack path analysis, blast radius calculation, and natural language query interface. Deterministic core with no ML for detection -
6
.

KIEMPossible (Palo Alto Networks)
Kubernetes Identity and Entitlement Management toolkit. Detects risky RBAC permissions including wide secret access, nodes/proxy access, serviceaccount token creation, escalate/bind/impersonate permissions, and CSR certificate issuing -
11
.

Paralus
CNCF Sandbox project for controlled, audited access to Kubernetes infrastructure. Features SSO/OIDC integration, just-in-time service account creation, dynamic permission revocation, and real-time audit logs for threat identification -
9
.

BloodHound
The standard for Active Directory attack path mapping. Turns AD data into a graph and finds shortest paths to Domain Admin. Defenders run it to find and cut attack paths before attackers do. SharpHound collects data; BloodHound visualizes -
19
.

AD-PathFinder (NetSPI)
Attack path mapping for AD, ADCS, SCCM, and MSSQL using BloodHound CE + OpenGraph data. Surfaces attack paths from low-privileged users to Domain Admins with password audit integration and HTML reports -
8
.

bloodtrail
BloodHound enhancement toolkit for Active Directory attack path discovery. Features attack chain detection (Exchange WriteDACL → DCSync, GenericAll → Password Reset, Backup Operators → NTDS.dit), password reuse analysis, and compound workflows -
3
.

redpath
Active Directory attack path mapper with minimum-cost paths and remediation priority. Single-purpose, scriptable, self-hostable with JSON/table/SARIF output for CI integration -
14
.

Apache Syncope
Full-fledged IAM system covering provisioning, reconciliation, reporting, access management, and API management. Features identity provisioning, governance, SSO, MFA, and SCIM support -
10
.

Perun
Identity and access management system covering the whole user lifecycle. Features virtual organization management, user/group management, resource management, and service management in distributed and federated environments -
5
.

Additional Strong Open-Source Options

Attack Path Analysis: BloodHound + AD-PathFinder, bloodtrail, redpath for AD attack path discovery and remediation prioritization.

Cloud Identity Security: P0LR Espresso (log normalization), Mantissa Stance (CIEM/attack paths), KIEMPossible (Kubernetes RBAC analysis).

UEBA & ML Detection: AI Access Sentinel (6-factor risk scoring), Identity Threat Hunter (Elastic + Vertex AI enrichment).

Identity Governance: Apache Syncope, Perun for provisioning, reconciliation, and access reviews.

Kubernetes Identity: Paralus (CNCF Sandbox), KIEMPossible for K8s identity and entitlement management.

Frameworks for building custom systems: Combine BloodHound or AD-PathFinder for AD attack path analysis, P0LR Espresso for cloud log normalization, AI Access Sentinel for ML-powered detection, and Idryx for identity graph unification. Add Elastic Security or OpenSearch for alerting and dashboards.

How to Contribute

Fork the repo.

Add/edit entries in README.md (follow existing format).

Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

Submit PR with a short explanation.

Star the repo if you find it useful!

Disclaimer

This is a community-curated list — not exhaustive and not an endorsement.

ITDR tools require access to sensitive authentication and identity data; ensure compliance with privacy regulations and internal security policies.

Attack path tools (BloodHound, AD-PathFinder) generate sensitive reconnaissance data — treat output as confidential and secure it appropriately.

Made for SOC analysts, identity security engineers, red teamers, and security architects.
Let's make identity threat detection more open, graph-driven, and proactive.
