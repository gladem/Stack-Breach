---
stepsCompleted: [1, 2, 3, 4, 5]
inputDocuments:
  - PRD Images/IMG_6951.PNG
  - PRD Images/IMG_6952.PNG
  - PRD Images/IMG_6953.PNG
  - PRD Images/IMG_6954.PNG
  - PRD Images/IMG_6955.PNG
  - PRD Images/IMG_6956.PNG
  - PRD Images/IMG_6957.PNG
  - PRD Images/IMG_6958.PNG
  - PRD Images/IMG_6959.PNG
  - PRD Images/IMG_6960.PNG
  - PRD Images/IMG_6961.PNG
  - PRD Images/IMG_6962.PNG
  - PRD Images/IMG_6963.PNG
  - PRD Images/IMG_6964.PNG
  - PRD Images/IMG_6965.PNG
  - PRD Images/IMG_6966.PNG
  - PRD Images/IMG_6967.PNG
  - PRD Images/IMG_6968.PNG
  - PRD Images/IMG_6969.PNG
  - PRD Images/IMG_6970.PNG
  - PRD Images/IMG_6971.PNG
  - PRD Images/IMG_6972.PNG
  - PRD Images/IMG_6973.PNG
  - PRD Images/IMG_6974.PNG
  - PRD Images/IMG_6975.PNG
  - PRD Images/IMG_6976.PNG
  - PRD Images/IMG_6977.PNG
  - PRD Images/IMG_6978.PNG
  - PRD Images/IMG_6979.PNG
  - PRD Images/IMG_6980.PNG
  - PRD Images/IMG_6981.PNG
date: 2026-03-11
author: Glade Mellor
---

# Product Brief: Stack-Breach

## Executive Summary

Stack Breach is a SaaS platform that detects unauthorized AI usage across company tools and generates compliance-ready audit reports, purpose-built for mid-size companies (50-500 employees) that can't afford enterprise compliance platforms. As AI adoption explodes across every department - marketing using ChatGPT, sales running Claude, support installing AI-powered browser extensions - companies face growing exposure to data breaches and regulatory violations they can't even see. Stack Breach provides the visibility and reporting these companies need at a price point ($200-$500/month) that makes compliance accessible. The platform starts as a detection and reporting tool focused on the highest-risk vectors - browser extensions and outbound API calls to AI providers - with a roadmap to expand detection surface and evolve into active policy enforcement. With AI adoption accelerating across every department and regulatory pressure expected to increase as governments catch up, the need for affordable shadow AI detection is urgent and growing.

---

## Core Vision

### Problem Statement

Employees across every department are rapidly adopting AI tools - browser extensions, API integrations, SaaS features with embedded AI, direct usage of chat interfaces - often without understanding the compliance and data security implications. A healthcare company routing patient notes through ChatGPT is a HIPAA violation. A design agency using Midjourney on client assets is a contractual breach. A support team's Chrome extension sending every ticket to an external API with no data retention policy is a data leak waiting to happen. Most mid-size companies discover this shadow AI usage the same way: an auditor asks a question nobody can answer. The velocity of AI tool adoption is accelerating faster than any company's ability to track it, making this an urgent and worsening problem.

### Problem Impact

- **Regulatory exposure**: Unauthorized AI usage can violate HIPAA, GDPR, SOC 2, and industry-specific regulations, resulting in fines and legal liability
- **Data security risk**: Sensitive company and customer data is being sent to external AI APIs with unknown data retention and processing policies
- **Audit failure**: Companies cannot demonstrate compliance because they have no visibility into what AI tools are being used, by whom, or what data flows through them
- **Growing attack surface**: The number of AI tools and integration points is expanding constantly, making the problem worse over time without systematic detection
- **Increasing regulatory pressure**: As AI adoption becomes widespread, governments and regulatory bodies are expected to introduce stricter compliance requirements - companies without visibility into their AI usage today will face even greater exposure as these regulations tighten
- **88% of companies** have experienced AI-related incidents, signaling this is not a hypothetical risk

### Why Existing Solutions Fall Short

Enterprise compliance platforms (e.g., Darktrace) that can detect unauthorized AI usage cost $50,000+ per year, putting them out of reach for mid-size companies. These platforms are built for large organizations with dedicated compliance teams. Mid-size companies - the ones most vulnerable because they lack compliance staff - are left on their own. There is no purpose-built, affordable solution targeting shadow AI detection for the SMB segment. The market gap is significant and widening daily as the rapid adoption of AI tools across every department outpaces any organization's ability to maintain visibility through manual processes.

