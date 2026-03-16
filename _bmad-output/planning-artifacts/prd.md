---
stepsCompleted: [step-01-init, step-02-discovery, step-02b-vision, step-02c-executive-summary, step-03-success, step-04-journeys, step-05-domain, step-06-innovation, step-07-project-type, step-08-scoping, step-09-functional, step-10-nonfunctional, step-11-polish, step-12-complete]
completedAt: '2026-03-15'
status: complete
inputDocuments:
  - _bmad-output/planning-artifacts/product-brief-Stack-Breach-2026-03-11.md
workflowType: 'prd'
classification:
  projectType: saas_b2b
  domain: cybersecurity_compliance
  complexity: high
  projectContext: greenfield
briefCount: 1
researchCount: 0
brainstormingCount: 0
projectDocsCount: 0
---

# Product Requirements Document - Stack-Breach

**Author:** Glademellor
**Date:** 2026-03-15

## Executive Summary

Stack-Breach is a SaaS compliance monitoring platform that detects unauthorized AI usage across company tools and generates audit-ready reports, purpose-built for mid-size companies (50–500 employees) without dedicated compliance teams. As AI tool adoption accelerates across every department — marketing, sales, support, HR — companies accumulate regulatory exposure they cannot see: HIPAA violations in healthcare, SOC 2 failures in financial services, data leakage across all sectors. Enterprise platforms capable of detecting this cost $50K+/year, leaving mid-size companies underserved. Stack-Breach fills this gap at $200–$500/month, starting with the highest-risk detection vectors (browser extensions and outbound API calls to AI providers) and expanding to enforcement.

**Target users:** IT Managers and Security Analysts at mid-size companies who own compliance responsibility without dedicated security staff. Budget approvers are VPs or Directors focused on risk reduction and audit outcomes. External auditors are the primary consumers of the platform's report output.

**Why now:** AI tool proliferation is outpacing every organization's ability to track it manually. Regulatory scrutiny is accelerating. The window to build a detection moat — before enterprise players trickle down or new point solutions emerge — is now.

### What Makes This Special

Stack-Breach is not a general security tool repurposed for AI detection. Three sources of sustainable differentiation:

1. **Network-effect detection library** — Each monitored customer enriches detection accuracy for all customers. Shadow AI detection data is sparse and fragmented; aggregating it at scale creates a moat requiring years of customer volume to replicate.
2. **Auditor-ready output from day one** — Reports are structured for compliance auditors, not engineers. The gap between IT discovery and regulatory reporting is where mid-size companies fail. Stack-Breach bridges it without a dedicated compliance team.
3. **Founding team domain credibility** — Co-founded by an engineering manager (Glade Mellor) with real-world tool adoption expertise and a CISSP-certified IT Security Champion (Gary Van Sluis) with deep compliance knowledge. Built from operational reality, not theoretical frameworks.

## Project Classification

| Field | Value |
|---|---|
| **Project Type** | SaaS B2B |
| **Domain** | Cybersecurity / Compliance Tech |
| **Complexity** | High — multi-tenant architecture, industry-specific compliance rules, regulated data, network-level detection, audit-grade reporting |
| **Project Context** | Greenfield |

## Success Criteria

### User Success

- **Setup completion:** IT Manager (non-specialist) completes full configuration within one business day with remote founding team support — no security expertise required
- **Time to first detection:** First violations surfaced within 48 hours of setup completion
- **Audit report utility:** Comprehensive compliance report generated on demand in minutes, formatted to auditor standards — no manual investigation required
- **Detection trust:** False positive rate low enough that flagged violations are consistently actionable — users act on alerts rather than ignoring them
- **Primary success moment:** User discovers shadow AI usage they didn't know existed and successfully hands a Stack-Breach report to an auditor who confirms it meets their requirements

### Business Success

- **Beta customer acquisition:** 10–20 paying beta customers onboarded within 90 days of launch
- **Trial-as-business-case:** Trial results (violations surfaced within 48 hours) serve as the internal business case for purchase — no formal proposal required
- **Detection moat initiation:** Each new customer begins contributing data to the detection library, establishing the network-effect flywheel early

