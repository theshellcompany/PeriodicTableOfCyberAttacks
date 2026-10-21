# Periodic Table of Cyber Attacks - Tabletop Exercise Framework

> **Using the Periodic Table as a Starting Point for Cybersecurity Tabletop Exercises**

---

## Overview

This framework uses the Periodic Table of Cyber Attacks as a **structured, visual, and realistic** starting point for cybersecurity tabletop exercises. The table's organization by attack families and sophistication levels provides a natural progression for exercises, while the European case studies and defense recommendations ground discussions in real-world scenarios.

**Interactive table**: [The Periodic Table of Cyber Attacks](./index.html)  

---

## Quick Start Guide

### 30-Second Setup
1. Display the periodic table on a screen or share digitally
2. Select an exercise template (below)
3. Pick attack elements from the table
4. Use the real European case studies for realism
5. Document gaps and action items

---

## 1. Scenario Selection Methods

Use these approaches to select attacks for your tabletop exercise:

### Method A: Random Attack Draw
- **How**: Participants pick 1-3 elements from different families
- **Combine**: Create attack chains by linking related attacks
- **Example Chain**: Ph (Phishing) → Ao (Token phishing) → Rw (Ransomware)
- **Use Case**: Cross-team coordination exercises

### Method B: Family Deep Dive
- **How**: Select one column (attack family)
- **Progress**: Work through attacks from Level 1 to Level 5
- **Example**: Network column - from Interception to BGP hijacking
- **Use Case**: Technical deep dives, team specialization

### Method C: Defense Gap Analysis
- **How**: Select any attack element
- **Review**: Compare listed defenses against your current controls
- **Question**: *"Would our current controls stop this?"*
- **Use Case**: Control validation, compliance testing

### Method D: Sophistication Escalation
- **How**: Start at Level 1, progress through levels
- **Simulate**: Attacker escalating capabilities
- **Example**: Credentials column - Brute force → Session hijacking → Token forgery
- **Use Case**: Incident response progression, red team vs. blue team

---

## 2. Structured Exercise Templates

### Template 1: Attack Chain Simulation

**Format**: 60-90 minutes  
**Participants**: Security team, IT operations, Management  
**Objective**: Test end-to-end incident response across attack stages

#### Agenda

| Time | Phase | Activity | Facilitator Notes |
|------|-------|----------|-------------------|
| 0:00-0:10 | **Setup** | Draw 3 connected elements from table | Ensure diverse families selected |
| 0:10-0:20 | **Recon** | Research real European case studies | Use links from table |
| 0:20-0:35 | **Detection** | How would we detect each stage? | Map to SIEM rules, alerts |
| 0:35-0:50 | **Response** | Walk through IR playbooks | Identify owner for each action |
| 0:50-1:00 | **Recovery** | System restoration, lessons learned | Focus on business impact |
| 1:00-1:10 | **Improvements** | Document action items | Assign owners, due dates |

#### Example Scenario
- **Elements**: Sm (Smishing) + Cs (Credential stuffing) + Rw (Ransomware)
- **Case Studies**: FluBot botnet + Great Western Railway breach + Picanol manufacturing shutdown
- **Attack Story**: Attackers use SMS phishing to deliver malware, harvest credentials, deploy ransomware

---

### Template 2: Sophistication Escalation

**Format**: 45 minutes  
**Participants**: Blue team, Red team (or combined)  
**Objective**: Practice adapting defenses as attacks escalate in sophistication

#### Agenda

| Time | Phase | Activity | Facilitator Notes |
|------|-------|----------|-------------------|
| 0:00-0:05 | **Setup** | Select column, start at Level 1 | Pick a column with 5+ entries |
| 0:05-0:20 | **Round 1-3** | Defender responds to Level 1-3 | Attacker describes next move |
| 0:20-0:35 | **Round 4-5** | Defender adapts to Level 4-5 | Focus on advanced techniques |
| 0:35-0:45 | **Debrief** | Lessons learned | Document gaps |

#### Example Scenarios by Column

| Column | Level 1 | Level 2 | Level 3 | Level 4 | Level 5 |
|--------|---------|---------|---------|---------|---------|
| **Network** | Interception | DDoS, Port scanning, ARP spoofing | MITM, IP spoofing | DNS hijacking, DNS tunneling | BGP hijacking |
| **Social Engineering** | Phishing, Smishing | Vishing, Pretexting | Spear phishing, CEO fraud | Deepfake impersonation | - |
| **Credentials** | Brute force, Credential stuffing | Password spraying, MFA fatigue | Token phishing, Session hijacking | - | - |

---

### Template 3: Defense Validation

**Format**: 30 minutes  
**Participants**: Security architects, IT operations  
**Objective**: Validate if existing controls would prevent documented attacks

#### Agenda