### Proposed Solution

Stack Breach is a monitoring platform that scans a company's tools for unauthorized AI usage, starting with the highest-risk and most detectable vectors: browser extensions calling external AI APIs and outbound API calls to known AI providers. Each flagged instance is tagged with what data it carried and which compliance rule it broke. The platform generates reports formatted for auditors, not engineers - making compliance actionable without requiring a dedicated compliance team. The rule engine is configurable per customer to account for industry-specific regulations. The detection surface expands over time to include third-party SaaS with embedded AI features and deeper integrations with collaboration platforms like Slack, GSuite, and Microsoft 365. As detection matures, Stack Breach will evolve from reporting into active enforcement capabilities, enabling companies to automatically block or restrict unauthorized AI usage based on their policies.

### Key Differentiators

- **SMB-first pricing**: $200-$500/month based on team size, versus $50K+/year for enterprise alternatives - a 200-person company pays less for a year of Stack Breach than one hour of legal cleanup after a failed audit
- **Purpose-built for shadow AI**: Not a general security tool repurposed for AI - built specifically to detect unauthorized AI usage patterns across the full spectrum of adoption paths
- **Focused MVP, extensible architecture**: Launches with browser extension and API call monitoring (highest risk-to-implementation ratio), designed to expand detection surface without re-architecting
- **Auditor-ready output**: Reports formatted for compliance auditors, not technical staff, bridging the gap between IT discovery and regulatory reporting
- **Configurable rule engine**: Industry-specific compliance rules from day one - healthcare violations are different from design agency violations
- **Network-effect detection library**: Every company monitored adds data on which tools create which risks in which industries, making detection more accurate for every future customer and harder to replicate without matching volume
- **Founding team credibility**: Co-founded by Glade Mellor, an engineering manager who understands how teams adopt tools in the wild, and Gary Van Sluis, a CISSP-certified IT Security Champion who brings deep security and compliance expertise. The product reflects real IT operations and security experience, not theoretical compliance frameworks
- **Tiered detection-to-pricing alignment**: Detection surface expansion maps naturally to pricing tiers, giving customers a clear upgrade path as their compliance needs grow
- **Built for the AI adoption wave**: Designed for a market where AI tool proliferation is the norm, not the exception - the platform's detection capabilities are built to keep pace with the constant emergence of new AI tools, integrations, and usage patterns

## Target Users

### Primary Users

#### IT Manager / IT Operations Lead (Recommender)
**Persona: "Sarah Chen" - IT Manager at a 150-person healthcare services company**

Sarah manages a small IT team of two and wears many hats - infrastructure, vendor management, helpdesk escalations, and compliance. She's not a security specialist, but compliance responsibilities fall on her desk because the company doesn't have a dedicated security team. Every audit cycle, she scrambles to manually inventory what tools employees are using. Last quarter, an auditor asked what AI tools had access to patient data and she had no answer. She needs a tool she can set up without deep security expertise, that runs in the background, and that produces reports she can hand directly to auditors. Sarah is the recommender, not the budget holder - she evaluates tools, builds the business case, and presents to leadership for approval.

- **Role**: IT Manager responsible for compliance reporting, tool oversight, and audit readiness
- **Environment**: Mid-size company (50-500 employees), small or no dedicated security team, wears multiple hats
- **Motivation**: Avoid audit failures, demonstrate compliance without manual detective work, protect the company from regulatory exposure
- **Pain today**: No visibility into shadow AI usage, manual and incomplete audit preparation, reactive discovery of violations
- **Success looks like**: Configuring Stack Breach in an afternoon, receiving automated alerts on new AI usage, and handing auditors a comprehensive report without scrambling
- **Buying role**: Recommender - discovers and evaluates the tool, builds the internal business case, presents findings to leadership for budget approval

#### Security / IT Department Staff
**Persona: "Marcus Rivera" - IT Security Analyst at a 300-person financial services firm**