### Technical Success

- **Detection accuracy:** ≥90% of unauthorized AI tools correctly identified across monitored environments
- **Data isolation:** Complete row-level tenant isolation — zero cross-tenant data exposure
- **Known AI provider coverage:** All major AI API endpoints (OpenAI, Anthropic, Google AI, and equivalents) detected at launch
- **Compliance rule accuracy:** Industry-specific rule presets (HIPAA, SOC 2) correctly map violations to specific regulatory requirements
- **Report integrity:** Audit reports accurately reflect detected violations with no omissions or misattributions

### Measurable Outcomes

| Outcome | Metric | Target |
|---|---|---|
| Detection accuracy | % shadow AI tools correctly identified | ≥90% |
| False positive rate | % flagged items that are not actual violations | Low enough that users trust and act on alerts |
| Customer acquisition | Paying beta customers | 10–20 within 90 days of launch |
| Time to first detection | Hours from setup to first violation surfaced | ≤48 hours |
| Setup completion time | Hours from signup to fully configured monitoring | ≤1 business day |
| Trial-to-paid conversion | % trial users who become paying customers | TBD — validated in beta |
| Audit report utility | Customers who successfully use report in a real audit | ≥1 in beta period |
| Customer retention | Monthly churn rate | TBD — validated in beta |

## Project Scoping & Phased Development

### MVP Strategy & Philosophy

**MVP Approach:** Revenue MVP — the goal is 10–20 paying beta customers within 90 days, not just validated learning. The trial experience must deliver a business case fast enough (48 hours to first violation) that customers convert without a formal sales cycle. Every scope decision is evaluated against this constraint.

**Resource constraint:** Two-person founding team (Glade + Gary) handling product, engineering, sales, and customer success. Manual processes (provisioning, onboarding, support) are acceptable substitutes for automated systems in MVP.

### MVP Feature Set (Phase 1)

**Must-Have Capabilities:**

| Capability | Rationale |
|---|---|
| Browser extension monitoring agent | Highest-risk detection vector |
| Outbound API call detection | Covers Zapier/integration scenarios; second highest-risk vector |
| AI provider endpoint library | Core of detection; covers all major providers at launch |
| Violation detail: tool + data + regulation | Without this, alerts are noise, not intelligence |
| Dashboard with risk severity | Primary interface for IT Manager daily use |
| Configurable rule engine with industry presets | HIPAA and SOC 2 presets required for target industries |
| Per-tenant rule customization | Required for Security Analyst power-user journey |
| Audit report generation (PDF) | The product's primary value output |
| Regulation-mapped report structure | Required for auditor journey |
| Row-level tenant data isolation | Non-negotiable security requirement |
| Manual tenant provisioning | Founding team handles; no self-service needed at MVP |
| Chrome Enterprise / MDM deployment support | Required for managed device environments |
| Network proxy compatibility | Common customer environment pattern |

**Out of MVP Scope:**

| Feature | Deferral Rationale |
|---|---|
| Self-service trial signup and provisioning | Manual onboarding sufficient for ≤20 beta customers |
| Real-time alerting | Periodic scanning sufficient; real-time adds infrastructure complexity |
| Slack / GSuite / M365 integrations | Phase 2; browser + API covers highest-risk vectors |
| Active enforcement / blocking | Requires policy maturity customers don't have yet |
| Department head notifications | Post-MVP |
| Executive dashboard | Audit report serves this purpose in MVP |
| API access / SIEM integrations | Phase 2/3 |
| GDPR / PCI-DSS / additional frameworks | HIPAA and SOC 2 sufficient for initial target industries |

### Phase 2: Growth (post first 20 customers)

- Self-service trial signup and automated tenant provisioning
- Real-time alerting on new violations
- Slack, Google Workspace, Microsoft 365 detection surface expansion
- Third-party SaaS embedded AI feature detection
- Additional compliance frameworks (GDPR, PCI-DSS)
- Executive dashboard with risk trend charts
- Department head notification system
- API access and CSV/JSON export for GRC tool integration