| Time | Phase | Activity | Facilitator Notes |
|------|-------|----------|-------------------|
| 0:00-0:05 | **Setup** | Select attack family | Choose based on team responsibility |
| 0:05-0:20 | **Validation** | Check each attack's defenses against controls | Use table's defense recommendations |
| 0:20-0:25 | **Scoring** | Rate each control (Green/Yellow/Red) | Be honest about gaps |
| 0:25-0:30 | **Prioritization** | Assign remediation priorities | Focus on high-impact, high-risk |

#### Scoring Matrix

| Status | Meaning | Action Required |
|--------|---------|-----------------|
| ✅ Green | Control implemented and tested | Monitor, maintain |
| ⚠️ Yellow | Control partially implemented | Complete implementation |
| ❌ Red | Control missing | Implement as priority |

---

## 3. Role-Based Tabletop Assignments

Assign exercises based on team responsibilities. Mix technical and non-technical roles for comprehensive cyber resilience.

### Technical Roles

#### SOC Analyst Focus
- **Objective**: Improve detection capabilities
- **Exercise**: Select 5 attacks across different families
- **Question**: *"What logs, alerts, or SIEM rules would detect this?"*
- **Deliverable**: Detection gap analysis

#### Incident Responder Focus
- **Objective**: Test response procedures
- **Exercise**: Walk through response for a Level 4-5 attack
- **Question**: *"What's our playbook for this scenario?"*
- **Deliverable**: Updated IR playbooks

#### Developer Focus
- **Objective**: Secure coding practices
- **Exercise**: Review Web Application column attacks
- **Question**: *"What application controls prevent these?"*
- **Deliverable**: Secure development guidelines

#### Network Engineer Focus
- **Objective**: Infrastructure hardening
- **Exercise**: Address all Network column attacks
- **Question**: *"How do we harden against each of these?"*
- **Deliverable**: Network security improvements

#### Security Architect Focus
- **Objective**: Validate architecture against sophisticated threats
- **Exercise**: Review all Level 4-5 attacks across Advanced & State-Level column
- **Question**: *"Does our architecture account for these sophisticated attack vectors?"*
- **Deliverable**: Architecture improvement roadmap

### Executive Leadership Roles

#### CISO (Chief Information Security Officer) Focus
- **Objective**: Strategic cybersecurity posture and risk management
- **Exercise**: Review Advanced & State-Level column and Supply Chain & Cloud column
- **Question**: *"How do these threats map to our enterprise risk appetite and tolerance?"*
- **Deliverable**: Enterprise cybersecurity strategy alignment, risk appetite statements
- **Key Attacks**: Cyber espionage, Zero-day, Zero-click spyware, Firmware rootkit, Industrial sabotage

#### CIO/CTO (Chief Information/Technology Officer) Focus
- **Objective**: Technology strategy and cyber resilience integration
- **Exercise**: Cross-column scenarios linking Social Engineering → Credentials → Lateral Movement
- **Question**: *"How do we balance innovation velocity with security controls for these attack paths?"*
- **Deliverable**: Technology roadmap with integrated security milestones
- **Key Attacks**: Software supply chain, Container escape, Cloud misconfiguration

#### CFO (Chief Financial Officer) Focus
- **Objective**: Financial risk assessment and cyber investment justification
- **Exercise**: Impact column deep dive with cost estimation
- **Question**: *"What's the potential financial impact (direct and indirect costs) of each scenario? How do we justify cybersecurity investments?"*
- **Deliverable**: Cyber risk financial quantification, business case for security investments
- **Key Attacks**: Ransomware, Data extortion, Cryptojacking, CEO fraud/BEC
- **Metrics**: Recovery costs, business interruption, regulatory fines, reputational damage valuation

#### CEO (Chief Executive Officer) Focus
- **Objective**: Enterprise-wide cyber resilience and crisis leadership
- **Exercise**: Review Level 5 attacks and their organizational impact
- **Question**: *"Which attacks could threaten our business continuity or existence? How do we lead through a cyber crisis?"*
- **Deliverable**: Executive crisis management framework, board-level cyber risk reporting
- **Key Attacks**: All Level 5 attacks, particularly Wiper, Industrial sabotage, BGP hijacking
- **Focus Areas**: Business continuity, regulatory compliance, stakeholder communication

#### COO (Chief Operating Officer) Focus
- **Objective**: Operational resilience and supply chain security
- **Exercise**: Supply Chain & Cloud column combined with Impact column
- **Question**: *"How do we maintain operations during and after a cyber attack on our supply chain?"*
- **Deliverable**: Operational resilience playbooks, supplier cybersecurity requirements
- **Key Attacks**: Software supply chain, Dependency confusion, Container escape, Typosquatting

### Business Function Roles

