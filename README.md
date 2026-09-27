# Awesome Exposure Management Platform Ecosystem

*Read this in other languages: [简体中文](README_zh-CN.md)*

**A curated list of top SaaS products & open-source GitHub projects in Exposure Management**

*Focusing on Attack Surface Management (ASM), Vulnerability Prioritization, CAASM, and Remediation.*

**Last Updated: September 2026**

---

This repository tracks prominent **SaaS platforms** and **open-source projects** in the **Exposure Management** domain. These tools assist security teams in unifying risk data across cloud, on-premises, and code environments, validating and prioritizing exposure based on real attack context, and accelerating remediation workflows.

**Featured platforms include:** Tenable One, Qualys TotalCloud, Rapid7 Exposure Command, Wiz, Palo Alto Cortex Exposure Management, Microsoft Security Exposure Management, Armis, Axonius, runZero, and Noetic Cyber.

> [!NOTE]
> **Open Source Landscape:** The open-source ecosystem in Exposure Management is currently in its **early stages**. Commercial SaaS platforms dominate the market with advanced features like attack path analysis and risk contextualization. Open-source solutions primarily focus on point capabilities like **attack surface discovery** (Nmap, OWASP Amass), **vulnerability scanning** (OpenVAS, Nuclei), and **asset discovery**. **XORCISM** is one of the few open-source projects explicitly positioning itself as a unified Exposure Management platform, though it remains in an early stage.

---

## Table of Contents