### Phase 3: Expansion (after product-market fit confirmed)

- Active enforcement: policy-based blocking of unauthorized AI usage
- Detection library marketplace: anonymized pattern sharing across customer base
- Company-level AI compliance posture scoring with industry benchmarking
- Full self-serve trial-to-paid flow without founding team involvement
- SIEM integrations (Splunk, Sentinel, etc.)

### Risk Mitigation Strategy

**Technical:**
- *Detection cold-start* — manually curated AI provider endpoint list is the baseline at launch; network-effect enrichment supplements over time
- *Proxy compatibility* — test against the three most common corporate proxy configurations before launch; document known limitations
- *Tenant isolation* — architect and test data isolation before onboarding the first customer; this risk cannot be carried into production

**Market:**
- *Trial doesn't convert* — mitigate by targeting beta customers from industries with high known AI adoption (healthcare, financial services)
- *Null-result trial* — if a customer's environment surfaces zero violations, the trial produces no business case. This is indistinguishable from "detection isn't working." Mitigate by: (a) pre-qualifying beta customers with confirmed AI tool usage before onboarding, (b) providing founding team assessment of expected violation likelihood before trial begins, (c) having a prepared explanation distinguishing "clean environment" from "detection gap" with evidence (library coverage report)
- *Wrong buyer* — validate trial-as-business-case assumption with the first 3 customers before scaling outreach

**Resource:**
- *Team size is the binding constraint* — every deferred feature recovers time; be ruthless about MVP scope
- *Manual onboarding capacity* — the founding team can support a maximum of 2–3 concurrent onboardings without degrading quality or stalling engineering. At ≥15 active customers, onboarding demand will exceed available founding team bandwidth. Self-service provisioning must be scoped and begun in Phase 2 before this threshold is reached — treat 15 customers as the hard trigger, not a soft guideline

## User Journeys

### Journey 1: Sarah Chen — The Audit Wake-Up Call (IT Manager, Success Path)

Sarah manages IT for a 150-person healthcare services company — a team of two, covering helpdesk, vendor management, and compliance without a dedicated security specialist. Last audit cycle, an auditor asked which AI tools had access to patient data. She had no answer.

**Discovery:** Three months before the next audit, Sarah searches "how to track employee AI tool usage." She finds Stack-Breach in a community thread — the positioning ("for IT teams without a dedicated security function") fits exactly.

**Onboarding:** Sarah signs up for a trial. Onboarding asks: "What industry are you in?" She selects Healthcare. HIPAA rules pre-load. She installs the browser monitoring component and connects API call monitoring. Setup takes four hours.

**First value:** The next morning: 12 unauthorized AI tools detected. Three high-risk — a browser extension used by the nursing coordination team sending patient notes to an external AI API. The violation is tagged: "HIPAA §164.502 — Unauthorized disclosure of PHI to third-party AI processor." Nobody knew this was happening.

**Resolution:** Sarah forwards the findings to her VP before 9am. Trial results are the business case — no proposal needed. The company subscribes. Three months later, she pulls the Stack-Breach compliance report in four minutes. The auditor confirms it covers everything. Sarah is the hero.

---

### Journey 2: Marcus Rivera — Configuration and Continuous Vigilance (Security Analyst, Power User)

Marcus is one of two security team members at a 300-person financial services firm. He owns SOC 2 compliance and knows employees use AI tools, but can't quantify exposure or map it to specific controls.

**Evaluation:** Marcus schedules a demo after a peer recommendation. He's skeptical — he needs configurability, not just a dashboard.

**Configuration:** During onboarding Marcus selects Financial Services. SOC 2 rules pre-load. He customizes immediately: approved tools = Microsoft Copilot only; engineering team scoped out of violation reporting for approved sandbox use.

**Detection:** Within 48 hours: 7 violations. Three from the sales team using a ChatGPT browser extension. One is a Zapier automation routing support tickets to an OpenAI API — nobody on IT knew this existed. Marcus has the tool, data type, SOC 2 control, and timestamp. He files a remediation ticket.