#### Communications & PR Team Focus
- **Objective**: Crisis communication strategy and stakeholder messaging
- **Exercise**: Ransomware, Data extortion, or Defacement scenarios
- **Question**: *"How do we communicate internally and externally during each phase of the incident? What's our messaging for different stakeholders (customers, partners, media, regulators)?"*
- **Deliverable**: Cyber incident communication plan, template statements, media training
- **Key Attacks**: Ransomware, Data extortion, Defacement, Insider threat (public disclosure)
- **Timeline Practice**: Initial notification, ongoing updates, resolution announcement
- **Stakeholder Mapping**: Employees, customers, partners, investors, regulators, media

#### Legal & Compliance Team Focus
- **Objective**: Regulatory compliance, legal obligations, and liability management
- **Exercise**: Data extortion, Ransomware, Insider threat scenarios
- **Question**: *"What are our legal obligations for breach notification? What regulations apply? What are the liability implications?"*
- **Deliverable**: Incident response legal playbook, regulatory notification templates, contract review checklist
- **Key Regulations**: GDPR (EU), sector-specific regulations, data breach notification laws
- **Key Attacks**: Data extortion, Ransomware, Insider threat, CEO fraud
- **Focus Areas**: Data classification, cross-border data transfers, third-party contracts, insurance coverage

#### HR & People Team Focus
- **Objective**: Workforce security awareness, insider threat prevention, and crisis support
- **Exercise**: Social Engineering column combined with Insider threat
- **Question**: *"How do we protect against, detect, and respond to insider threats? How do we support employees during and after an incident?"*
- **Deliverable**: Security awareness training program, insider threat policy, employee support protocols
- **Key Attacks**: Phishing, CEO fraud, Insider threat, MFA fatigue (user training)
- **Focus Areas**: Security culture, reporting mechanisms, mental health support, remote work security

#### Finance & Procurement Team Focus
- **Objective**: Financial controls, vendor risk management, and cyber insurance
- **Exercise**: CEO fraud/BEC, Supply Chain & Cloud, Credentials column
- **Question**: *"How do we prevent financial fraud through cyber means? How do we assess and manage third-party cyber risk?"*
- **Deliverable**: Vendor cybersecurity assessment framework, payment fraud prevention controls, cyber insurance policy review
- **Key Attacks**: CEO fraud/BEC, Credential stuffing, Cloud misconfiguration, Software supply chain
- **Focus Areas**: Payment approval workflows, vendor due diligence, contract cybersecurity clauses, insurance coverage gaps

#### Customer Success/Service Team Focus
- **Objective**: Customer trust preservation and service continuity
- **Exercise**: Defacement, Data extortion, Ransomware scenarios
- **Question**: *"How do we maintain customer trust and service delivery during a cyber incident? What do customers need to know and when?"*
- **Deliverable**: Customer communication protocols, service continuity plans, trust restoration strategy
- **Key Attacks**: Defacement, Data extortion, Ransomware, DDoS
- **Focus Areas**: SLA implications, customer notification timing, support capacity during incidents

#### Board of Directors Focus
- **Objective**: Oversight of cyber risk management and enterprise resilience
- **Exercise**: Review Level 4-5 attacks across all columns
- **Question**: *"Are we satisfied with management's identification and mitigation of cyber risks? How does cyber risk integrate with our overall enterprise risk management?"*
- **Deliverable**: Board cybersecurity oversight framework, risk appetite statement, management reporting requirements
- **Key Metrics**: Cyber risk quantification, security program maturity, incident response effectiveness
- **Oversight Areas**: Budget approval, executive performance on cybersecurity, regulatory compliance, third-party risk

---

## 4. Facilitation Guide

### Pre-Exercise (5 minutes)
1. **Display the Table**: Project the periodic table or share digitally
2. **Brief Introduction**:
   - Explain the structure: *"Columns are attack families, rows are sophistication levels 1-5"*
   - Note the color coding: *"Each family has a unique color"*
   - Highlight the value: *"Real European cases, real defenses"*
3. **State Objective**: *"Today we're using real incidents to test our preparedness"*

### During Exercise
- Use the table as a **visual aid** - participants can see attack relationships
- Reference **case studies** for realism and context
- Check the **defenses** against your current security posture
- Use the **MITRE ATT&CK IDs** (Txxxx) for deeper research
- Encourage participants to **touch the table** - physically or digitally select elements

### Facilitation Tips
- **Start simple**: Begin with Level 1-2 attacks for confidence
- **Escalate gradually**: Move to Level 3-5 as the exercise progresses
- **Encourage cross-talk**: Mix teams to get different perspectives
- **Use the links**: Click through to case study sources for details
- **Timebox discussions**: Keep each phase moving

### Post-Exercise (10-15 minutes)
1. **Document Gaps**: List all identified vulnerabilities
2. **Create Action Items**: Specific, assigned, dated
3. **Schedule Follow-ups**: Next exercise, remediation reviews
4. **Share Findings**: Report to stakeholders

---

## 5. Recommended Starting Points

