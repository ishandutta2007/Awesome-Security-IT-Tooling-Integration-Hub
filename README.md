# Awesome-Security-IT-Tooling-Integration-Hub

# Awesome Security & IT Tooling Integration Hub

> A curated list of top Security and IT Tooling Integration Hub platforms — both SaaS/Hosted commercial solutions and open-source alternatives for connecting security tools, IT operations, and identity systems into automated workflows.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Druva Marketplace](#druva-marketplace)
  - [MuleSoft Anypoint Platform](#mulesoft-anypoint-platform)
  - [Boomi Connect](#boomi-connect)
  - [Workato](#workato)
  - [Celigo](#celigo)
  - [Jitterbit Harmony](#jitterbit-harmony)
  - [SnapLogic](#snaplogic)
  - [Zapier](#zapier)
  - [Make](#make)
  - [Microsoft Power Automate](#microsoft-power-automate)
- [Open-Source Software](#-open-source-software)
  - [Apache Camel](#apache-camel)
  - [WSO2 Micro Integrator](#wso2-micro-integrator)
  - [Prismatic Components Library](#prismatic-components-library)
  - [n8n](#n8n)
  - [ConnectKit](#connectkit)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Security and IT Tooling Integration Hub platforms. These are not open-source but are included as reference points for feature comparison.

### Druva Marketplace
**Type:** Data protection-native integration hub for security and IT ecosystems
Druva's Marketplace serves as the central integration hub for the Druva Data Security Cloud, explicitly designed to bridge data protection with the broader IT and security stack [citation:1]. It offers pre-built integrations for **Security & SIEM** (Splunk, Microsoft Sentinel, CrowdStrike), **Identity Management** (Okta, Entra ID), **ITSM & Operations** (ServiceNow, Slack), and **Legal & Compliance** (OpenText), alongside API-driven custom integration capabilities [citation:2][citation:11]. The integration center also includes webhooks for real-time event-driven automation, allowing external services to be triggered when events occur in Druva [citation:10]. **Key distinction:** This is not a general-purpose iPaaS—it is a purpose-built integration layer for organizations already using Druva for data protection, connecting backup and security telemetry to the tools security and IT teams already operate.
**Best for:** Druva customers wanting to activate their data protection platform within SIEM, ITSM, and identity workflows without building custom integrations from scratch.

### MuleSoft Anypoint Platform
**Type:** Enterprise iPaaS with extensive prebuilt connector library
MuleSoft Anypoint Platform offers hundreds of prebuilt, certified connectors for SaaS apps (Salesforce, SAP), cloud platforms (AWS, Azure), databases, and AI technologies, with support for REST, SOAP, and event-driven architectures [citation:3][citation:12]. A key differentiator is the **Anypoint Exchange** marketplace, where custom connectors can be shared and certified. For security and IT tooling specifically, MuleSoft provides AI Connectors for MCP and A2A integration, enabling governed AI agent access to enterprise systems [citation:3]. **Trade-off:** Enterprise pricing and complexity typically target organizations with dedicated integration teams.
**Best for:** Large enterprises needing a mature, governed iPaaS with the broadest certified connector library and AI agent connectivity via MCP.

### Boomi Connect
**Type:** Managed MCP connector service for governed AI access
Boomi Connect is a managed service that exposes **1,000+ IT-governed tools** across major enterprise applications to AI assistants (Claude, Copilot, Gemini) via the Model Context Protocol [citation:4][citation:13]. It is explicitly built for the security and IT tooling use case: full OAuth pass-through preserves individual user permissions, organization-level credentials centralize API key management, and **CISO-ready observability** logs every tool invocation, user, and workflow for audit [citation:13]. **Key distinction:** Boomi Connect solves the governed connectivity problem for AI agents, not traditional system-to-system integration—it lets knowledge workers access enterprise tools through AI without IT losing control.
**Best for:** Security-conscious organizations wanting to enable AI assistant access to enterprise systems with granular access control, audit trails, and user-level permission mapping.

### Workato
**Type:** Enterprise iPaaS with MCP and agent orchestration
Workato provides **1,200+ pre-built connectors** alongside data pipelines, API management, and master data management on a single platform, named a Leader in the 2026 Gartner Magic Quadrant for iPaaS [citation:5]. For security and IT tooling, Workato packages recipes, APIs, and existing MCP servers as governed MCP servers that any MCP-compatible agent can call, with every agent action authenticated, authorized, and auditable from one console [citation:5]. Compliance coverage includes SOC 2, ISO 27001, ISO 42001, HIPAA, PCI, and DORA [citation:5]. **Trade-off:** Quote-only pricing, with MCP and agent tooling reserved for upper editions.
**Best for:** Enterprises wanting a mature iPaaS with strong governance and native MCP packaging for AI agent access to security and IT systems.

### Celigo
**Type:** Integration platform with on-premises connectors and AI assistance
Celigo provides **1,000+ pre-built connectors** for business apps, marketplaces, ERPs, and trading partners, with a hybrid deployment model that includes on-premises connectivity [citation:6]. The Ora conversational assistant helps build and troubleshoot automations, with Celigo claiming 96% of exceptions resolve without manual intervention. Security features include MFA, role-based access controls, audit visibility, and SOC 2 compliance [citation:6]. **Trade-off:** Web platform only, with quote-based pricing for Standard, Professional, and Enterprise editions.
**Best for:** Organizations needing broad business system connectivity with on-premises support and AI-assisted automation building.

### Jitterbit Harmony
**Type:** Unified platform with API management, EDI, and MCP
Jitterbit Harmony combines iPaaS, API Manager, App Builder, and EDI with enterprise-grade **Model Context Protocol (MCP)** support, allowing existing APIs and integrations to be transformed into secure, governed, reusable capabilities for AI agents [citation:7]. It is ISO 42001 certified for responsible AI, with hybrid security based on NIST, CISA, and CERT frameworks. Prebuilt integrations with LLMs (OpenAI, Azure OpenAI, Google Gemini, Amazon Bedrock) prevent vendor lock-in [citation:7]. **Trade-off:** Enterprise-focused, with a median time-to-go-live of 1.74 months.
**Best for:** Organizations wanting a single platform spanning traditional integration, API management, and governed AI agent access with strong security certifications.

### SnapLogic
**Type:** Agentic integration platform with OEM/embedded capabilities
SnapLogic offers **1,000+ pre-built connectors** called Snaps, with a cloud-native iPaaS architecture extended to AI agents through MCP [citation:8]. Its OEM/Embedded Program allows ISVs and MSPs to embed the integration layer within their own products, with white-labeling options. Security certifications include SOC 3, SOC 2 Type 2, HIPAA, and SAML SSO [citation:8]. **Trade-off:** The OEM model targets product teams rather than internal IT integration.
**Best for:** ISVs and MSPs wanting to embed a proven integration layer with AI agent connectivity into their own security or IT products.

### Zapier
**Type:** No-code automation with enterprise governance
Zapier provides 7,000+ app integrations with enterprise security features including SOC 2 Type II, SSO (SAML 2.0 + SCIM), role-based access, and domain capture [citation:29]. For AI safety, **AI Guardrails** scan AI steps for PII, prompt injection, and toxicity, with configurable block/route/detect actions, while agent permissions control which apps and actions are available per user, team, and workspace . Audit logs record every AI and agent action . **Trade-off:** Per-task pricing can become expensive at volume; AI governance features are builder-opted rather than default-on.
**Best for:** Teams wanting broad app connectivity with accessible AI governance and audit capabilities without deep integration expertise.

### Make
**Type:** Visual automation with enterprise governance and MCP
Make provides a visual canvas with **3,000+ app connectors**, AI Agents that live within the canvas, and an MCP Server that exposes active scenarios as callable tools for external LLMs (Claude, ChatGPT) [citation:24]. Enterprise features include on-prem agent for local network access, SSO (OAuth2/SAML2), audit logs for user actions, GDPR/SOC 3/SOC 2 Type II compliance, and role-based access with process operations spend limits [citation:30]. **Important security consideration:** Make's HTTP module has no built-in domain allowlist, and webhook payloads have no built-in input validation—AI SAFE2 framework documentation explicitly flags these as injection and SSRF vectors requiring external controls [citation:24].
**Best for:** Teams wanting a flexible visual automation platform with MCP exposure and enterprise governance, accepting the need for additional security controls on webhook and HTTP modules.

### Microsoft Power Automate
**Type:** Low-code automation with Microsoft ecosystem integration
Power Automate provides hundreds of connectors to Microsoft and third-party services, with a visual designer and integration into the broader Microsoft 365 and Power Platform ecosystem. Sentinel solutions exist for monitoring Power Platform and Dynamics 365 activity, providing analytics rules and hunting queries for security teams [citation:25]. **Best for:** Microsoft-centric organizations wanting security and IT tooling integration within their existing Microsoft investments.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Security and IT Tooling Integration tools. The open-source ecosystem spans **code-first integration frameworks**, **visual automation platforms**, and **AI agent connectivity libraries**.

### Apache Camel
**Stack:** Java / YAML / XML | **License:** Apache-2.0
Apache Camel is a mature, code-first integration framework with **350+ components**, based on Enterprise Integration Patterns (EIP) [citation:26]. For security and IT tooling specifically, Camel offers multiple security layers: **Route Security** via Shiro or Spring Security policies, **Payload Security** via XML Security and Crypto data formats for encryption/decryption, **Endpoint Security** via Jetty/CXF/Netty SSL and authentication, and **Configuration Security** via Jasypt for encrypting sensitive properties [citation:20]. Routes can be written in Java, YAML, or XML, with Camel K for Kubernetes and Camel Karavan for low-code visual design. **Trade-off:** Requires Java development expertise; you build and maintain the integration logic yourself.
**Best for:** Java teams wanting a battle-tested, Apache-governed integration framework with strong built-in security primitives and no vendor lock-in.

### WSO2 Micro Integrator
**Stack:** Java | **License:** Apache-2.0
WSO2 MI is a cloud-native integration runtime with a comprehensive **MI Connector Library** covering security-relevant systems including LDAP, Jira, ServiceNow, Salesforce, and database connectors [citation:22][citation:28]. The connector library is actively maintained with both handwritten connectors and those generated from Ballerina packages. WSO2 MI is positioned as an open-source alternative to MuleSoft, booting in seconds with native Prometheus metrics and Kubernetes-native design. **Trade-off:** You run the platform yourself; requires Kubernetes/SRE capability for production.
**Best for:** Organizations with Kubernetes expertise wanting an open-source integration runtime without MuleSoft's lock-in and cost structure.

### Prismatic Components Library
**Stack:** TypeScript | **License:** Apache-2.0 (reference library)
Prismatic open-sourced its **entire library of pre-built Application Connector and Data Platform components** under Apache-2.0 in June 2026 [citation:19]. The repository is available on GitHub and automatically synchronizes with Prismatic's internal source code on every release. **Important caveat:** This is a **reference library** rather than a community-maintained open-source project—external pull requests are not accepted, and modified versions are maintained by the customer [citation:19]. The value is in production-grade connector code that developers can read, fork, and extend as a starting point for custom integrations, particularly for AI-assisted development workflows.
**Best for:** Developers building custom security or IT integrations who want production-grade connector code as a reference, accepting that they maintain any modifications themselves.

### n8n
**Stack:** TypeScript / Node.js | **License:** Sustainable Use (source-available)
n8n is the most widely adopted source-available workflow automation platform, with a visual builder, 400+ integrations, and JavaScript/Python code nodes. The community has produced extensive **security automation workflow collections** covering red team, blue team, SOC, and DFIR use cases—including threat intel ingestion, IOC enrichment, SIEM-to-Slack alert routing, EDR noise taming, phishing auto-triage, and cloud config drift monitoring [citation:21][citation:27]. **Important:** The Sustainable Use License is source-available but not OSI-approved; internal self-hosting is permitted. **Trade-off:** Security workflows are community-contributed and vary in quality; no built-in enterprise governance features comparable to commercial iPaaS.
**Best for:** Technical security teams wanting a self-hostable automation platform with a rich community library of security workflows, accepting the source-available licensing terms.

### ConnectKit
**Stack:** Python | **License:** Open Source
ConnectKit gives AI agents access to user SaaS accounts (Gmail, Calendar, Drive, GitHub, Slack, and **520+ more**) through one YAML file per service, with OAuth, API keys, token vault, and tool discovery handled automatically [citation:9]. It runs **entirely on-device** with an encrypted SQLite credential vault and local YAML specs—no cloud APIs or hosted auth services. It supports both CLI and MCP adapter backends, with per-user credential isolation and self-hosted support [citation:9]. **Trade-off:** Designed for AI agent connectivity rather than system-to-system integration; it is a library you embed in your own agent tooling.
**Best for:** Developers building AI agents that need governed access to user SaaS accounts without a cloud dependency, particularly for security operations or IT support agents.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Connector Library | Security Focus | MCP/AI Agents | Self-Hosted | Best For |
|----------|---------|-------|-------------------|----------------|---------------|-------------|----------|
| **Druva Marketplace** | Proprietary | Cloud | Pre-built + API | ✅ SIEM/ITSM/IdP | (API) | ❌ | Druva data protection integration |
| **MuleSoft** | Proprietary | Cloud | Hundreds certified | (Enterprise) | ✅ AI Connectors | ❌ | Enterprise iPaaS + governance |
| **Boomi Connect** | Proprietary | Cloud | 1,000+ managed tools | ✅ CISO observability | ✅ MCP-native | ❌ | Governed AI agent access |
| **Workato** | Proprietary | Cloud | 1,200+ | ✅ SOC/ISO portfolio | ✅ MCP packaging | ❌ | Enterprise iPaaS + agent governance |
| **Celigo** | Proprietary | Cloud/hybrid | 1,000+ | ✅ MFA/RBAC/SOC2 | (Ora assistant) | ❌ | Business systems + on-prem |
| **Jitterbit** | Proprietary | Cloud | 1,000+ (EDI) | ✅ ISO 42001 | ✅ MCP | ❌ | Unified integration + AI governance |
| **SnapLogic** | Proprietary | Cloud | 1,000+ Snaps | ✅ SOC/HIPAA | ✅ MCP | ❌ | OEM/embedded integration |
| **Zapier** | Proprietary | Cloud | 7,000+ | ✅ AI Guardrails | ✅ MCP | ❌ | Broad connectivity + AI safety |
| **Make** | Proprietary | Cloud | 3,000+ | (Requires external controls) | ✅ MCP | ❌ | Visual automation + MCP |
| **Apache Camel** | Apache-2.0 | Java | 350+ components | ✅ Security layers | (Custom) | ✅ | Code-first secure integration |
| **WSO2 MI** | Apache-2.0 | Java | Comprehensive library | ✅ LDAP/ITSM/CRM | ✅ MCP (Inbound) | ✅ | Open-source MuleSoft alternative |
| **Prismatic** | Apache-2.0 | TypeScript | Reference library | (Connector code) | (AI-assisted) | ✅ (Fork) | Connector code reference |
| **n8n** | Sustainable Use | TypeScript | 400+ + community | ✅ Community workflows | (Custom) | ✅ | Security automation workflows |
| **ConnectKit** | Open Source | Python | 520+ SaaS | (Agent access) | ✅ MCP-native | ✅ | AI agent SaaS connectivity |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Security or IT Tooling Integration Hub that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with n8n). Note that the ecosystem **splits** between **purpose-built security/IT integration hubs** (Druva Marketplace for data protection ecosystems), **general-purpose enterprise iPaaS with security governance** (MuleSoft, Boomi Connect, Workato, Jitterbit), and **open-source frameworks** (Apache Camel for code-first security integration, WSO2 MI for a MuleSoft alternative, n8n for community security workflows). **Boomi Connect** and **Workato** are notable for explicitly solving the governed AI agent access problem via MCP, while **Apache Camel** remains the strongest open-source choice for teams needing built-in security primitives (route policies, payload encryption, endpoint security) in their integration layer [citation:20].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