**Ongoing value:** Monthly violation reviews. Dashboard trend line drops as remediation takes hold. At SOC 2 audit season, Marcus exports full violation history with remediation notes. The auditor confirms it's exactly what they need.

---

### Journey 3: Daniel (VP Operations) — Budget Approval (Budget Approver)

Daniel receives Sarah's forwarded trial findings email at 8:47am. He's been hearing about AI compliance risks in board meetings with no visibility into actual exposure at his company.

**Decision:** He reads the dashboard screenshot in 90 seconds — 12 unauthorized tools, 3 high-risk, patient data involved. He replies: "Set up a call with the vendor." Twenty minutes with the founding team: "What does this cost?" ($300/month) and "What happens if we get audited without this?" are the only questions he needs answered. He approves the purchase that afternoon.

**Ongoing:** Three months later, he reviews the Stack-Breach audit report Sarah generated. For the first time he has a clear view of the company's AI risk posture without a technical briefing. He includes the risk summary in his next board update.

---

### Journey 4: Jennifer (External Auditor) — Report Consumer

Jennifer conducts a HIPAA audit at Sarah's company. She's been doing this eight years and expects patchwork screenshots and spreadsheets.

**First impression:** Sarah hands her a PDF generated in four minutes. Jennifer opens it: structured by HIPAA section, each with a findings list, violation detail, data exposure description, and remediation status — matching her audit checklist structure exactly.

**Resolution:** No follow-up questions needed. Three violations were detected and remediated before the audit — documented proof of proactive compliance. Jennifer marks the AI tool compliance section complete. She mentions Stack-Breach to two colleagues.

---

### Journey 5: Founding Team — Manual Onboarding Operations

Glade and Gary onboard a 200-person legal services firm. No self-service portal exists; all provisioning is manual.

**Provisioning:** Glade creates the tenant, sets industry to Legal, pre-loads relevant rules, sends an onboarding call invite.

**Deployment:** Gary walks the IT Manager through browser extension and API monitoring setup. The customer environment has a corporate proxy — Gary adjusts the configuration. Setup completes in 90 minutes.

**Follow-up:** 48 hours later, 6 violations. The IT Manager is already building the business case to continue past trial. Glade notes the proxy issue is the third occurrence — files it as a product requirement for automated proxy detection in Phase 2.

## Domain-Specific Requirements

### Compliance & Regulatory (Platform as a Vendor)

- **SOC 2 Type II certification** — customers in regulated industries require this before procurement; target certification within 12 months of launch
- **Data handling transparency** — clear, auditable data retention policies for all monitored data; Stack-Breach must not become the liability it's designed to prevent
- **GDPR data processor agreements** — required when monitoring EU-based employees; purpose-limitation controls must be in place
- **Vendor security questionnaire readiness** — SIG Lite and CAIQ responses prepared before enterprise sales motion begins

### Technical Constraints

- **Zero cross-tenant data leakage** — the highest-severity technical requirement; a breach exposing one customer's violations to another is catastrophic and business-ending
- **Encryption at rest and in transit** — all monitored network data and stored violation records encrypted end-to-end
- **Audit log integrity** — platform audit trail must be tamper-evident; customers may present Stack-Breach logs as evidence in their own compliance audits
- **Minimal data retention footprint** — retain only what's needed for detection and reporting; do not accumulate sensitive employee behavioral data beyond stated purpose
- **Network proxy compatibility** — detection agents must function correctly in standard corporate proxy environments

### Risk Mitigations (Domain)

- **False positive risk** — miscategorized violations erode user trust irreversibly; invest in precision over recall in the early detection library
- **Detection evasion** — employees may route AI usage through VPNs or obfuscated endpoints; document this as a known architectural gap, not a post-launch surprise
- **Over-alerting fatigue** — excessive low-severity alerts cause dashboard blindness; severity tiers must make critical violations unmissable while suppressing noise

## Innovation & Novel Patterns

### Primary Innovation: Network-Effect Detection Library

Shadow AI detection data doesn't exist as a structured, accessible dataset. Stack-Breach's architecture — where every monitored customer enriches the shared detection library — creates a compounding data moat. The more customers onboard, the more accurate detection becomes for all.