### For Beginners
- **Social Engineering column**: Relatable, good for awareness training
- **Level 1-2 attacks** across all families: Common threats, build confidence
- **Single family deep dive**: Focus on one area without overwhelming

### For Intermediate Teams
- **Network column**: Technical depth, good for network teams
- **Specific attack chains**: Link multiple families (e.g., phishing → credential compromise → lateral movement)
- **Defense validation**: Check if controls match table recommendations

### For Advanced Teams
- **Level 4-5 attacks only**: State-level threats, complex scenarios
- **Multi-column attack chains**: Sophisticated, realistic threats
- **Defense evasion scenarios**: Attacker bypasses controls
- **Red team vs. blue team**: Competitive, realistic testing

---

## 6. Complete Example: Ransomware Response Exercise

### Session Details
- **Title**: European Ransomware Response Exercise
- **Duration**: 90-120 minutes (extended for full cross-functional participation)
- **Participants**: Security, IT, Legal, Communications, HR, Finance, Customer Success, Executive Leadership, Board (optional)

### Role-Specific Objectives

| Role | Primary Focus | Key Questions | Deliverables |
|------|---------------|---------------|--------------|
| **CEO/CISO** | Enterprise impact, crisis leadership | Which systems are critical? When do we involve external authorities? | Executive decision framework |
| **CFO** | Financial impact, ransomware payment decision | What's the cost vs. impact analysis? What are insurance implications? | Financial impact assessment |
| **Legal** | Compliance, liability, notification obligations | What are our GDPR notification timelines? What data was affected? | Legal incident playbook, notification templates |
| **Communications** | Stakeholder messaging, reputation management | Who needs to know what, and when? What's our media strategy? | Crisis communication plan, template statements |
| **HR** | Employee support, insider threat considerations | How do we support staff? Do we have insider threat indicators? | Employee support protocol, insider threat checklist |
| **Finance** | Payment fraud prevention, vendor management | How do we verify legitimate vs. fraudulent payments? | Payment verification procedures |
| **Customer Success** | Customer trust, service continuity | How do we maintain customer service during the incident? | Customer communication protocol |
| **SOC/IR Team** | Technical detection and response | How do we detect, contain, and eradicate the threat? | Updated IR playbooks, detection improvements |
| **IT Operations** | System recovery and continuity | What's our backup and restoration process? | Recovery plan, business continuity validation |

### Phase 1: Scenario Setup (15 minutes)
- **Attack Chain**: Sm (Smishing) → Cs (Credential stuffing) → Rw (Ransomware)
- **Real Cases**:
  - FluBot: SMS-based malware spreading across Europe (2021-2022)
  - Great Western Railway: Credential stuffing via reused passwords (2018)
  - Picanol: Ransomware stopping production for a week (2020)
- **Scenario**: *"Attackers used SMS phishing to deliver malware to employee mobile devices. The malware harvested credentials from browsers, which were then used to access internal systems and deploy ransomware. Production systems are encrypted, and the attackers are demanding payment. Initial analysis suggests customer data may have been exfiltrated before encryption."*

### Phase 2: Detection & Assessment (25 minutes)
**Technical Track (SOC/IT)**:
- How would we detect the initial Smishing attempt?
- Do we have mobile device monitoring?
- Do we monitor for credential stuffing patterns?
- Do we have ransomware-specific detection (file encryption, unusual processes)?
- Are our logs centralized and correlated?
- What data may have been accessed or exfiltrated?

**Legal Track**:
- What data types are affected? (PII, financial, intellectual property)
- Do we have data classification and inventory to answer this quickly?
- What are our GDPR notification timelines (72 hours) and requirements?
- Which regulatory bodies need notification?

**Business Track (CFO/Finance/Customer Success)**:
- What systems are affected and what's their business value?
- What's the potential financial impact of downtime?
- What are our contractual obligations to customers?
- Do we have cyber insurance and what does it cover?

**Document**: Current detection capabilities, data classification gaps, financial impact preliminary assessment

### Phase 3: Immediate Response (30 minutes)
**Technical Response (SOC/IR/IT)**:
- Initial triage and severity assessment
- Containment actions (isolate systems, block IPs, network segmentation)
- Evidence collection and preservation
- Forensic investigation priorities

**Legal & Compliance Response**:
- Data breach assessment and legal obligations
- Regulatory notification planning and timeline
- Contract review (customer contracts, vendor agreements)
- Insurance claim preparation

**Communications Response**:
- Internal communication: Who gets notified first? What's the message?
- External communication: When and how do we notify customers?
- Media strategy: Holding statements, spokesperson designation
- Social media monitoring and response

**HR Response**:
- Employee notification and support
- Insider threat assessment (any suspicious internal activity?)
- Remote work considerations if systems are down
- Mental health and support resources