- [SaaS & Managed Platforms](#saas--managed-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [Building Custom Exposure Management](#building-a-custom-exposure-management-pipeline)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

---

## SaaS & Managed Platforms

| Platform | Key Capabilities & Highlights | Pricing / Free Tier |
| :--- | :--- | :--- |
| **[Tenable One](https://www.tenable.com/)** | AI-driven exposure management platform unifying assets, vulnerabilities, and attack surface data. Features third-party data connectors and custom risk dashboards to identify toxic risk combinations (unpatched vulnerabilities + misconfigurations + excessive permissions). | Commercial quote-based. Demo / trial available upon request. |
| **[Qualys TotalCloud](https://www.qualys.com/)** | CNAPP platform delivering a unified risk view via TruRisk Insights. Includes **Attack Path Analysis** (mapping attack vectors & blast radius) and **Cloud Workflow Automation** (no-code QFlow playbooks for automated remediation). | Commercial quote-based. Free trial available. |
| **[Rapid7 Exposure Command](https://www.rapid7.com/)** | End-to-end vulnerability and exposure management platform featuring a **Remediation Hub** for automated remediation workflows, compensating control evaluation, and third-party integrations (Tenable, Qualys, Wiz). Offers 275+ out-of-the-box integrations and 500+ pre-built workflows. | Commercial quote-based. Free trial available. |
| **[Wiz](https://www.wiz.io/)** | Cloud security platform featuring unified **UVM** (Unified Vulnerability Management) and **ASM** (Attack Surface Management). Uses the Wiz Security Graph to correlate code-to-cloud context and validate external exposure with real exploitability simulation. | Commercial quote-based. Demo available upon request. |
| **[Palo Alto Cortex Exposure Management](https://www.paloaltonetworks.com/)** | Exposure management module within Cortex XDR. Correlates Palo Alto sensors (Cortex Agent, ASM, Network Scanner) with 3rd-party scanners (Qualys, Rapid7, Tenable, CrowdStrike). Features precision filtering and automated remediation content packs. | Commercial quote-based. Demo / trial available. |
| **[Microsoft Security Exposure Management](https://www.microsoft.com/)** | Integrated into the Microsoft Defender XDR portal. Built on an **Enterprise Exposure Graph** to automatically generate **attack paths** and flag critical assets (domain controllers, sensitive databases, privileged roles). | Included with select Microsoft Defender/365 security plans; add-ons vary. |
| **[Armis](https://www.armis.com/)** | Armis Centrix platform powered by an AI asset intelligence engine covering IT, IoT, IoMT, OT, cloud, and mobile assets. Provides AI-driven risk scoring, deduplication, and real-time detection of anomalous behavior and active exploit patterns. | Commercial quote-based. Free trial / demo available. |
| **[Axonius](https://www.axonius.com/)** | Asset cloud platform aggregating 1,000+ data sources into a unified asset data model. Modules cover Cyber Assets, SaaS Applications, Identities, **Exposures** (vulnerability aggregation & prioritization), and Software Assets. **Workflows** automate patch orchestration. | Commercial quote-based. Free trial / demo available. |
| **[runZero](https://www.runzero.com/)** | Cyber Asset Attack Surface Management (CAASM) & network discovery platform featuring uncredentialed scanning. Provides full asset visibility, **Outlier Scoring** (0–5 scale) for unusual assets, and aggregated findings for vulnerabilities and misconfigurations. | **Free Tier:** Community Edition available for up to 256 assets (free forever). Enterprise pricing is quote-based. |
| **[Noetic Cyber](https://www.noeticcyber.com/)** | CAASM platform synthesizing multi-source data to provide a comprehensive view of asset exposure and cyber risk. Integrates with Lansweeper to enhance asset visibility and automate prioritized remediation workflows. | Commercial quote-based. Demo available upon request. |

---

## Open-Source GitHub Projects

- **[XORCISM](https://github.com/XORCISM-AI/XORCISM)**
  One of the few open-source projects explicitly built as a **Unified Exposure Management Platform**. Aligns with NIST CSF 2.0 governance, offers AI-assisted penetration testing capabilities, and computes fused exposure scores. Provides a read-only REST API (`/api/v1/exposures`) for SIEM integration and automation. *(Early-stage project).*

- **[OpenVAS](https://github.com/greenbone/openvas-scanner)**
  Full-featured open-source vulnerability scanner (Greenbone Community Edition). Provides 50,000+ network vulnerability tests with support for authenticated and unauthenticated scanning. Serves as a fundamental **vulnerability discovery engine**.

- **[Nuclei](https://github.com/projectdiscovery/nuclei)**
  Fast and customizable template-based vulnerability scanner developed by ProjectDiscovery. Powered by a community-driven repository covering CVEs, misconfigurations, and exposed panels. Ideal for **continuous attack surface discovery**.

- **[Nmap](https://github.com/nmap/nmap)**
  The de facto standard for network discovery and port scanning. Supports host discovery, service/version detection, and OS fingerprinting. Used as an underlying discovery engine by many security platforms.

- **[OWASP Amass](https://github.com/owasp-amass/amass)**
  In-depth attack surface mapping and domain discovery tool. Performs active and passive reconnaissance to map an organization's external network assets and DNS infrastructure.

- **[Katana](https://github.com/projectdiscovery/katana)**
  Next-generation web crawling and spidering framework designed to discover web application endpoints and hidden assets.

- **[OWASP Dependency-Track](https://github.com/DependencyTrack/dependency-track)**
  Intelligent Software Supply Chain Component Analysis platform that monitors Software Bill of Materials (SBOM) for known vulnerabilities over time.

---

### Additional Open-Source Building Blocks

- **Vulnerability Scanning:** [OpenVAS](https://github.com/greenbone/openvas-scanner), [Nuclei](https://github.com/projectdiscovery/nuclei), [Trivy](https://github.com/aquasecurity/trivy) (containers, code & file systems).
- **Asset Discovery:** [Nmap](https://github.com/nmap/nmap), [OWASP Amass](https://github.com/owasp-amass/amass), [Masscan](https://github.com/robertdavidgraham/masscan) (high-speed port scanner).
- **Exposure Mapping:** [Katana](https://github.com/projectdiscovery/katana) (web crawler), [OWASP ZAP](https://github.com/zaproxy/zaproxy) (DAST).
- **SBOM & Dependencies:** [Dependency-Track](https://github.com/DependencyTrack/dependency-track), [Syft](https://github.com/anchore/syft) (SBOM generation), [Grype](https://github.com/anchore/grype) (vulnerability matcher).

---

### Building a Custom Exposure Management Pipeline

You can assemble a customized exposure management architecture using open-source tools:
1. **Asset & Surface Discovery:** Use **Nmap** + **OWASP Amass** for external attack surface mapping.
2. **Vulnerability Assessment:** Deploy **OpenVAS** + **Nuclei** for infrastructure scanning.
3. **Application & Code Exposure:** Integrate **Dependency-Track** + **Trivy** for supply chain and container risks.
4. **Web Exposure:** Use **Katana** for endpoint crawling.
5. **Data Integration Layer:** Aggregate asset inventories and findings into **PostgreSQL** or **Elasticsearch**.

> [!WARNING]
> Building a custom solution requires manual effort to implement **attack path correlation**, **risk prioritization algorithms**, and **remediation orchestration**, as mature open-source solutions for these specific layers are still emerging.

---

## How to Contribute

1. Fork the repository.
2. Add or update entries in `README.md` following the established format.
3. Include the project/platform name, official link, concise description, and whether it is SaaS or Open-Source.
4. Submit a Pull Request with a brief summary of changes.

If you find this project helpful, feel free to give it a star! ⭐

---

## Disclaimer

- This is a **community-curated list** for educational and research purposes—it is not exhaustive and does not constitute an official endorsement.
- Exposure Management platforms handle sensitive vulnerability and asset data; ensure proper access control and security practices are followed.
- **Open-Source Reality:** Exposure Management remains one of the developing areas in the open-source security ecosystem. Commercial platforms excel in risk prioritization, attack path analysis, and automated remediation. While open-source tools offer robust capabilities at the **discovery and scanning layers**, unified platforms like **XORCISM** are in early development.

---

**Built for Security Engineers, Vulnerability Management Teams, SOC Analysts, and Security Architects.**