Marcus is one of two people on a lean security team. He's responsible for data protection policies and ensuring the company meets SOC 2 requirements. He knows employees are using AI tools but has no systematic way to find them all. He needs to identify violations, understand the data exposure, configure detection rules specific to financial services regulations, and remediate issues before they become audit findings. In companies without a dedicated security team, this role may be filled by the IT Manager (like Sarah) who also handles tool configuration.

- **Role**: Security analyst or IT staff responsible for data protection and regulatory compliance
- **Environment**: Mid-size company with a small dedicated security function, compliance-conscious industry
- **Motivation**: Proactively find and remediate compliance violations, configure industry-specific detection rules, reduce the company's risk surface
- **Pain today**: Knows shadow AI is happening but can't quantify or locate it systematically, spends time on manual investigation
- **Success looks like**: A configured rule engine catching 90%+ of unauthorized AI usage, clear violation details with data exposure mapping, actionable remediation paths

### Secondary Users

#### VP / Director (Budget Approver)
The actual buyer. They don't use Stack Breach directly but approve the spend based on Sarah's recommendation. They care about risk reduction, cost avoidance, and regulatory liability - not detection mechanics. Audit reports serve as interim executive reporting in MVP, giving leadership visibility into the company's shadow AI risk posture without requiring a separate dashboard.

#### External Auditors
Receive compliance reports generated by Stack Breach. They need reports formatted to their standards - clear, structured, and mapped to specific regulatory requirements. They don't use the platform directly but are the primary audience for its core output.

#### Department Heads
May be notified when their team members are flagged for non-compliant AI usage. They need enough context to have a conversation with their employee about compliant alternatives. Not an MVP priority - post-MVP notification feature.

### User Journey

#### Discovery
Sarah discovers Stack Breach through multiple paths: after a painful audit where she couldn't answer questions about AI usage, through peer recommendations in IT communities (Reddit r/cybersecurity, r/ITManagers, LinkedIn), or after a board member raises concerns about AI compliance risks. She searches for affordable shadow AI detection and finds Stack Breach positioned for mid-size companies.

#### Onboarding
Sarah signs up for a trial. The setup is guided and jargon-free: "What industry are you in? Healthcare? We've pre-loaded HIPAA rules for you." She connects Stack Breach to her company's environment and installs the browser extension monitoring component. Setup takes less than a day. Stack Breach begins scanning immediately.

#### Trial as Business Case
Within 48 hours, Stack Breach surfaces initial findings - "We found 12 unauthorized AI tools across your organization, with 3 high-risk data exposure points." Sarah forwards these findings to her VP. The trial results ARE the internal business case - no proposal writing needed, the data speaks for itself.

#### Core Usage
Stack Breach runs continuously in the background. Sarah checks for new flagged AI usage regularly. If a dedicated security analyst is on staff, they configure industry-specific rules and handle remediation. When violations are detected, they're tagged with what data was exposed and which regulation was violated.

#### Success Moment
The next audit cycle, Sarah pulls a comprehensive compliance report from Stack Breach in minutes. The auditor confirms it covers everything they need. Her VP reviews the same report and for the first time understands the company's AI risk posture. Sarah is the hero who found the solution.

#### Long-term Value
Every quarter, Stack Breach catches new AI tools employees have started using. The detection library gets smarter. When regulatory requirements tighten, Sarah updates her rule engine rather than starting from scratch. Audit reports serve double duty as leadership reporting. As the company grows, Stack Breach's detection surface expands through pricing tiers.

## Success Metrics

### User Success Metrics

- **Detection accuracy**: The platform reliably identifies unauthorized AI usage with high accuracy and low false positive rates. Target: 90%+ detection rate of shadow AI tools with minimal noise that gets ignored
- **Time-to-value**: Users experience value quickly from signup to actionable findings. Target: Setup completed within one day, first violations detected within 48 hours
- **Audit readiness**: Users can produce compliance reports on demand without manual investigation. Target: Comprehensive audit report generated in minutes, not days of manual work

### Business Objectives

- **Customer acquisition**: Grow the customer base as the primary indicator of product-market fit and business viability. Target: 10-20 beta customers within 90 days of launch
- **Detection accuracy as product quality**: Maintain and improve detection accuracy as the core measure of product value - accuracy drives retention, word-of-mouth, and competitive moat
- **Network-effect growth**: Each new customer enriches the detection library, improving accuracy for all customers and making the platform harder to replicate

### Key Performance Indicators