**Finance Response**:
- Payment verification: Are any recent payments fraudulent?
- Ransomware payment decision framework (pay vs. don't pay)
- Cost tracking: Incident response costs, downtime costs
- Vendor notification and support coordination

**Customer Success Response**:
- Customer notification strategy and timeline
- Service level impact assessment
- Support capacity during incident
- Trust restoration planning

**Executive Leadership Response**:
- Crisis leadership and decision-making
- Board notification (if applicable)
- External authority engagement (law enforcement, regulators)
- Business continuity activation

**Document**: Response playbook gaps, communication plan updates, financial impact tracking sheet, legal notification timeline

### Phase 4: Recovery & Business Continuity (25 minutes)
**Discussion Questions**:
- **Technical**: What's our backup verification process? What's the restoration priority order? How do we verify systems are clean before restoration?
- **Business**: How do we maintain operations during recovery? What's our business continuity plan activation?
- **Legal**: What legal holds need to be in place during investigation? What evidence needs preservation?
- **Communications**: What's our communication cadence during recovery? How do we message progress?
- **HR**: How do we support employees during extended recovery? Any lessons for remote work policies?
- **Finance**: How do we track and recover costs? What financial controls need strengthening?
- **Customer Success**: How do we update customers on progress? What support do they need?

**Document**: Recovery plan improvements, business continuity validation, updated communication templates

### Phase 5: Lessons Learned & Improvements (25 minutes)
**Cross-Functional Discussion**:
- What worked well across teams?
- Where were the coordination gaps?
- What processes need updating?
- What training is needed for each role?

**Action Items Example**:
| Gap | Owner | Action | Due Date | Priority |
|-----|-------|--------|----------|----------|
| No SMS filtering | Security Team | Implement SMS gateway filtering | 2 weeks | High |
| Incomplete log correlation | SOC | Configure SIEM for cross-stage correlation | 1 month | High |
| No ransomware playbook | IR Team | Develop ransomware-specific playbook | 2 weeks | High |
| Missing GDPR notification template | Legal | Create breach notification templates | 1 week | High |
| No executive crisis communication plan | Communications | Develop crisis communication framework | 2 weeks | High |
| Employee support protocol incomplete | HR | Update employee support and insider threat procedures | 2 weeks | High |
| Payment verification gaps | Finance | Implement dual-approval for payment changes | 1 week | High |
| Customer notification timeline unclear | Customer Success | Define customer notification SLAs | 2 weeks | High |

---

## 7. Cross-Functional Exercise Planning

### Why Cross-Functional Participation Matters

Cyber incidents don't respect organizational boundaries. A ransomware attack impacts:
- **Technology**: Systems, data, infrastructure
- **Legal**: Compliance, liability, notifications
- **Finance**: Costs, insurance, payments
- **Operations**: Business continuity, supply chain
- **People**: Employees, customers, partners
- **Reputation**: Brand, trust, market position

**Best Practice**: Include at least one representative from each major function in every tabletop exercise. For advanced exercises, include the full cross-functional team.

### Recommended Participant Mix by Exercise Type

| Exercise Type | Technical Roles | Business Roles | Duration |
|---------------|------------------|----------------|----------|
| **Awareness Training** | Security team (facilitator) | All employees | 30-45 min |
| **Technical Deep Dive** | SOC, IR, IT, Developers | - | 60-90 min |
| **Department-Specific** | Security team (facilitator) | One department (e.g., Finance, HR) | 45-60 min |
| **Cross-Functional** | SOC, IR, IT | Legal, Communications, Finance, HR, Customer Success | 90-120 min |
| **Executive/Board** | CISO (facilitator) | CEO, CFO, COO, CIO, Board | 60-90 min |
| **Full Enterprise** | All technical roles | All business functions + Executive + Board | 120-180 min |

### Facilitating Cross-Functional Exercises

**Pre-Exercise**:
- **Brief all participants** on their role-specific objectives (use Section 3 as reference)
- **Provide pre-reading**: Attack scenarios, relevant case studies from the periodic table
- **Assign pre-work**: Each function reviews their current capabilities against the scenario
- **Set expectations**: Different roles have different priorities and languages - facilitate translation

**During Exercise**:
- **Use breakout groups** for role-specific discussions before reconvening
- **Assign a scribe** from each function to document gaps and action items
- **Timebox each phase** but allow flexibility for deep dives when valuable
- **Encourage challenges**: "Legal, how would you respond to that? Finance, what's the cost?" 
- **Track dependencies**: Note when one team's action depends on another's decision

**Post-Exercise**:
- **Consolidate action items** from all functions into a single tracking sheet
- **Identify cross-functional gaps**: Where did coordination break down?
- **Schedule follow-ups**: Role-specific deep dives on identified gaps
- **Report to leadership**: Consolidated findings with business impact context

### Common Coordination Gaps to Test

| Gap Area | Example Questions | Roles Involved |
|----------|-------------------|----------------|
| **Detection to Response Handoff** | When does IT/Security notify Legal/Communications? What triggers the escalation? | SOC → Legal, Communications |
| **Incident Classification** | Who decides if an event is a "breach" requiring notification? What's the threshold? | Security, Legal, Executive |
| **Communication Timing** | When do we go public? Who approves external statements? | Communications, Legal, Executive |
| **Financial Authority** | Who can authorize emergency spending? What's the approval chain? | Finance, Executive, IT |
| **Employee Support** | How do we inform and support employees during an incident? | HR, Communications, IT |
| **Customer Notification** | Who decides when and how to notify customers? What do we say? | Customer Success, Legal, Communications |
| **Vendor Management** | How do we notify and coordinate with vendors during an incident? | Procurement, IT, Legal |
| **Business Continuity** | Who decides what systems to prioritize for recovery? | Operations, IT, Executive |

### Sample Cross-Functional Exercise Agenda (120 minutes)

| Time | Phase | Activity | Facilitator Focus |
|------|-------|----------|-------------------|
| 0:00-0:10 | **Kickoff** | Scenario presentation, role objectives | Ensure all participants understand their focus |
| 0:10-0:25 | **Breakout: Role-Specific Assessment** | Each function assesses scenario independently | Circulate between groups, answer questions |
| 0:25-0:45 | **Reconvene: Cross-Functional Discussion** | Share assessments, identify gaps | Facilitate understanding across perspectives |
| 0:45-1:15 | **Breakout: Coordinated Response Planning** | Groups plan coordinated response | Encourage inter-group communication |
| 1:15-1:45 | **Reconvene: Full Response Walkthrough** | Test end-to-end coordination | Identify handoff points and dependencies |
| 1:45-2:00 | **Action Items & Close** | Document gaps, assign owners, set timelines | Ensure clarity on next steps |

---

## 8. Exercise Tracking Sheet Template

Use this template to document exercise results:

```markdown
## Tabletop Exercise: [Name]
**Date**: [YYYY-MM-DD]  
**Facilitator**: [Name]  
**Participants**: [List]  
**Duration**: [Minutes]

### Scenario
- **Attack Elements**: [List symbols and names]
- **Case Studies**: [Links to real cases]
- **Attack Story**: [Brief narrative]

### Findings

| # | Attack | Case Study | Detection Capability | Response Readiness | Gap | Owner | Action | Due |
|---|--------|------------|---------------------|-------------------|-----|-------|--------|-----|
| 1 | Phishing | Maastricht University | ✅ Email filtering | ✅ IR playbook | User awareness | HR | Training | 2 weeks |
| 2 | Smishing | FluBot | ❌ No SMS monitoring | ⚠️ Partial | SMS gateway | Security | Implement | 1 month |
| 3 | Ransomware | Picanol | ✅ EDR alerts | ✅ Backups | Playbook | IR Team | Update | 2 weeks |

### Action Items
1. [ ] Implement SMS filtering - Security Team - 2 weeks
2. [ ] Update ransomware IR playbook - IR Team - 2 weeks
3. [ ] Conduct follow-up exercise - All - 1 month

### Lessons Learned
- [Lesson 1]
- [Lesson 2]
- [Lesson 3]

### Next Steps
- [ ] Schedule follow-up exercise
- [ ] Review action items in 2 weeks
- [ ] Share findings with leadership
```

---

## 8. Quick Reference: Attack Family Guide

Use this guide to quickly select exercises based on team focus.

### Attack Families for Non-Technical Roles

#### Best Attack Families for Cross-Functional Exercises

| Attack Family | Why It's Good for Cross-Functional | Key Roles to Include |
|---------------|-----------------------------------|----------------------|
| **Impact (imp)** | Direct business impact, requires coordination across all functions | Executive, Legal, Communications, Finance, HR, Customer Success |
| **Social Engineering (soc)** | Human factors, requires awareness and process controls | HR, Legal, Finance, Communications, All employees |
| **Supply Chain & Cloud (sup)** | Third-party risk, contractual and operational implications | Procurement, Legal, Finance, Operations, Executive |
| **Advanced & State-Level (adv)** | Strategic threats requiring executive decision-making | Executive, Board, Legal, Communications, Security |
| **Credentials & Identity (cred)** | Access control affecting all business functions | IT, HR, Finance, Legal, Customer Success |

#### Attack Families for Specific Business Functions

| Business Function | Primary Attack Families | Secondary Attack Families | Exercise Focus |
|-------------------|------------------------|---------------------------|----------------|
| **Legal** | Impact, Social Engineering | Supply Chain, Advanced | Compliance, notifications, liability |
| **Communications** | Impact, Social Engineering | Advanced, Web Applications | Crisis communication, reputation |
| **HR** | Social Engineering, Credentials | Impact, Advanced | Employee awareness, insider threat |
| **Finance** | Impact, Social Engineering | Supply Chain, Credentials | Financial controls, payment fraud |
| **Customer Success** | Impact, Web Applications | Social Engineering, Supply Chain | Customer trust, service continuity |
| **Procurement** | Supply Chain, Credentials | Impact, Network | Vendor risk, third-party security |
| **Operations** | Impact, Supply Chain | Network, Advanced | Business continuity, operational resilience |

### Social Engineering (soc)
- **Theme**: Human manipulation
- **Good for**: Security awareness, phishing training, HR training, financial fraud prevention
- **Attack Types**: Phishing, Smishing, Vishing, Pretexting, Spear phishing, CEO fraud, Deepfake
- **Best Exercise**: User awareness training, email security validation, financial approval process testing

### Credentials & Identity (cred)
- **Theme**: Authentication attacks
- **Good for**: IAM teams, identity security, HR (password policies), Finance (payment approvals)
- **Attack Types**: Brute force, Credential stuffing, Password spraying, MFA fatigue, Token phishing, Session hijacking
- **Best Exercise**: Identity provider security, MFA strategy validation, financial approval workflow testing

### Malware (mal)
- **Theme**: Malicious software
- **Good for**: Endpoint security, EDR teams, HR (employee device policies), Legal (forensic evidence)
- **Attack Types**: Trojan, Infostealer, Worm, Fileless malware, Rootkit
- **Best Exercise**: Endpoint detection and response, malware analysis, employee device security policies

### Web Applications (web)
- **Theme**: Web-based vulnerabilities
- **Good for**: Developers, application security, Customer Success (customer-facing apps), Legal (data protection)
- **Attack Types**: XSS, SQL injection, Path traversal, SSRF, RCE
- **Best Exercise**: Secure coding, application hardening, customer data protection

### Network (net)
- **Theme**: Network-level attacks
- **Good for**: Network engineering, infrastructure teams, Operations (business continuity), IT (service availability)
- **Attack Types**: Interception, DDoS, MITM, DNS hijacking, BGP hijacking
- **Best Exercise**: Network security, traffic monitoring, service availability planning

### Supply Chain & Cloud (sup)
- **Theme**: Third-party and cloud risks
- **Good for**: Procurement, cloud security, Legal (contracts), Finance (vendor management), Operations (supply chain)
- **Attack Types**: Cloud misconfiguration, Typosquatting, Dependency confusion, Container escape, Software supply chain
- **Best Exercise**: Vendor risk management, cloud security posture, third-party contractual obligations

### Impact (imp)
- **Theme**: Direct damage/impact
- **Good for**: Incident response, business continuity, Executive (decision-making), Legal (breach notification), Communications (crisis management), Finance (cost analysis), Customer Success (customer impact)
- **Attack Types**: Cryptojacking, Defacement, Ransomware, Data extortion, Wiper
- **Best Exercise**: Full cross-functional incident response, business continuity testing, crisis communication
- **Best Exercise**: Incident response, disaster recovery

### Lateral Movement & Persistence (lat)
- **Theme**: Post-compromise activity
- **Good for**: SOC, threat hunting, IT (system access), HR (privileged access), Legal (forensic investigation)
- **Attack Types**: Remote tool abuse, Credential reuse, Kerberoasting, Living off the land, Golden ticket, Token forgery
- **Best Exercise**: Threat detection, lateral movement prevention, privileged access management

### Advanced & State-Level (adv)
- **Theme**: Sophisticated threats
- **Good for**: Executive, security strategy, Board (oversight), Legal (national security implications), Communications (reputation management)
- **Attack Types**: Insider threat, Watering hole, Cyber espionage, Zero-day, Zero-click spyware, Firmware rootkit, Industrial sabotage
- **Best Exercise**: Strategic planning, nation-state threat response, executive crisis simulation

### AI & Machine Learning (ai)
- **Theme**: AI-specific attacks
- **Good for**: AI/ML teams, data science, Legal (IP protection), Customer Success (AI product security), Communications (responsible AI messaging)
- **Attack Types**: Jailbreak, Prompt injection, AI agent hijacking, Malicious model files, Adversarial examples, Model extraction, Data poisoning
- **Best Exercise**: AI security, model protection, responsible AI governance

### Physical & Proximity (phy)
- **Theme**: Physical security
- **Good for**: Facilities, physical security, HR (employee safety), IT (device security), Legal (incident response)
- **Attack Types**: Tailgating, Infected USB drives, Rogue Wi-Fi, Badge cloning, Bluetooth exploit, Hardware implant, Side-channel attack
- **Best Exercise**: Physical security controls, access control, workplace safety

---

## 9. Tips for Success

### Facilitator Tips
- **Prepare**: Read through the selected case studies beforehand
- **Stay Flexible**: Allow discussions to go deeper if valuable
- **Keep it Real**: Reference your organization's actual systems and controls
- **Document Everything**: Capture all gaps and action items
- **Follow Up**: Schedule reviews of action items
- **Translate Across Functions**: Help technical and non-technical participants understand each other's perspectives and requirements

### Participant Tips for Technical Roles
- **Be Honest**: If you don't know, say so - that's the point
- **Think Holistically**: Consider business impact, not just technical details
- **Ask Questions**: Use the facilitator and other participants as resources
- **Stay Engaged**: These are real threats that have happened in Europe
- **Explain Simply**: Help non-technical colleagues understand technical concepts and their implications

### Participant Tips for Business Roles
- **Embrace the Unknown**: Cybersecurity has its own language - ask for clarification when needed
- **Share Business Context**: Help technical teams understand business priorities, constraints, and impact
- **Think Cross-Functionally**: Consider how your function's response affects and depends on other teams
- **Challenge Assumptions**: "What if our primary payment system is down?" "What if we can't notify customers for 24 hours?"
- **Stay Solution-Focused**: Focus on what needs to happen, not just what went wrong

### Organization Tips
- **Start Small**: 30-minute exercises with small groups
- **Build Momentum**: Regular exercises (monthly or quarterly)
- **Mix It Up**: Try different templates and approaches
- **Measure Progress**: Track improvements over time
- **Share Results**: Report findings to leadership (without blame)
- **Rotate Participants**: Give different team members exposure to cybersecurity thinking
- **Executive Sponsorship**: Ensure leadership participates and supports the program

---

## 10. Resources

### Original Materials
- [The Periodic Table of Cyber Attacks](./index.html)
- [Source on GitHub](https://github.com/theshellcompany/PeriodicTableOfCyberAttacks)

### Referenced Frameworks
- **MITRE ATT&CK**: [attack.mitre.org](https://attack.mitre.org) - For detailed attack techniques
- **MITRE ATLAS**: [atlas.mitre.org](https://atlas.mitre.org) - For AI/ML attack patterns
- **CWE**: [cwe.mitre.org](https://cwe.mitre.org) - For software weakness classifications

### European Cybersecurity Resources
- **ENISA**: [enisa.europa.eu](https://www.enisa.europa.eu) - EU cybersecurity agency
- **CERT-EU**: [cert.europa.eu](https://cert.europa.eu) - EU institutions CERT
- **NCSC UK**: [ncsc.gov.uk](https://www.ncsc.gov.uk) - UK National Cyber Security Centre

---

## Appendix: Attack Element Quick Reference

All 79 attack techniques organized by family and sophistication:

| Sym | Name | Family | Level | MITRE ID |
|-----|------|--------|-------|----------|
| Ph | Phishing | Social Engineering | 1 | T1566 |
| Sm | Smishing | Social Engineering | 1 | T1660 |
| Vi | Vishing | Social Engineering | 2 | T1566.004 |
| Pt | Pretexting | Social Engineering | 2 | T1598 |
| Sp | Spear phishing | Social Engineering | 3 | T1566.001 |
| Be | CEO fraud / BEC | Social Engineering | 3 | T1656 |
| Df | Deepfake impersonation | Social Engineering | 4 | T1656 |
| Bf | Brute force | Credentials | 1 | T1110.001 |
| Cs | Credential stuffing | Credentials | 1 | T1110.004 |
| Ps | Password spraying | Credentials | 2 | T1110.003 |
| Mf | MFA fatigue | Credentials | 2 | T1621 |
| Ao | Token phishing | Credentials | 3 | T1528 |
| Sh | Session hijacking | Credentials | 3 | T1539 |
| Tj | Trojan | Malware | 2 | T1204.002 |
| Is | Infostealer | Malware | 2 | T1555 |
| Wm | Worm | Malware | 3 | T1210 |
| Fm | Fileless malware | Malware | 4 | T1059.001 |
| Rk | Rootkit | Malware | 4 | T1014 |
| Xs | Cross-site scripting | Web | 2 | CWE-79 |
| Sq | SQL injection | Web | 2 | CWE-89 |
| Tr | Path traversal | Web | 2 | CWE-22 |
| Sr | Server-side request forgery | Web | 3 | CWE-918 |
| Rc | Remote code execution | Web | 4 | CWE-917 |
| Sn | Interception | Network | 1 | T1040 |
| Dd | DDoS | Network | 2 | T1498 |
| Mi | Man-in-the-middle | Network | 3 | T1557 |
| Dn | DNS hijacking | Network | 4 | T1584.002 |
| Bg | BGP hijacking | Network | 5 | - |

*(Complete list available in the HTML files)*

---

## License & Usage

This framework is provided as-is for cybersecurity education and preparedness. You are free to:
- Use it for internal exercises
- Modify it for your needs
- Share it with attribution

Please credit the original Periodic Table of Cyber Attacks and maintain the European focus when sharing.

---

*Created: 2026-10-09*  
*Last Updated: 2026-10-09*  
*Version: 2.0 - Expanded with C-level, Communications, Legal, and Business Function roles*