- **Assumption challenged:** Compliance detection tools are static rule engines. Stack-Breach's library improves continuously from real-world usage data.
- **Market gap:** No purpose-built SMB shadow AI detection platform with a shared, anonymized detection library exists today.
- **Validation:** Measure detection accuracy per 5-customer increment — improvement should be measurable within the first 20 customers.
- **Fallback:** Manually curated AI provider endpoint coverage delivers value independent of network-effect enrichment.

### Secondary Innovation: Trial-as-Business-Case

Most B2B SaaS requires a vendor proposal to justify budget. Stack-Breach's trial output (violations surfaced within 48 hours) *is* the business case. Value demonstration is built into the detection engine, not the sales motion.

- **Assumption challenged:** B2B SaaS requires a formal justification cycle before purchase.
- **Validation:** Track time-from-trial-start to purchase decision without active sales intervention.

### Market Context

- Enterprise alternatives (Darktrace, Nightfall) cost $50K+/year targeting large organizations — not viable for the SMB segment
- No affordable, purpose-built shadow AI detection product for mid-size companies exists today
- First-mover advantage in the detection library is significant — replicating it requires years of customer volume
- The window is open but not permanent; enterprise players will eventually trickle down

### Innovation Risks

- **Cold-start:** Early customers see lower accuracy before the library matures; manually curated endpoint coverage is the baseline
- **Privacy:** Anonymization of detection patterns is non-negotiable; any perception of unanonymized sharing would be business-ending
- **Replication speed:** Stack-Breach's moat depends on moving fast in the first 12–18 months

## SaaS B2B Architecture Requirements

### Tenant Model

- **Tenant = Company account** — one tenant per customer organization
- **Row-level data isolation** — all detection data, violation records, rules, and reports are tenant-scoped at the database layer; no cross-tenant data access
- **Tenant-scoped authentication** — users authenticate into their tenant context; no shared user pool
- **Manual tenant provisioning (MVP)** — founding team creates and configures tenants; automated provisioning is Phase 2
- **Per-tenant rule engine** — each tenant has an independent rule configuration; global presets are copied per-tenant, not shared

### Permission Model (RBAC)

| Role | Access |
|---|---|
| **IT Manager / Admin** | Full platform access: configure rules, view all violations, generate reports, manage settings |
| **Security Analyst** | Full access to violations and rule configuration; cannot manage tenant settings |
| **Read-Only Viewer** | View dashboard and reports only; no configuration access (VP/Director use case) |
| **Founding Team (Internal)** | Tenant provisioning, cross-tenant admin for support; scoped to internal operations |

### Subscription Tiers

| Tier | Price | Company Size | Detection Surface |
|---|---|---|---|
| **Starter** | ~$200/month | 50–100 employees | Browser extension + API call monitoring |
| **Growth** | ~$350/month | 100–300 employees | Starter + Phase 2 integrations |
| **Scale** | ~$500/month | 300–500 employees | Full detection surface |

All beta customers onboarded at a single negotiated rate; formal tier structure introduced post-beta.

### Implementation Constraints

- **Multi-tenancy is foundational** — all data, rules, configurations, and reporting are tenant-scoped from day one; retrofitting isolation post-launch is high-risk
- **Detection agents run in customer environments** — browser extension and API call monitor deploy inside customer networks; the SaaS backend aggregates and analyzes
- **Detection library must be remotely updatable** — AI provider endpoints change continuously; updates must not require customer re-deployment or device restart
- **Proxy compatibility required at launch** — common customer environment pattern; must work before first customer onboards

## Functional Requirements

### Detection Engine