| KPI | Measure | Why It Matters |
|-----|---------|----------------|
| Detection accuracy rate | % of shadow AI tools correctly identified vs. total present | Core product quality - if detection isn't accurate, nothing else matters |
| False positive rate | % of flagged items that are not actual violations | Low noise ensures users trust the tool and don't ignore alerts |
| Customer count | Total paying customers | Primary business traction metric |
| Time to first detection | Hours from setup completion to first violation surfaced | Drives trial-to-paid conversion - fast value demonstration |
| Setup completion time | Hours from signup to fully configured monitoring | Validates the product is accessible to non-specialist IT managers |
| Trial-to-paid conversion | % of trial users who become paying customers | Validates that the trial experience delivers the business case |
| Customer retention | Monthly/quarterly churn rate | At $200-$500/month, retention is critical to sustainable growth |

## MVP Scope

### Core Features

1. **Shadow AI Detection Engine**
   - Monitor browser extensions calling external AI APIs
   - Detect outbound API calls to known AI providers (OpenAI, Anthropic, Google AI, etc.)
   - Flag each violation with what data was carried and which compliance rule it broke

2. **Configurable Rule Engine**
   - Industry-specific compliance rule presets (e.g., HIPAA for healthcare, SOC 2 for financial services)
   - Guided industry selection during onboarding: "What industry are you in? We've pre-loaded the relevant rules"
   - Per-tenant rule customization for company-specific policies

3. **Dashboard**
   - Visual overview of flagged violations and risk levels
   - View of unauthorized AI tools detected across the organization
   - Violation details: what tool, what data, which rule broken, risk severity
   - The primary interface for IT managers and security staff to monitor shadow AI usage

4. **Audit Report Generation**
   - Compliance reports formatted for external auditors, mapped to regulatory requirements
   - Serves double duty as interim leadership reporting
   - On-demand generation - pull a comprehensive report in minutes

5. **Multi-tenant Architecture**
   - Row-level data isolation per customer
   - Per-tenant rule engine configurations
   - Tenant-scoped authentication
   - Manual customer provisioning (no self-service portal in MVP)

6. **Guided Onboarding**
   - Jargon-free setup flow designed for non-specialist IT managers
   - Industry selection with pre-loaded rule presets
   - Remote hands-on onboarding support for early customers from founding team

### Out of Scope for MVP

- **Slack / GSuite / Microsoft 365 deep integration** - Phase 2 detection surface expansion
- **Third-party SaaS embedded AI detection** - Phase 2 detection surface expansion
- **Active enforcement / blocking capabilities** - Future evolution after detection matures
- **Executive dashboard** - Audit reports serve as interim leadership reporting
- **Department head notifications** - Post-MVP feature
- **Self-service customer provisioning portal** - Manual onboarding is sufficient for early customers
- **Self-serve trial signup** - Early customers onboarded by founding team remotely
- **Real-time alerting** - MVP focuses on periodic scanning and on-demand reporting

### MVP Success Criteria

- **Detection accuracy**: 90%+ of unauthorized AI tools correctly identified with low false positive rate
- **Setup speed**: Customer fully configured within one day with remote founding team support
- **Time to first detection**: First violations surfaced within 48 hours of setup
- **Customer validation**: 10-20 beta customers onboarded within 90 days of launch
- **Core value delivered**: Sarah discovers shadow AI usage she didn't know about and has clear risk identification to take action
- **Audit report utility**: At least one customer successfully uses a Stack Breach report in an actual audit

### Future Vision

- **Expanded detection surface**: Slack, GSuite, Microsoft 365 integrations; third-party SaaS with embedded AI features
- **Active enforcement**: Policy-based blocking and restriction of unauthorized AI usage
- **Executive dashboards**: Dedicated leadership views with risk trends and posture scoring
- **Department notifications**: Automated alerts to team leads when violations involve their staff
- **Self-service onboarding**: Automated provisioning and trial-to-paid flow without founding team involvement
- **Real-time alerting**: Immediate notifications when new violations are detected
- **API access**: Allow customers to integrate Stack Breach data into existing security tooling
- **Compliance framework expansion**: Beyond HIPAA and SOC 2 to GDPR, PCI-DSS, industry-specific frameworks
- **Detection library marketplace**: Share anonymized detection patterns across customer base, strengthening the network effect moat
