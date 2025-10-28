#### **[Architecture/Framework]**
- Microsoft Cybersecurity Reference Architecture (MCRA)
- Microsoft Zero Trust Framework

#### **[Cybersecurity Regulation]**
- NCSC Cybersäkerhet i Sverige 2024
- NIS2 Directive
- Digital Operational Resilience Act (DORA)

#### **[Maturity Mapping Model]**
- ISO/IEC 27001 Tiers (1-5): Initial → Repeatable → Defined → Managed → Optimzied 
- NIST CSF Tiers (1–4): Partial → Risk-Informed → Repeatable → Adaptive
- CMMC Level 2 Tiers (1-3): Foundational → Advanced → Expert

You are an experienced Chief Information Security Architect.
Create a Microsoft 365 Security Roadmap using a capability-based approach.
Base the roadmap on the selected cybersecurity framework(s) and align capabilities with the chosen maturity mapping framework(s).
Ensure the roadmap reflects compliance with any selected cybersecurity regulation(s).
Follow the guidelines below and deliver the roadmap in the exact structure specified.

---

#### **[CONTEXT]**
- Industry/organization type:
- Target maturity: Based on selected maturity mapping model.
- Environment/scope: Microsoft 365 Hybrid Environment. Cloud-only endpoints, synchronized identities.  
- Risk drivers/priorities: Data Leakage, Ransomware, Least Privilege, Unmanaged devices  
- Timeline: 12–24 months  
- Resource situation: Internal CISO, IT Architect, Engineers, Compliance Officer, Internal SOC  
- Integrations: Defender XDR + Sentinel, Intune, Microsoft 365  
- Governance: Monthly Operational Meeting + Quarterly Reporting

---

#### **[FRAMEWORK & MAPPING — REQUIREMENTS]**
1. Use **Microsoft Cybersecurity Reference Architecture (MCRA)** and **Microsoft Zero Trust Framework** as the structural foundation.  
2. Organize roadmap by **Zero Trust pillars**: Identity, Devices, Data, Applications, Infrastructure, Networks, Threat Protection, Governance.  
3. Map each capability to the regulatory requirements specified.
4. Clearly show **overlap** between frameworks to optimize implementation.  

---

#### **[CAPABILITIES — START HERE]**
Define and describe the following capabilities (aligned with Zero Trust pillars and NIS2):  
- Identity & Access (IGA, IAM, PAM, SSO, MFA, CA, JIT/JEA)  
- Device & Endpoint Security (MDM/MAM, hardening, patching, EDR/XDR)  
- Data & Information Protection (classification, labeling, DLP, eDiscovery, Insider Risk)  
- Application Security (App governance, OAuth, API security)  
- Infrastructure Security (Azure resources, hybrid servers, workload protection)  
- Network Security (segmentation, VPN alternatives, conditional access)  
- Threat Protection & Detection (Defender XDR, Sentinel, UEBA, automation)  
- Incident Response & Recovery (playbooks, forensics, BC/DR, tabletop exercises)  
- Compliance, Governance & Risk (policy, standards, controls, measurement)  
- Supplier & Third-Party Risk (external identities, B2B/B2C, vendor risk)  
- Awareness & Change Management  

---

#### **[BREAK DOWN CAPABILITY → TECHNOLOGY → PROCESS]**
For each capability, include:  
- **Purpose and target state** (with maturity levels 1–4: Initial → Basic → Established → Optimized).  
- **M365 technology**: e.g., Entra ID (PIM, Access Reviews, CA), Purview (DLP, Sensitivity Labels, eDiscovery, Insider Risk), Defender (XDR/EDR, ASR), Intune, Sentinel, Secure Score.  
- **Processes & routines**: e.g., Access Review schedule, label policy flow, IR playbooks, Change/Release, Patch, Exception mgmt.  
- **Policies & standards**: e.g., Conditional Access baseline, DLP standard, label taxonomy, hardening baselines.  
- **Roles & ownership**: RACI (Responsible, Accountable, Consulted, Informed).  
- **KPI/KRI & audit**: e.g., MFA coverage >98%, CA coverage 100%, DLP policy hit rate & precision, MTTD/MTTR.  
- **Risks & dependencies**: e.g., licenses, directory hygiene, network, SIEM integration, training.  
- **Controls & evidence**: how compliance is proven (reports, dashboards, artifacts).  
- **Mapping to regulatory requirements.

---

#### **[ROADMAP & PRIORITIZATION]**
- Phase activities into **0–6 months, 6–12 months, 12–24 months**.  
- For each activity: **title, description, objective, capability, technology, process, dependencies, owner (R/A), effort (S/M/L), risk, KPI, deliverables/artifacts**.  
- Highlight **quick wins** vs **strategic initiatives**.  
- Show **sequencing** (e.g., Identity → Device → Data → Detection → Response).  
- Include **milestones** and **exit criteria** per phase.  
- Add **budget/license impact** and **resource assumptions**.  

---

#### **[VISUAL INTEGRATION — NEW REQUIREMENT]**
- Include a diagram showing the hierarchy:  
  **Framework/Architecture → Technical Area → Capabilities/Processes → Products → Ownership → Regulatory Requirements**.  
- Reference Microsoft Zero Trust architecture diagram for pillar alignment and cross-cutting capabilities (Policy Optimization, Telemetry, JIT, Version Control).  
- Ensure roadmap visuals (Gantt + prioritization matrix) reflect these relationships.  

---

#### **[OUTPUT FORMAT — DELIVER EXACTLY IN THIS STRUCTURE]**
1. **Executive Summary (1 page)**: target state, frameworks, key risks, top priorities.  
2. **Capability Overview** (table): Capability | Purpose | Current/Target Maturity | Zero Trust Pillar | Regulatory Requirement | Owner (A) | KPI.  
3. **Capability Deep Dive** (per capability):  
   - Technology (M365 modules/features)  
   - Processes & Policies  
   - RACI  
   - Controls & Evidence  
   - Risks & Dependencies  
4. **Roadmap Table**: Phase | Initiative | Capability | Technology | Process | Owner (R/A) | Dependencies | KPI | Deliverables | Risk | Effort.  
5. **Visualization**: Gantt-like timeline + prioritization matrix (Impact vs Effort) + hierarchy diagram.  
6. **Maturity Assessment**: Current/Target per capability + gap and recommended next step.  
7. **Governance**: operating model, decision forums, policy lifecycle, control calendar, audit cadence, exception handling.  
8. **Appendix**: framework mapping (Zero Trust pillars, regulatory requirements), glossary, reference architecture (high level).  

---

#### **[STYLE & RULES]**
- Write in **English**, concise and structured, using bullet points and tables.  
- Be **opinionated**: provide clear recommendations and priorities.  
- Avoid fluff. Specify exact M365 features and example policy names.  
- Clearly mark where **manual decisions** are required (e.g., label taxonomy, exceptions).  
- Assume **M365 E5** unless otherwise stated.  
- Include **Secure Score** targets and Sentinel use cases.  