- **FR1:** The system monitors browser extensions on managed devices and detects outbound calls to known AI provider endpoints
- **FR2:** The system monitors outbound network API calls from managed devices and detects requests to known AI provider endpoints
- **FR3:** The system maintains and updates a library of known AI provider endpoints (OpenAI, Anthropic, Google AI, Cohere, Mistral, and equivalents) without requiring customer re-deployment
- **FR3a:** When the platform derives detection signals from customer monitoring data to enrich the shared endpoint library, it processes only anonymized behavioral patterns (e.g., destination hostname/IP, request structure) — never payload content, PII, or tenant-identifiable metadata. Customers are informed of this data use in the vendor agreement and privacy policy. The enrichment pipeline is documented and auditable
- **FR4:** The system classifies each detected AI interaction by the type of data carried (e.g., text, file content, form data)
- **FR5:** The system detects AI API calls and transmits violation events to the platform backend without data loss or connection error in customer environments using standard HTTP/HTTPS corporate proxy configurations
- **FR6:** The system deploys to managed devices via Chrome Enterprise policy or MDM/EMM tooling without per-user installation

### Violation Management

- **FR7:** The system tags each detected violation with the specific compliance rule broken, mapped to the applicable regulation (e.g., HIPAA §164.502, SOC 2 CC6.1)
- **FR8:** The system assigns a risk severity level (high / medium / low) to each detected violation
- **FR9:** IT Managers and Security Analysts can view detected violations filtered by severity, tool, department, and date range
- **FR10:** IT Managers and Security Analysts can view full violation detail: tool name, data type exposed, regulation violated, timestamp, and affected user or device
- **FR11:** Security Analysts can record remediation notes and mark violations as remediated
- **FR12:** The system tracks remediation status per violation and surfaces unresolved violations distinctly from resolved ones

### Rule Engine

- **FR13:** Tenant Admins can select their industry during onboarding and have industry-specific compliance rule presets automatically applied. Preset minimum content:
  - **HIPAA preset:** Flags any outbound AI API call that carries text classified as potentially containing PHI (patient names, diagnoses, treatment details, dates linked to individuals); maps violations to HIPAA Privacy Rule §164.502 (unauthorized disclosure) and Security Rule §164.312 (technical safeguards); flags browser extensions with no published data retention or processing policy
  - **SOC 2 preset:** Flags outbound AI API calls to non-approved vendors (default: all AI providers flagged unless explicitly approved); maps violations to SOC 2 Trust Services Criteria CC6.1 (logical access) and CC6.6 (external party management); flags integrations routing data to AI providers without documented data processing agreements
- **FR14:** Tenant Admins can create, edit, and delete custom compliance rules within their tenant
- **FR15:** Tenant Admins can designate specific AI tools as approved, preventing them from generating violations
- **FR16:** Tenant Admins can scope detection rules to specific departments or user groups to exclude approved use cases
- **FR17:** Rule changes by one tenant have no effect on any other tenant's rule configuration

### Dashboard

- **FR18:** IT Managers and Security Analysts can view a dashboard summarizing total violations by severity level and time period
- **FR19:** IT Managers and Security Analysts can view all unauthorized AI tools detected across their organization
- **FR20:** The dashboard displays high-severity violations at the top of the violation list by default, visually distinguished from medium/low violations by color coding or iconography, appearing above the fold on a standard 1080p desktop display
- **FR21:** Read-Only Viewers (VP/Director) can access the dashboard and view violation summaries and reports without configuration access

### Audit Report Generation

- **FR22:** IT Managers can generate a compliance report on demand without manual data collection
- **FR23:** Generated reports are structured by regulatory requirement, with violations mapped to specific regulation sections
- **FR24:** Generated reports include remediation status per violation
- **FR25:** Generated reports can be exported as PDF for delivery to external auditors
- **FR26:** Reports use plain-language violation summaries (no internal system codes or raw log data) and include a one-paragraph executive summary section describing risk posture and key findings without requiring compliance or technical background to interpret

### Tenant & User Management

- **FR27:** The founding team can provision new tenant accounts, configure industry presets, and onboard customers without a self-service portal
- **FR28:** Each tenant's data (violations, rules, reports, configurations) is fully isolated from all other tenants at the data layer
- **FR29:** Tenant Admins can invite users and assign roles (Admin, Security Analyst, Read-Only Viewer)
- **FR30:** Users authenticate into their tenant context; no cross-tenant user access exists
- **FR31:** The platform maintains an immutable audit log of all platform actions (logins, rule changes, report exports, user provisioning) per tenant

