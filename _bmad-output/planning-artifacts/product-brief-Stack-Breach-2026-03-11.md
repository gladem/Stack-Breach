---
stepsCompleted: [1, 2]
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