### Onboarding

- **FR32:** New customers complete initial configuration — industry selection, rule preset application, and monitoring agent deployment — within one business day with founding team support
- **FR33:** The onboarding flow presents industry selection in plain language and automatically applies the appropriate compliance rule presets
- **FR34:** The monitoring agent deployment process is documented and executable by a non-specialist IT Manager with remote founding team guidance

## Non-Functional Requirements

### Security

- **NFR-S1:** All customer data (violation records, monitored traffic, configurations, reports) is encrypted at rest using AES-256 or equivalent
- **NFR-S2:** All data in transit between detection agents and the platform backend is encrypted using TLS 1.2 or higher
- **NFR-S3:** Tenant data isolation is enforced at the database layer via row-level security (RLS) or equivalent mechanism — no query, report, or API call returns data belonging to another tenant. Verified by: automated cross-tenant access tests that attempt to retrieve tenant A's violation records while authenticated as tenant B, run as part of CI/CD pipeline. SOC 2 audit evidence = test results log demonstrating zero cross-tenant data returns across all API endpoints and report generation paths
- **NFR-S4:** Tenant Admin accounts require multi-factor authentication (MFA)
- **NFR-S5:** The platform maintains a tamper-evident audit log of all security-relevant actions (authentication events, rule changes, report exports, user provisioning) with minimum 12-month retention
- **NFR-S6:** Third-party penetration testing conducted at least annually; critical and high findings remediated before the next customer onboarding cycle
- **NFR-S7:** The detection agent collects only the minimum data required to identify a violation — no full request/response payloads or personal user data beyond compliance mapping needs

### Performance

- **NFR-P1:** On-demand audit report generation completes within 10 seconds for a tenant with up to 500 employees and 12 months of violation history
- **NFR-P2:** Dashboard violation list loads within 3 seconds under a single-tenant load of up to 500 managed devices and 10,000 violation records
- **NFR-P3:** Detection agent processing introduces less than 50ms overhead per network request to the end user's browser, as measured by browser developer tools network timing on a standard corporate device
- **NFR-P4:** The AI provider endpoint library is updatable (new providers, updated endpoints) without detection agent reinstallation or device restart
- **NFR-D1:** Detection accuracy of ≥90% is measured against the platform's current known AI provider endpoint library — verified by controlled test environments where ground truth (known AI tools installed and in use) is established before scanning. Accuracy = (correctly flagged violations) / (total violations present in ground truth). The endpoint library's completeness is tracked separately as a coverage metric: number of known public AI providers with active API endpoints covered vs. total identified.

### Reliability

- **NFR-R1:** Platform uptime ≥99.5% measured monthly — downtime creates compliance monitoring gaps for customers
- **NFR-R2:** Detection agent failures are reported to the dashboard within one scan cycle (scan cycle = 15 minutes) so IT Managers are aware of monitoring gaps
- **NFR-R3:** Detection events are queued and processed after backend recovery — no data loss on failure
- **NFR-R4:** Violation history and configurations can be restored within 4 hours of a data loss event

### Scalability

- **NFR-SC1:** The platform architecture supports growth from 20 to 500 tenant accounts without re-architecture
- **NFR-SC2:** Per-tenant monitoring supports organizations with up to 500 managed devices without performance degradation
- **NFR-SC3:** The AI provider endpoint library scales to thousands of endpoints without detection agent performance impact
- **NFR-SC4:** The detection data pipeline processes increased event volume from network-effect library enrichment without manual intervention

### Integration

- **NFR-I1:** The browser extension monitoring agent supports Chrome and Chrome-based browsers (Edge, Brave) deployed via Chrome Enterprise policy or MDM
- **NFR-I2:** Outbound API call detection supports standard HTTP/HTTPS corporate proxy configurations
- **NFR-I3:** Generated PDF reports conform to PDF/A format suitable for long-term archival and auditor tooling
- **NFR-I4:** The detection agent update mechanism operates without changes to customer IT infrastructure or managed software re-deployment
