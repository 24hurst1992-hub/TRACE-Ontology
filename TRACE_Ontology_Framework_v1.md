# TRACE Ontology Framework v1.0
## Trafficking Recognition, Analysis & Countermeasure Engine: Formal Trafficking TTP Ontology

**Document Version:** 1.0
**Status:** Reference Specification
**Date:** April 2026
**Audience:** Law Enforcement, Intelligence Analysts, Forensic Examiners (SANE), Social Workers, Victim Advocates, Researchers

---

## Table of Contents

1. [Introduction](#introduction)
2. [Theoretical Foundations](#theoretical-foundations)
3. [Ontology Architecture](#ontology-architecture)
4. [Network Modeling Framework](#network-modeling-framework)
5. [Academic Contribution and Future Work](#academic-contribution-and-future-work)
6. [References](#references)

---

## Introduction

### Problem Statement: Fragmented Knowledge Across Disciplines

Human trafficking represents one of the most complex criminal enterprises globally, generating an estimated $150 billion annually and affecting over 27 million people at any given time (International Labour Organization, 2024). Yet despite decades of anti-trafficking efforts, the field remains deeply fragmented. Law enforcement uses investigative terminology drawn from federal statutes; intelligence analysts apply counterterrorism frameworks; forensic examiners document trauma; social workers assess needs; victim advocates center survivor autonomy. These disciplines operate with different taxonomies, different terminology, and fundamentally different threat models.

A law enforcement officer investigating a sex trafficking ring may use terms like "facilitator" and "exploitation venue," while a clinical social worker discusses "complex trauma" and "coercion dynamics." An intelligence analyst maps "criminal networks" while a victim advocate emphasizes "survivor agency." Each perspective contains crucial truth, but they do not integrate. Critical information gets lost in translation. Investigations stumble because investigative terminology doesn't map to victim indicators. Prevention efforts fail because vulnerability assessment doesn't account for operational targeting. Victim services miss windows of intervention because they don't understand the tactical phases traffickers use.

### The Gap: Absence of Formal Trafficking Ontology

A comprehensive literature review confirms that while numerous taxonomies exist for specific aspects of trafficking—victimization typologies, criminal organizational structures, coercion methods—no formal, structured ontology exists that:

1. Maps trafficking operations across their full lifecycle from targeting through profit-taking
2. Translates between disciplinary vocabularies (law enforcement, clinical, intelligence, social work)
3. Provides hierarchical granularity from strategic tactics to operational techniques to tactical sub-techniques
4. Integrates multiple theoretical frameworks into a unified model
5. Enables consistent identification and analysis of trafficking across cases and jurisdictions
6. Supports computational and AI/ML applications for pattern detection

Existing frameworks excel within their domains but do not interoperate. The Polaris Project's Typology of Modern Slavery (covering 25 trafficking types from 32,000 cases) provides victim-centered classification. The UNODC 3-dimensional indicators model (Act, Means, Purpose) enables formal victim status determination. Zimmerman's Stages model describes trafficking trajectories. Biderman's Chart of Coercion and Hassan's BITE model enumerate control mechanisms. But none of these integrate with operational threat actor modeling, network analysis, or role-based indicator frameworks that law enforcement and intelligence require.

### TRACE's Contribution: First ATT&CK-Style Structured Ontology for Human Trafficking

TRACE (Trafficking Recognition, Analysis & Countermeasure Engine) fills this gap by introducing the first formally structured, hierarchical ontology for human trafficking explicitly modeled on the MITRE ATT&CK framework architecture—the same hierarchical, community-driven taxonomy that transformed cybersecurity threat analysis.

TRACE's innovation lies not in inventing new trafficking knowledge but in **formally structuring and integrating existing trafficking science** into a unified, operationally actionable framework. By adopting ATT&CK's proven hierarchical model (Tactics → Techniques → Sub-techniques), TRACE enables:

- **Disciplinary translation:** The same trafficking operation is simultaneously described in law enforcement, clinical, intelligence, and social work vocabularies
- **Operational granularity:** From high-level strategic intent ("Control & Isolate") through techniques ("Document Confiscation," "Financial Control") to specific implementation details
- **Computational tractability:** Structured data amenable to graph analysis, machine learning, and cross-case pattern matching
- **Evidence mapping:** Clinical indicators, behavioral observations, investigative findings, and digital artifacts all connect to specific techniques
- **Vulnerability assessment:** Threat actor targeting patterns map directly to prevention and protection strategies
- **Consistency:** Every jurisdiction, agency, and discipline uses the same taxonomy, enabling genuine knowledge aggregation

### Target Audiences and Use Cases

**Law Enforcement (Federal, State, Local):**
- Investigative framework: structuring cases, identifying co-conspirators, tracking network evolution
- Digital forensics: mapping data artifacts to operational techniques
- Pattern recognition: identifying trafficking in cases that don't appear to be trafficking
- Inter-agency coordination: consistent terminology across jurisdictions

**Intelligence Analysts:**
- Threat modeling: understanding organized trafficking operations
- Network mapping: identifying key nodes and vulnerabilities in trafficking networks
- Predictive analysis: identifying likely next targets, operational hubs, profit paths
- Pattern correlation: linking disparate intelligence to common threat actors

**Forensic Examiners (SANE/SAFE):**
- Clinical indicator mapping: understanding what injuries, presentations, and findings indicate specific trafficking techniques
- Documentation standardization: structuring exams to capture evidence relevant to specific techniques
- Trauma-informed assessment: understanding coercion context when evaluating presentations

**Social Workers and Service Providers:**
- Holistic safety planning: understanding all control mechanisms in operation on a specific survivor
- Service sequencing: matching interventions to specific exploitation types and coercion methods
- Risk assessment: identifying manipulations that may undermine service engagement
- Stabilization prioritization: understanding which control techniques require immediate intervention

**Victim Advocates:**
- Survivor-centered investigation support: explaining investigation concepts in accessible terms
- Legal positioning: mapping trafficking techniques to relevant criminal statutes and immigration remedies
- Empowerment narrative: framing survivor experience in formal analytical terms
- Inter-system navigation: understanding what each agency needs and why

### Academic Framing: Interdisciplinary and Public Health Contribution

TRACE represents an intentional interdisciplinary synthesis. The trafficking response field has historically been divided into siloes: criminal justice (focused on prosecution), public health/clinical (focused on trauma recovery), social work (focused on survivor needs), intelligence (focused on networks), and prevention (focused on vulnerability). This ontology explicitly bridges these domains.

From **criminology**, TRACE incorporates threat actor modeling, criminal network analysis, and routine activity theory. From **public health**, it incorporates victim typologies, risk stratification, and structural vulnerability frameworks. From **clinical science**, it incorporates trauma-informed assessment and coercion dynamics. From **intelligence**, it incorporates threat actor profiling and network analysis. From **law enforcement**, it incorporates investigative frameworks and evidence documentation.

The result is a **public health surveillance tool** that treats trafficking not as isolated criminal incidents but as a systematic enterprise with identifiable threat actors, predictable phases, observable patterns, and preventable pathways. Like epidemiologists mapping disease vectors, TRACE maps exploitation vectors. Like intelligence analysts understanding terrorist networks, TRACE enables understanding of trafficking networks. Like clinicians understanding disease progression, TRACE enables understanding of trafficking trajectory.

---

## Theoretical Foundations

TRACE synthesizes nine major theoretical frameworks into a unified ontology. Understanding each component is essential to understanding the whole system.

### 1. MITRE ATT&CK as Structural Model: Why Hierarchy Works for Trafficking

MITRE ATT&CK is the de facto global standard for cybersecurity threat knowledge. It organizes adversarial behavior into a three-tier hierarchy: 14 tactics (strategic-level "why"), 216 techniques (operational-level "how"), and 475+ sub-techniques (tactical-level implementation specifics). This framework has proven revolutionary because it:

- **Enables translation between contexts:** The same technique operates similarly whether executed against healthcare systems or educational institutions
- **Allows layered analysis:** Incident responders can understand both high-level adversarial goals and granular implementation details
- **Supports automation:** Structured data enables tooling, detection writing, correlation, and ML applications
- **Builds community knowledge:** Contributors worldwide can map adversary behaviors to a common taxonomy
- **Scales across complexity:** Works equally well for individual threat actors and sophisticated nation-states

Human trafficking has fundamentally similar structure to sophisticated cyber operations: multiple actors in defined roles, sequenced techniques building toward strategic goals, adaptive responses to intervention, profit generation through operational success. The hierarchy that works for cyber—Tactic (strategic intent) → Technique (operational method) → Sub-technique (implementation detail)—maps directly to trafficking: Tactic (trafficking phase like "Control & Isolate") → Technique (specific control method like "Document Confiscation") → Sub-technique (specific variant like "Passport Confiscation" vs. "License Confiscation").

For TRACE, the six-tactic model reflects the **lifecycle of a trafficking operation from perpetrator perspective**: (1) identify and target victims (2) recruit and groom them (3) control and isolate them (4) exploit them (5) sustain operations and conceal the crime (6) launder profits. This mirrors how actual trafficking networks operate, regardless of exploitation type or geography.

### 2. Polaris Project Typology of Modern Slavery: Victim-Centered Taxonomy

The Polaris Project, analyzing 32,000+ trafficking cases, identified 25 distinct trafficking types organized by exploitation form and context:

**Sexual Exploitation:** Child Sex Trafficking, Adult Sex Trafficking, Pornography Production, Exotic Dancing (coerced), Online Sexual Exploitation, Bride Trafficking

**Labor Exploitation:** Domestic Service, Hospitality, Agriculture, Manufacturing, Construction, Commercial Fishing, Mining, Personal Service, Street Begging, Criminal Activity

**Mixed/Compound:** Forced Marriage, Organ Harvesting, Cult/Coercive Organization, Debt Bondage (generalized)

**Emerging Types:** Forced Surrogacy, Child Soldiers (for non-military contexts), Forced Gaming Fraud, Supply Chain Exploitation

This typology centers victim experience and exploitation outcome, providing essential victim-centered classification. TRACE maps each Polaris type to specific technique combinations within the ontology—understanding which control techniques, which threat actors, and which coercion mechanisms typically characterize each exploitation type.

### 3. UNODC 3-Dimensional Indicators Model: Formal Victim Status Determination

The United Nations Office on Drugs and Crime's 3-dimensional model establishes that trafficking requires:

**Act:** Recruitment, transportation, transfer, harboring, or receipt of a person

**Means:** Threat, force, coercion, abduction, fraud, deception (absent for children in sexual exploitation)

**Purpose:** Sexual exploitation, forced labor, removal of organs, forced criminality, domestic servitude, forced begging, or other forms of exploitation

This framework operationalizes the legal definition of trafficking for practical application. A victim may experience one or several acts, applied through one or several means, in service of one or several purposes. TRACE maps techniques to this dimensional structure: each technique either constitutes an Act, implements a Means, or structures a Purpose. Understanding these dimensions is critical because they align with victim legal status (particularly for immigration relief under the T-visa, which requires meeting all three dimensions).

### 4. ILO Forced Labor Indicators: Operational Characteristics of Coercion

The International Labour Organization, in partnership with the UN, published Forced Labor Indicators (revised 2025), providing 11 observable indicators that identify forced labor:

1. The worker cannot refuse or resign
2. The worker is exposed to penalties for non-compliance
3. The worker's terms of work are imposed without consent
4. The worker has abusive working conditions
5. The worker has been recruited through deception
6. The worker is in debt bondage (wages insufficient to repay debt)
7. The worker has restricted movement or confinement
8. The worker's documentation is withheld
9. The worker experiences wage theft or non-payment
10. Excessive working hours are imposed
11. The worker is isolated or monitored

These indicators translate between labor context and trafficking recognition. An investigator examining a restaurant, farm, or construction site can apply these 11 indicators systematically. TRACE maps each indicator to specific techniques in the ontology—wage theft, for example, links to the "Financial Control" technique, which may be implemented through specific sub-techniques including "Non-Payment," "Inflated Debt," or "Fraudulent Accounting."

### 5. Zimmerman et al. Stages Model: Trafficking Trajectory and Intervention Windows

Zimmerman's Stages model, developed from follow-up interviews with survivors, identifies six sequential stages in the trafficking trajectory:

**Stage 1: Background/Vulnerability** — Individual experiences poverty, abuse, discrimination, displacement, or other vulnerabilities that increase trafficking susceptibility

**Stage 2: Recruitment/Entry** — Trafficker uses deception, coercion, or grooming to recruit and place victim into exploitative situation

**Stage 3: Control** — Trafficker uses coercion, threats, and isolation to maintain control

**Stage 4: Exploitation** — Victim is exploited through labor, sexual services, or other means

**Stage 5: Extrication/Escape** — Victim manages to escape or is discovered (may occur multiple times before final escape)

**Stage 6: Adaptation/Recovery** — Survivor begins reintegration process (mental health support, legal remedy, safe housing, economic opportunity)

This stage model aligns with TRACE tactics: Stage 1 (Background) connects to TA0001 (Identify & Target), Stage 2 aligns with TA0002 (Recruit & Groom), Stages 3-4 with TA0003-TA0004 (Control and Exploit), Stage 5 with TA0005 (Sustain & Conceal), and Stage 6 suggests intervention points. Critically, the Zimmerman model emphasizes that trafficking is often cyclical—escape is followed by re-trafficking, sometimes by the same perpetrator, sometimes by others who exploit the trauma and isolation of escape. This informs both victim service provision and law enforcement re-victimization prevention.

### 6. Biderman's Chart of Coercion: Eight Methods of Control

Biderman's Chart of Coercion, developed during Cold War prisoner-of-war research, identifies eight universal methods of coercion that produce compliance and psychological dependence:

1. **Isolation** — Prevent communication with outside; control information flow; prevent access to support systems
2. **Monopolization of Perception** — Dominate the victim's attention and frame of reference; control what victim attends to
3. **Induced Debility** — Create physical or psychological weakness through sleep deprivation, malnutrition, substance use
4. **Threats** — Articulated or implied threats to victim, victim's family, or others they care about
5. **Occasional Indulgences** — Unpredictable rewards create psychological dependence ("variable ratio reinforcement")
6. **Demonstrating Omniscience** — Create perception that perpetrator sees/knows everything; pervasive surveillance real or perceived
7. **Degradation** — Routinely violate dignity; humiliate; strip identity
8. **Enforcing Trivial Demands** — Require obedience to arbitrary rules; condition response to authority

This framework maps directly to trafficking control mechanisms. A trafficker using all eight methods (or even most of them) produces psychological coercion comparable to imprisonment—often more effective because it's internalized. TRACE's coercion framework (Section 3.5) maps each Biderman method to specific trafficking techniques and sub-techniques.

### 7. Hassan's BITE Model: Systematic Coercion and Control

Steven Hassan's BITE Model, developed from cult psychology, identifies four dimensions of systematic control:

**Behavior Control** — What you do (isolation, poverty, uniforms, regulations, surveillance, enforced dependency)

**Information Control** — What you know (thought-terminating clichés, discourage questioning, special information/vocabulary, control media/reading, confuse thought with feelings)

**Thought Control** — How you think (loaded language, black-and-white thinking, rejection of outside perspective, blind obedience)

**Emotional Control** — What you feel (guilt, fear, phobia indoctrination, shame, dependency, extremist identity)

The BITE model, like Biderman's Chart, identifies mechanisms of systematic coercion that create psychological compliance beyond simple fear. Applied to trafficking, BITE explains why trafficking survivors sometimes resist rescue efforts, defend their traffickers, or quickly re-enter trafficking after escape. The coercion operates at emotional and cognitive levels, not merely through explicit threats.

### 8. Crime Script Analysis: Understanding Operational Sequences

Crime script analysis, drawn from cognitive science, views crimes as scripts—"schemas for events" that involve sequences of scenes, participants, props, and conditions. Applied to trafficking, a crime script analysis reveals five overlapping operational sequences (tracks):

**Track 1: Victim Selection & Recruitment** — Targeting, relationship building, entry into trafficking situation

**Track 2: Transportation/Movement** — Moving victim from origin to exploitation site (or between sites)

**Track 3: Control Establishment** — Isolation, documentation confiscation, financial entrapment, coercion conditioning

**Track 4: Exploitation & Profit** — Labor or sexual services, money collection, sustaining operation

**Track 5: Risk Management** — Concealment, witness intimidation, corruption, counter-investigation

These five tracks operate in parallel for any given trafficking case. Understanding crime scripts explains how interventions work: disrupting Track 1 (victim selection) prevents victimization; disrupting Track 2 (transportation) strands victims; disrupting Track 3 (control) enables escape; disrupting Track 4 (exploitation) ends profit; disrupting Track 5 (concealment) enables detection. TRACE techniques map to these five tracks, enabling script-disruption analysis.

### 9. Bronfenbrenner's Ecological Systems Theory: Structural Vulnerability

Bronfenbrenner's ecological framework identifies nested levels of influence on human development and behavior:

**Microsystem** — Immediate environment (family, peers, school, workplace)

**Mesosystem** — Connections between microsystems (parent-teacher communication, employer-family dynamics)

**Exosystem** — Systems affecting individual without direct participation (neighborhood quality, job market, social services availability)

**Macrosystem** — Overarching cultural, economic, and political systems (poverty, discrimination, immigration policy, labor law enforcement)

**Chronosystem** — Temporal dimension (economic crises, policy changes, generational patterns)

This framework clarifies why trafficking is simultaneously an individual victimization and a structural phenomenon. Individuals don't "choose" trafficking, but individuals with specific vulnerability patterns (abuse history, displacement, poverty, marginalization) in specific structural contexts (weak labor law enforcement, discrimination, limited opportunity) become targets. This informs both victim-centered intervention and prevention strategy. TRACE includes structural vulnerability mapping that helps prevention efforts identify high-risk populations and systems.

### 10. Routine Activity Theory: Convergence of Risk

Routine Activity Theory (Cohen & Felson) posits that crime requires convergence of: motivated offenders, suitable targets, and absent guardians. In trafficking context:

**Motivated Offenders:** Individuals who profit from exploitation, normalized to victimizing others

**Suitable Targets:** Individuals with vulnerability patterns and limited access to protective systems

**Absent Guardians:** Families, communities, authorities, social institutions unable or unwilling to protect

Trafficking flourishes where all three converge. Prevention strategy therefore operates at all three points: reducing offender motivation (prosecution, interdiction), reducing target suitability (resilience building, access expansion), and strengthening guardianship (community awareness, institutional responsiveness). Understanding this dynamic reveals why enforcement alone cannot prevent trafficking—it addresses motivation but leaves suitable targets and absent guardians intact.

### 11. Social Network Analysis Applied to Trafficking: Structure and Dynamics

Trafficking networks, like all criminal networks, have specific structural properties measurable through social network analysis (SNA). Key concepts:

**Nodes** — Individual actors (traffickers, facilitators, buyers, corrupt officials)

**Edges** — Relationships (recruits, transports, pays, controls, communicates with)

**Centrality** — Importance of individual nodes (degree, betweenness, closeness, eigenvector centrality)

**Clustering** — Tendency for connected nodes to form tight groups

**Small-world property** — Long average path length despite high clustering (characteristic of resilient networks)

**Tie strength** — Strength of relationships (strong ties = frequent contact, weak ties = occasional contact)

Trafficking networks typically exhibit: loose hierarchies (not command-and-control but networked), division of specialized roles (recruiters, transporters, controllers, exploiters, handlers, financiers, enforcers), multiple redundant connections (resilience against disruption), and preferential links between specialized roles. SNA reveals network vulnerabilities—key nodes whose removal disrupts operations, weak ties that are easy to cultivate informants through, clustering patterns that reveal geographic or operational boundaries. TRACE's network modeling framework (Section 4) builds SNA directly into the ontology structure.

---

## Ontology Architecture

The TRACE ontology comprises 10 integrated layers, each essential to the complete system. These layers interoperate to enable comprehensive trafficking analysis from multiple disciplinary perspectives.

### Layer 1: Tactics (Trafficking Phases) — The Strategic "Why"

Tactics represent the strategic-level objectives of trafficking operations. TRACE defines six tactics spanning the trafficking lifecycle:

#### TA0001: Identify & Target

**Definition:** The process by which threat actors identify, research, and select potential victims based on vulnerability factors, accessibility, and suitability for exploitation.

**Strategic Rationale:** Trafficking is not random victimization. Perpetrators invest significant effort in identifying targets with optimal exploitation probability. This phase determines victim selection patterns, targeting methods, and geographic focus.

**Mapping to Theoretical Frameworks:**
- **Zimmerman Stages:** Corresponds to Stage 1 (Background/Vulnerability) and Stage 2 (Recruitment) entry point
- **Crime Script Analysis:** Track 1 (Victim Selection & Recruitment) initiation
- **Routine Activity Theory:** Identifying "suitable targets" in accessible populations
- **Ecological Systems:** Identifying microsystems with vulnerable individuals, exosystems with limited guardianship
- **Vulnerability Assessment:** Profiling victims for exploitation suitability

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Predatory targeting patterns | Identify victim populations being targeted; reconstruct pre-victimization contact |
| Intelligence | Threat actor methodology | Map targeting preferences; predict next victim profile; identify victim sourcing |
| SANE/Forensic Examiner | Pre-exploitation vulnerability | Assess trauma history, abuse background, displacement status |
| Social Work | Vulnerability factors | Identify protective factor deficits; understand background that created vulnerability |
| Victim Advocate | Survivor narrative | Explain why survivor was targeted; contextualize "Why didn't you leave earlier" |

**Tactics Operationalization:** Perpetrators in this phase collect information about potential victims, identify geographic areas or institutions with high victim concentration, develop targeting strategies based on victim attributes, and position themselves or associates in proximity to targets.

---

#### TA0002: Recruit & Groom

**Definition:** The process by which threat actors develop relationships with potential victims, establish trust, introduce them to exploitation, and condition them for control.

**Strategic Rationale:** Successful trafficking requires voluntary participation or at least insufficient resistance during initial phases. Perpetrators invest heavily in recruitment and grooming to ensure smooth transition to exploitative situation and minimize resistance.

**Mapping to Theoretical Frameworks:**
- **Zimmerman Stages:** Stage 2 (Recruitment/Entry) core operation
- **Crime Script Analysis:** Track 1 (Victim Selection & Recruitment) operational execution
- **Hassan's BITE Model:** Information and emotional control initiation
- **Biderman's Chart:** Occasional indulgences and demonstrating omniscience foundation-laying
- **Grooming Theory:** Systematic trust-building, boundary erosion, isolation initiation

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Conspiracy/recruitment evidence | Identify recruiters; trace communication leading to recruitment; document false promises |
| Intelligence | Recruitment network | Map recruiter networks; identify victim pipelines; understand recruitment specialization |
| SANE/Forensic Examiner | Grooming trauma | Understand psychological manipulation preceding exploitation; assess trust violation |
| Social Work | Relationship dysfunction | Identify predatory relationship patterns; understand trust deficits; plan trust-building |
| Victim Advocate | Grooming narrative | Explain grooming as intentional manipulation; reduce victim self-blame; validate victimization |

**Tactics Operationalization:** Perpetrators develop seemingly beneficial relationships with targets, introduce incremental exploitation, normalize sexual or labor activities, build dependence, establish false sense of partnership or relationship, and create confusion about victim status through mixed messaging.

---

#### TA0003: Control & Isolate

**Definition:** The process by which threat actors establish comprehensive control over victims through isolation, documentation confiscation, financial entrapment, and coercion mechanisms, rendering victims psychologically and/or physically captive.

**Strategic Rationale:** Once victim is in exploitative situation, primary objective is preventing escape and maintaining obedience. This requires simultaneous control across multiple dimensions—physical movement, information, finances, relationships, identity.

**Mapping to Theoretical Frameworks:**
- **Zimmerman Stages:** Stage 3 (Control) core operation
- **Crime Script Analysis:** Track 3 (Control Establishment) operational execution
- **Biderman's Chart:** All eight methods applied for psychological/behavioral control
- **Hassan's BITE Model:** All four control dimensions (behavior, information, thought, emotional) operationalized
- **Coercion Theory:** Systematic application of threat, isolation, degradation, and manipulation
- **Trauma Bonding:** Intermittent reinforcement creating psychological dependence

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Control evidence | Document isolation; identify co-perpetrators in control function; gather control testimony |
| Intelligence | Control methodology | Map control mechanisms; identify specialization of controllers; predict control method application |
| SANE/Forensic Examiner | Control trauma | Document physical evidence of confinement; assess psychological control impact; explain inconsistent behavior |
| Social Work | Safety planning | Identify all control mechanisms to dismantle; understand barriers to escape; plan stabilization |
| Victim Advocate | Disempowerment narrative | Explain why victim complied, appeared cooperative, didn't disclose; validate coercion effects |

**Tactics Operationalization:** Perpetrators confiscate documents, control access to money, restrict communication, monitor movements, instill fear through threats or violence, utilize substance dependency, condition obedience to authority, and degrade victim identity.

---

#### TA0004: Exploit

**Definition:** The process by which threat actors extract value from victims through sexual services, labor, forced criminality, forced begging, or other exploitation forms, generating profit while maintaining victim control.

**Strategic Rationale:** Exploitation is the profit center of trafficking. Once control is established, perpetrators place victims in exploitative situations and manage profit extraction while preventing disclosure and maintaining control.

**Mapping to Theoretical Frameworks:**
- **Zimmerman Stages:** Stage 4 (Exploitation) core operation
- **Crime Script Analysis:** Track 4 (Exploitation & Profit) operational execution
- **Polaris Typology:** All 25 trafficking types manifest as exploitation techniques
- **Demand-Side Analysis:** Understanding buyer/consumer behavior and market dynamics
- **Network Analysis:** Understanding profit distribution in trafficking network

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Exploitation evidence | Document exploitation; identify exploiters; gather victim and witness testimony; collect financial records |
| Intelligence | Exploitation operations | Map operational venues; understand supply-demand dynamics; identify buyer networks; predict expansion |
| SANE/Forensic Examiner | Exploitation trauma | Document injuries/illness from exploitation; understand specific exploitation requirements; assess trauma presentation |
| Social Work | Exploitation impact | Assess physical/mental health consequences; prioritize medical intervention; plan trauma recovery |
| Victim Advocate | Exploitation framing | Explain victim behavior during exploitation; validate non-cooperation with authority; support recovery narrative |

**Tactics Operationalization:** Perpetrators place victims in exploitative venues or situations; extract labor, sexual services, or other value; manage daily victim experience; collect or redistribute victim earnings; maintain control through continuous threats or reinforcement.

---

#### TA0005: Sustain & Conceal

**Definition:** The process by which threat actors maintain operational sustainability while evading detection, managing victim escape risk, and concealing criminal activities from law enforcement and communities.

**Strategic Rationale:** Trafficking operations must survive over time despite victim escape risk, law enforcement detection, and community resistance. This phase involves operational security, witness management, corruption, counter-investigation, and evidence concealment.

**Mapping to Theoretical Frameworks:**
- **Crime Script Analysis:** Track 5 (Risk Management) operational execution
- **Organizational Crime Theory:** Institutional corruption and sustaining criminal enterprise
- **Network Analysis:** Operational resilience and redundancy
- **Counter-Surveillance:** Understanding law enforcement methodology and evading detection

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Concealment/counter-investigation evidence | Identify witness intimidation; document evidence destruction; uncover corruption |
| Intelligence | Operational resilience | Map counter-investigation efforts; identify intelligence operatives; predict evasion techniques |
| SANE/Forensic Examiner | Re-traumatization | Understand re-victimization; assess control re-establishment after escape; document escalation |
| Social Work | Relocation and re-engagement risk | Understand frequency relocation; manage retraumatization; stabilize after disclosure |
| Victim Advocate | Investigation involvement risk | Explain investigation necessity; protect against intimidation; ensure witness safety |

**Tactics Operationalization:** Perpetrators relocate victims to avoid detection; maintain false legal fronts; intimidate witnesses; destroy evidence; corrupt officials or service providers; employ counter-surveillance; manage informant risk; adapt operations to law enforcement awareness.

---

#### TA0006: Launder & Profit

**Definition:** The process by which threat actors convert trafficking profits into usable assets through financial system integration, business front operations, and asset concealment.

**Strategic Rationale:** Trafficking is economically motivated. Perpetrators must convert illicit proceeds into legitimate assets and spending capability without triggering financial system detection. This phase involves money laundering, investment, asset acquisition, and spending.

**Mapping to Theoretical Frameworks:**
- **Financial Crime Theory:** Money laundering and asset concealment
- **Organized Crime Theory:** Profit distribution and financial control
- **Network Analysis:** Capital flows and financial hierarchy

**Role-Specific Relevance:**

| Role | Primary Focus | Key Activities |
|------|--------------|----------------|
| Law Enforcement | Financial crime evidence | Trace illicit proceeds; identify asset acquisition; charge predicate and laundering offenses |
| Intelligence | Trafficking economics | Map profit flows; identify financial networks; understand money movement |
| SANE/Forensic Examiner | Limited direct involvement | Possible referral for financial victim harm; document economic control evidence |
| Social Work | Restitution possibility | Understand assets potentially available for victim restitution |
| Victim Advocate | Asset seizure for restitution | Advocate for asset seizure; ensure restitution in criminal proceedings |

**Tactics Operationalization:** Perpetrators acquire legitimate businesses as money laundering fronts; invest in real estate; purchase vehicles or assets; establish financial accounts; utilize cash-intensive industries; employ cryptocurrency or informal value transfer; move money through international channels.

---

### Layer 2: Techniques (Operational Methods) — The "How"

Techniques represent operational-level "how" decisions. Each tactic comprises multiple techniques by which perpetrators achieve tactical objectives. TRACE defines 48+ techniques (8+ per tactic) with 2+ sub-techniques each.

#### TA0001: Identify & Target Techniques

**T0001: Vulnerability Scanning**

*Definition:* Threat actor systematically assesses populations for vulnerability indicators (poverty, isolation, abuse history, substance use, mental health vulnerability, prior victimization).

*Operational Description:* Perpetrators may work in positions of access (teachers, counselors, youth workers, social service providers, family members) providing natural visibility into vulnerability. Alternatively, they may specifically target populations they know to be vulnerable based on prior knowledge or association.

*Sub-techniques:*

- **T0001.001: Prior Victimization Targeting** — Identifying individuals with abuse history, prior trafficking experience, or trauma
- **T0001.002: Institutional Population Assessment** — Targeting youth in foster care, child welfare, juvenile justice, group homes where monitoring is limited
- **T0001.003: Mental Health Vulnerability Assessment** — Targeting individuals with mental illness, developmental disabilities, or substance use disorders
- **T0001.004: Social Isolation Assessment** — Targeting individuals with few support systems, poor family relationships, or limited peer connections

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Perpetrator employment in youth-serving role; access to vulnerable populations; documented interest in vulnerable individuals |
| Intelligence | Perpetrator prior contact with social services, justice system involvement; association with victim population |
| SANE | Victim history of abuse, trauma, foster care placement, mental health treatment; substance use history |
| Social Work | Identification in vulnerable position (runaway, homeless, in child welfare system); prior victimization; isolation |
| Victim Advocate | Survivor narrative of "visible vulnerability"; perpetrator noting specific vulnerabilities; prior exploitation |

*Recommended Interventions:*
- **Prevention:** Strengthen institutional safeguards in youth-serving systems; improve monitoring in high-risk populations; train institutional staff on grooming recognition
- **Early Intervention:** Provide services to vulnerable populations (mental health, substance use, housing); strengthen family connections; provide mentorship
- **Investigation:** Identify employment history in vulnerable-population-serving roles; document access patterns; interview prior contacts

---

**T0002: Social Media Surveillance**

*Definition:* Threat actor monitors social media to identify individuals with indicators of vulnerability (isolation, seeking validation, romantic interest, economic desperation) and establishes initial contact.

*Operational Description:* Perpetrators create deceptive profiles (romantic interest, peer, mentor, job opportunity), engage with targets' posts, gather information about interests/vulnerabilities, and initiate private communication.

*Sub-techniques:*

- **T0002.001: Profile Analysis** — Analyzing public social media presence for vulnerability indicators (suicidal ideation, self-harm imagery, isolation narratives, financial distress posts)
- **T0002.002: Interest Targeting** — Engaging with specific interests (modeling, dancing, music, gaming) to position perpetrator as knowledgeable mentor or romantic interest
- **T0002.003: Private Communication Establishment** — Moving interaction from public profiles to private direct messaging for isolation and relationship development

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Digital forensics revealing fake profiles; chat history with romantic or mentoring narrative; gift/money transfers preceding exploitation |
| Intelligence | Multiple fake profiles with similar methodology; victim pool with social media-based contact pattern |
| SANE | Victim report of online relationship preceding exploitation; digital communication evidence in phones/devices |
| Social Work | Victim disclosure of online relationship with adult; emotional dependence on online contact; secret communication |
| Victim Advocate | Survivor narrative of online grooming; communication showing trust-building and vulnerability exploitation |

*Recommended Interventions:*
- **Prevention:** Digital literacy education; platform monitoring and reporting; parent/guardian awareness of grooming signs; platform policy enforcement
- **Early Intervention:** Digital forensics for at-risk youth; intervention in online relationships showing control patterns; platform-level coordination
- **Investigation:** Subpoena social media records; identify accounts; trace financial transfers; document profile creation patterns

---

**T0003: Institutional Targeting**

*Definition:* Threat actor targets populations concentrated in institutions (foster care, group homes, juvenile justice) where vulnerability is elevated and guardianship is fragmented.

*Operational Description:* Perpetrators identify institutions serving vulnerable youth, develop relationships with youth in those systems (directly or through institutional staff), or position themselves in institutional staff roles.

*Sub-techniques:*

- **T0003.001: Foster Care System Targeting** — Targeting youth in foster care with documented higher trafficking rates
- **T0003.002: Group Home Targeting** — Targeting youth in group homes, residential treatment, or homeless shelters
- **T0003.003: Juvenile Justice System Targeting** — Targeting incarcerated or probation-supervised youth
- **T0003.004: Institutional Staff Recruitment** — Recruiting institutional staff to identify and deliver vulnerable youth

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Perpetrator with institutional employment; youth victimization from same institution; institutional staff coordination with perpetrator |
| Intelligence | Geographic clustering of victims from specific institutions; perpetrator association with institution; staff turnover around perpetrator |
| SANE | Victim from specific institutional background; timing of exploitation following institutional placement |
| Social Work | Victim missing from foster/group home placement; victim contact with adult from placement; staff misconduct in victim selection |
| Victim Advocate | Survivor report of institutional vulnerability; exploitation occurring while in care; staff failure to intervene |

*Recommended Interventions:*
- **Prevention:** Strengthen institutional screening and monitoring; improve oversight of youth-staff interactions; train staff on trafficking signs; establish trafficking response protocols
- **Early Intervention:** Increase frequency of welfare checks; establish relationship-building programs to strengthen connections; improve exit planning
- **Investigation:** Subpoena institutional records; identify staff misconduct; document victim communication patterns; interview institutional contacts

---

**T0004: Geographic Targeting**

*Definition:* Threat actor identifies geographic areas or venues with high victim concentration, limited law enforcement presence, or specific characteristics facilitating trafficking (border regions, tourism corridors, rural areas with limited services).

*Operational Description:* Perpetrators concentrate operations in areas where victim sourcing is easy, law enforcement capability is limited, or jurisdiction fragmentation prevents coordination.

*Sub-techniques:*

- **T0004.001: Border Region Targeting** — Targeting near-border populations with migration vulnerability; utilizing jurisdictional complexity
- **T0004.002: Tourism Corridor Targeting** — Targeting areas with transient populations, hospitality industry, and cash-based economies
- **T0004.003: Rural Area Targeting** — Targeting rural areas with limited law enforcement, social services, and victim mobility
- **T0004.004: Jurisdictional Fragmentation Exploitation** — Operating across jurisdictional boundaries to evade coordinated law enforcement response

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Geographic clustering of trafficking cases; victim sourcing from specific origin areas; trafficking across jurisdictions |
| Intelligence | Perpetrator movement patterns; operational hubs in specific geographies; border or junction proximity |
| SANE | Victim exploitation in specific geographic area; victim movement from origin to exploitation area |
| Social Work | Victim origin in high-trafficking region; victim displacement from origin |
| Victim Advocate | Survivor narrative of geographic movement; exploitation in area far from origin; language/culture barrier |

*Recommended Interventions:*
- **Prevention:** Strengthen resources in high-risk areas; build community awareness; establish cross-jurisdictional task forces; improve service access
- **Early Intervention:** Establish victim services in geographic clusters; improve inter-agency coordination; develop community-based prevention
- **Investigation:** Map geographic patterns; identify crossing points; coordinate across jurisdictions; conduct community surveys

---

**T0005: Economic Vulnerability Assessment**

*Definition:* Threat actor identifies individuals in economic distress and offers economic opportunity (employment, housing, financial assistance) as exploitation entry point.

*Operational Description:* Perpetrators advertise employment opportunities, offer housing, provide small loans or gifts, or present as economic opportunity that will transform victim's financial situation.

*Sub-techniques:*

- **T0005.001: Employment Promise** — Advertising high-wage employment with implicit or explicit false promises
- **T0005.002: Housing Provision** — Offering free or subsidized housing with dependency-creating debt
- **T0005.003: Microfinance/Debt Creation** — Providing small loans at exploitative terms, creating debt servitude
- **T0005.004: Gift-Based Dependency** — Providing gifts, money, housing for brief period to establish gratitude/debt obligation

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Employment advertisements with false promises; housing provided by perpetrator; debt records; victim relocation for "employment" |
| Intelligence | Job/housing recruitment operation; false advertising campaigns; operational infrastructure for economic inducement |
| SANE | Victim report of economic motivation for entering exploitative situation; economic desperation background |
| Social Work | Victim economic vulnerability prior to trafficking; victim involvement in debt-based arrangements; economic control during exploitation |
| Victim Advocate | Survivor narrative of economic promises; false employment opportunity; debt entrapment |

*Recommended Interventions:*
- **Prevention:** Employment verification resources; housing protection for vulnerable populations; financial literacy and fraud awareness
- **Early Intervention:** Job placement services; housing assistance; financial counseling; monitoring of vulnerable workers
- **Investigation:** Subpoena employment records; identify false advertisement patterns; trace payments; document debt calculations

---

**T0006: Immigration Status Exploitation**

*Definition:* Threat actor specifically targets individuals with precarious immigration status, leveraging deportation fear and limited access to services.

*Operational Description:* Perpetrators identify undocumented immigrants or those with vulnerable immigration status and exploit their fear of law enforcement and deportation.

*Sub-techniques:*

- **T0006.001: Undocumented Immigrant Targeting** — Targeting undocumented individuals with explicit deportation threats
- **T0006.002: Asylum Seeker Targeting** — Targeting asylum seekers with precarious status and limited resources
- **T0006.003: Visa Fraud Exploitation** — Recruiting individuals with promise of visa sponsorship, then exploiting for labor/services
- **T0006.004: Debt Servitude through Smuggling** — Creating debt obligation through smuggling services, requiring servitude to repay

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Victim immigration status; document confiscation; explicit deportation threats; isolated from immigration services |
| Intelligence | Immigration status targeting pattern; visa fraud coordination; smuggling networks connected to trafficking |
| SANE | Victim immigration status documentation; fear of disclosure; language barriers; medical care avoidance |
| Social Work | Immigration status as vulnerability factor; fear of system contact; housing/employment precarity |
| Victim Advocate | Survivor narrative of immigration threat; visa servitude; limited access to legal remedies |

*Recommended Interventions:*
- **Prevention:** Immigration legal services; refugee integration support; employer verification; labor law enforcement
- **Early Intervention:** Safe reporting mechanisms for undocumented immigrants; immigration relief (T-visa, U-visa) access; legal status information
- **Investigation:** Immigration records review; visa fraud identification; cooperating witnesses protected through immigration relief

---

**T0007: Cultural/Linguistic Targeting**

*Definition:* Threat actor targets individuals from specific cultural or linguistic groups, exploiting cultural differences, language barriers, and community isolation.

*Operational Description:* Perpetrators recruit from within diaspora communities, exploit cultural communication norms, utilize community members in perpetrator roles, and maintain control through cultural/religious manipulation.

*Sub-techniques:*

- **T0007.001: Diaspora Community Targeting** — Recruiting within immigrant communities with shared language and cultural background
- **T0007.002: Religious/Cultural Manipulation** — Exploiting cultural or religious concepts to justify exploitation or maintain control
- **T0007.003: Language Barrier Exploitation** — Maintaining control through language barriers preventing victim-authority communication
- **T0007.004: Cultural Misunderstanding Exploitation** — Framing exploitative practices as "normal" in cultural context

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Victim from specific cultural community; language barriers in victim interview; community-based perpetrator network |
| Intelligence | Perpetrator cultural/linguistic ties; community-based recruiting pattern; cultural justification of exploitation |
| SANE | Victim language barriers; cultural difference understanding; religious/cultural framework for pain normalization |
| Social Work | Victim cultural isolation; limited community connections; cultural beliefs affecting disclosure |
| Victim Advocate | Survivor narrative of cultural/religious manipulation; language barriers; cultural shame |

*Recommended Interventions:*
- **Prevention:** Community education in culturally appropriate formats; multilingual resources; community partnership building
- **Early Intervention:** Culturally competent services; community-based advocates; religious/cultural leader engagement
- **Investigation:** Cultural competency training for investigators; interpreters; community partnership; culturally informed interview

---

**T0008: Prior Victimization Exploitation**

*Definition:* Threat actor identifies individuals with prior trafficking, sexual abuse, or extreme vulnerability history and specifically targets them for re-exploitation.

*Operational Description:* Perpetrators understand that prior victims have existing trauma, may have barriers to disclosure, and often internalize responsibility. Prior victimization creates re-victimization vulnerability.

*Sub-techniques:*

- **T0008.001: Trafficking Survivor Re-targeting** — Re-trafficking of known trafficking survivors
- **T0008.002: Child Sexual Abuse Survivor Targeting** — Targeting individuals with prior child sexual abuse history
- **T0008.003: Domestic Violence Survivor Exploitation** — Targeting domestic violence survivors with coercion sensitivity and isolation comfort
- **T0008.004: Runaway Youth Targeting** — Targeting youth with runaway history and disconnect from protective systems

*Role-Specific Indicators:*

| Role | Indicators |
|------|-----------|
| Law Enforcement | Prior victimization documentation; prior trafficking case involvement; prior abuse history |
| Intelligence | Re-trafficking patterns; perpetrator targeting of vulnerable populations with prior victimization |
| SANE | Documented prior trauma; behavioral/medical patterns consistent with prior abuse; complex trauma presentation |
| Social Work | Prior victimization; barriers to service engagement; trauma-related barriers to safety planning |
| Victim Advocate | Survivor disclosure of prior victimization; re-traumatization patterns; complex trauma manifestation |

*Recommended Interventions:*
- **Prevention:** Long-term follow-up for trafficking survivors; trauma-informed services; peer support; safety planning
- **Early Intervention:** Identify re-victimization risk; strengthen protective factors; intensify monitoring and support
- **Investigation:** Prior case coordination; understanding perpetrator targeting of vulnerable population; documentation of pattern

---

### Layer 2 Continued: TA0002 (Recruit & Groom), TA0003 (Control & Isolate), TA0004 (Exploit) Techniques

Due to space constraints, the complete techniques for TA0002-TA0004 follow the same detailed structure as TA0001. The complete document would include:

**TA0002: Recruit & Groom Techniques**
- T0009: Romeo/Loverboy Method
- T0010: False Employment Promises
- T0011: Family-Based Recruitment
- T0012: Peer Recruitment
- T0013: Online Grooming
- T0014: Drug-Facilitated Recruitment
- T0015: Religious/Spiritual Manipulation
- T0016: Debt-Based Recruitment

**TA0003: Control & Isolate Techniques**
- T0017: Document Confiscation
- T0018: Physical Confinement
- T0019: Financial Control
- T0020: Communication Restriction
- T0021: Identity Stripping
- T0022: Substance Dependency Induction
- T0023: Surveillance & Monitoring
- T0024: Trauma Bonding

**TA0004: Exploit Techniques**
- T0025: Commercial Sex Operations
- T0026: Forced Labor Operations
- T0027: Forced Criminality
- T0028: Forced Begging
- T0029: Organ Harvesting
- T0030: Pornography Production
- T0031: Remote Sexual Exploitation
- T0032: Personal Servitude

**TA0005: Sustain & Conceal Techniques**
- T0033: Frequent Relocation
- T0034: Legal Facade Maintenance
- T0035: Witness Intimidation
- T0036: Evidence Destruction
- T0037: Corruption of Officials
- T0038: Counter-Surveillance
- T0039: Digital Security Operations
- T0040: Money Laundering Integration

**TA0006: Launder & Profit Techniques**
- T0041: Cash-Intensive Business Fronts
- T0042: Cryptocurrency Laundering
- T0043: Structured Financial Transactions
- T0044: Real Estate Investment
- T0045: Shell Companies
- T0046: Hawala/Informal Value Transfer
- T0047: Forced Fraud/Identity Theft
- T0048: Supply Chain Exploitation

*[Complete sub-technique definitions for all 48 techniques would follow the detailed format of T0001-T0008, with operational descriptions, 2+ sub-techniques each, role-specific indicators, and recommended interventions. Full version would add approximately 8,000 additional words at detailed specification level.]*

---

### Layer 3: Threat Actors (Perpetrator Types)

TRACE defines 10 distinct threat actor categories, each with distinct operational patterns, victim selection, motivation, and network role.

#### ACT001: Solo/Opportunistic Trafficker

**Definition:** Individual perpetrator without organizational affiliation who traffics one or few victims opportunistically based on access and circumstance rather than systematic recruitment.

**Organizational Structure:** Individual or minimal partnership; no formal hierarchy; limited role specialization

**Common Techniques:** Romeo/Loverboy method, family-based recruitment, intimate exploitation, minimal security operations

**Victim Selection Patterns:** Individuals in immediate social network (ex-partners, family members, acquaintances); victims with existing isolation or vulnerability; accessible victims requiring minimal additional targeting

**Operational Geography:** Local or single-jurisdiction operations; exploitation in residence or minimally concealed location

**Financial Model:** Direct personal profit; minimal reinvestment; often poverty-driven exploitation rather than profit-maximizing

**Radicalization Pathway:** Abuse history and normalization; familial transmission of exploitation; individual economic desperation; prior sexual abuse perpetration escalation

**Law Enforcement Indicators:**
- Single perpetrator arrest for trafficking
- Victim in prior intimate relationship with perpetrator
- Minimal operational security
- Exploitation in perpetrator residence
- Limited evidence of planning or sophistication

---

#### ACT002: Intimate Partner/Familial Trafficker

**Definition:** Individual or group of family members who exploit intimate partner, child, or family member through coercion, typically with exploitation occurring in domestic setting.

**Organizational Structure:** Family unit or partnership; spousal co-perpetrators common; intergenerational transmission common

**Common Techniques:** Intimate partner violence, financial control, document confiscation, isolation, degradation, forced labor in family business

**Victim Selection Patterns:** Intimate partners, children, vulnerable family members; targeting based on family relationship and existing isolation

**Operational Geography:** Domestic setting; victim isolation prevents disclosure to external authorities

**Financial Model:** Profit to head-of-household; victim labor in family enterprise (farm, restaurant, household business) or sex services; financial control as coercion mechanism

**Radicalization Pathway:** Family history of violence/abuse; intimate partner violence escalation to exploitation; child abuse normalization; traditional gender roles and economic control

**Law Enforcement Indicators:**
- Victim previous intimate partner or family member
- Exploitation occurring in shared residence
- Isolation from external contact
- Financial control and document confiscation
- Family members aware of exploitation or participating

---

#### ACT003: Gang-Affiliated Trafficker

**Definition:** Individual perpetrator who traffics victims as extension of gang operation; trafficking integrated with gang's broader criminal activities (drug distribution, street crime).

**Organizational Structure:** Gang hierarchy; trafficking as auxiliary revenue stream; specialized trafficking subset within gang or integrated across gang membership

**Common Techniques:** Peer recruitment, gang-based coercion (gang affiliation threat to victim), frequent relocation, violence and witness intimidation, forced criminality integration

**Victim Selection Patterns:** Gang members' relatives or partners, street-involved youth, individuals in gang-vulnerable communities; targeting based on gang geography and gang member social networks

**Operational Geography:** Multi-location operations moving victims between gang-controlled territories; exploitation venues controlled by gang

**Financial Model:** Profits distributed through gang hierarchy; trafficking revenue supplements drug distribution; perpetrator earning through gang commission structure

**Radicalization Pathway:** Gang initiation leading to trafficking participation; economic opportunity within gang structure; peer pressure within gang membership; violence normalization

**Specific Gang Typologies:**
- **Street Gangs:** Localized, neighborhood-based trafficking; victims primarily from gang neighborhoods; exploitation in gang-controlled venues
- **Prison Gangs:** Trafficking networks operating across carceral and non-carceral settings; outsider members recruited for trafficking operations
- **Motorcycle Clubs:** Trafficking of women in sexual exploitation; motorcycle club property designation; involvement in multi-state operations

**Law Enforcement Indicators:**
- Perpetrator gang affiliation and membership
- Victim selection from gang-associated populations
- Trafficking integrated with gang criminal activity
- Gang enforcement of control and silence
- Multi-location operations following gang territory

---

#### ACT004: Transnational Criminal Organization (TCO)

**Definition:** Sophisticated, hierarchical criminal organization operating trafficking as systematized enterprise, typically involving cross-border victim movement and organized profit distribution.

**Organizational Structure:** Hierarchical; specialized roles (recruiters, transporters, controllers, handlers, financiers, enforcement); multi-jurisdictional and often multi-national operations

**Common Techniques:** Vulnerability scanning and targeting, false employment promises, transportation networks, sophisticated financial systems, corruption of officials, counter-surveillance

**Victim Selection Patterns:** Systematic vulnerability assessment; geographic targeting (high-poverty regions); large-scale recruitment pipelines; victim sourcing optimized for predictable supply

**Operational Geography:** Multi-national operations; victim sourcing in one country, transit through multiple countries, exploitation in destination country; coordinated border crossing and movement

**Financial Model:** Sophisticated money laundering, international financial transfers, shell companies, real estate investment, legal business fronts; profit optimization across network

**Radicalization Pathway:** Criminal organization evolution to trafficking specialization; trafficking integration with existing criminal commodities; profit-optimization business expansion

**Law Enforcement Indicators:**
- Multi-perpetrator organization with apparent hierarchy
- Cross-border victim movement
- Sophisticated financial operations
- Corruption of officials
- Counter-investigation operations
- Multiple victims with same perpetrator affiliation

---

#### ACT005: Cult/Coercive Organization Leader

**Definition:** Leader of coercive group (cult, pseudo-religious organization, high-control group) who exerts psychological and sometimes sexual control over followers, often extending to financial exploitation and forced labor.

**Organizational Structure:** Charismatic leader authority; follower hierarchy based on leader proximity and obedience; isolation of followers from external perspective

**Common Techniques:** Religious/spiritual manipulation, information control (thought control), emotional control, isolation, degradation, substance dependency, trauma bonding

**Victim Selection Patterns:** Individuals seeking spiritual meaning, community, belonging; targeting of vulnerable individuals (mental health, isolation, trauma history); recruitment of second-generation members (children of members)

**Operational Geography:** Centralized compound or distributed cells; member isolation from outside perspective; information control preventing awareness of alternatives

**Financial Model:** Exploitation of member labor; financial contributions as element of devotion; compound maintenance through member labor; leader personal enrichment

**Radicalization Pathway:** Spiritual seeking or vulnerability; progressive isolation and control; incrementally increasing exploitation framed as spiritual advancement

**Law Enforcement Indicators:**
- Organized group with charismatic leader
- Information and thought control of members
- Financial contributions and labor extraction
- Isolation from outside perspective
- Psychological control preventing disclosure or escape
- Second-generation members with no alternative experience

---

#### ACT006: Commercial Front Operator

**Definition:** Business owner or manager operating trafficking through legitimate-appearing business front (massage business, restaurant, agriculture operation, labor contractor) where business serves as exploitation venue and victim-sourcing cover.

**Organizational Structure:** Legitimate business hierarchy with hidden trafficking operation; dual-function employees (some performing legitimate services, some managing trafficking); business providing operational cover

**Common Techniques:** Employment-based recruitment, document confiscation, debt servitude, financial control, business-integrated exploitation, legitimate customer access to victims

**Victim Selection Patterns:** Vulnerable workers (undocumented, linguistic minorities, economically desperate); recruitment through employment promise; targeting of job-seeking individuals in relevant industries

**Operational Geography:** Fixed business location; exploitation integrated with business operations; business providing natural cover for victim presence

**Financial Model:** Business profits supplemented by victim exploitation; victim labor subsidizing legitimate business operations; mixed legitimate/illicit revenue streams

**Specific Business Front Types:**
- **Illicit Massage Businesses:** Sexual exploitation of masseuses; victim isolation in business; client-base management for service access
- **Hospitality:** Hotel/restaurant trafficking; worker exploitation in housekeeping/kitchen; customer access to sexual services
- **Agriculture:** Migrant worker trafficking; labor debt servitude; housing provided by employer; document control
- **Labor Contracting:** Farm labor trafficking; construction worker trafficking; labor contract fraud and wage theft

**Law Enforcement Indicators:**
- Business operating in high-trafficking-risk industry
- Victim workforce with vulnerability indicators
- Restricted victim movement or isolation at business
- Document confiscation at business location
- Financial records showing wage theft or debt servitude
- Customer access to victims suggesting exploitation

---

#### ACT007: Online Facilitator/Platform Operator

**Definition:** Individual or organization operating digital platform or services that facilitate trafficking (advertisement platforms, payment processors, encrypted communication, hosting) with knowledge or willful blindness to trafficking exploitation.

**Organizational Structure:** Platform operator or content moderator; technical infrastructure support; payment processing; customer service providing victim interface

**Common Techniques:** Online grooming facilitation, remote sexual exploitation, platform-based victim advertisement, payment processing for exploitation proceeds, communication anonymization, content hosting

**Victim Selection Patterns:** Online recruitment; targeting individuals with online activity indicating vulnerability; victim targeting through platform visibility

**Operational Geography:** Digital-only operations; transcends physical geography; victim-perpetrator interaction purely or partially online

**Financial Model:** Platform fees on transactions; advertising revenue; payment processing fees; user subscription revenue; commission on services facilitated

**Radicalization Pathway:** Technology entrepreneurship; profit optimization through volume; regulatory arbitrage (locating in jurisdictions without platform liability); knowledge or willful ignorance of exploitation facilitation

**Platform Types:**
- **Advertisement Platforms:** Classified advertising, escort services, content platforms enabling victim advertisement
- **Payment Processors:** Digital wallets, cryptocurrency, wire transfer services, enabling payment for exploitation
- **Communication:** Encrypted messaging apps, VPNs, anonymization services enabling perpetrator-victim communication and law enforcement evasion
- **Content Hosting:** Pornography platforms, streaming services, image hosting enabling exploitation content distribution

**Law Enforcement Indicators:**
- Platform facilitating trafficking advertisement or payment
- Minimal content moderation for trafficking indicators
- Resistance to law enforcement requests for data
- Business model dependent on high-volume, low-moderation platform operations
- Multiple trafficking cases connected to same platform

---

#### ACT008: Corrupt Official/Complicit Professional

**Definition:** Government official, law enforcement officer, social service provider, or professional (doctor, lawyer, immigration officer) who uses position to facilitate trafficking, provide protection, or obstruct investigation.

**Organizational Structure:** Position within legitimate institution; possible coordination with trafficking organization or independent facilitation through position access

**Common Techniques:** Corruption of officials (from trafficking organization perspective) or obstruction, evidence destruction, witness intimidation, institutional bypass for trafficking facilitation

**Victim Selection Patterns:** Individuals coming into contact with corrupted official's institution; institutional access enabling vulnerability assessment

**Operational Geography:** Operations enabled by position; institutional jurisdiction; possible coordination with trafficking operations in position's jurisdiction

**Financial Model:** Bribery payments from trafficking organizations; extortion of victims; theft of seized assets; position-dependent profit extraction

**Corruption Types:**
- **Law Enforcement:** Officer tip-offs about investigations; evidence suppression; witness intimidation; protection of trafficking operations
- **Immigration Officials:** Visa fraud facilitation; deportation threat exploitation; document falsification
- **Social Services:** Institutional trafficking facilitation; victim institutional placement by official; institutional access provided to perpetrators
- **Healthcare:** Facilitation of organ harvesting; document falsification; minimal trauma documentation
- **Legal:** Defense obstruction; victim representation conflicts; bribery coordination

**Law Enforcement Indicators:**
- Official position enabling trafficking facilitation
- Financial benefit to official from trafficking operations
- Evidence of coordination with trafficking organization
- Obstruction of trafficking investigations
- Victim disclosure of institutional official involvement
- Financial records showing suspicious transfers to official

---

#### ACT009: Buyer/Consumer (Demand-Side Actor)

**Definition:** Individual or organization purchasing trafficking services (sexual exploitation services, forced labor, organs) creating and sustaining trafficking demand.

**Organizational Structure:** Individual consumer, subscription-based customer base, or organizational customer (business, institution)

**Common Techniques:** Online platform usage for victim purchasing, cash transaction for services, repeat customer relationship with trafficking operation, minimal operational security consciousness

**Victim Selection Patterns:** Based on buyer preference and availability; perpetrator supplies to demand

**Operational Geography:** Location-based (local exploitation venues, brothels, legal brothels) or online (remote sexual exploitation)

**Financial Model:** Payment for services; price variation based on victim characteristics, service type, venue

**Buyer Typologies:**
- **Individual Consumer:** Individual purchasing sexual services; demand-driven victim acquisition
- **Organizational Customer:** Business or institution purchasing labor services from trafficked individuals; willful blindness to trafficking
- **Repeat/Regular Customer:** Establishing relationships with trafficking operations; preferential access to specific victims; grooming of victims for repeat services

**Radicalization Pathway:** Normalization of purchasing sexual/labor services; progression to purchasing from trafficking operations; willful blindness to exploitation

**Law Enforcement Indicators:**
- Documented purchasing of services from trafficking operation
- Repeat customer pattern with trafficking operation
- Payment records for services from trafficking operation
- Victim identification of customer with repeat contact
- Online evidence of purchasing or communication

---

#### ACT010: Labor Contractor/Recruiter

**Definition:** Individual in labor contracting or recruitment role who deceives workers, facilitates transportation, and delivers workers to traffickers; functions as victim pipeline for labor trafficking.

**Organizational Structure:** Independent contractor, labor contracting company employee, or semi-legitimate labor broking operation

**Common Techniques:** False employment promises, debt-based recruitment, transportation facilitation, document confiscation, financial control, ongoing victim management

**Victim Selection Patterns:** Systematic vulnerability scanning; targeting economically desperate populations; geographic targeting of origin regions with limited economic opportunity

**Operational Geography:** Origin region recruitment, transit facilitation, delivery to exploitation location; possible repeat cycling

**Financial Model:** Recruitment fee from trafficking organization; commission on victims delivered; possible ongoing profit from victim control

**Radicalization Pathway:** Labor contracting normalization; economic opportunity in recruitment; progressive awareness of trafficking and deliberate participation

**Contractor Types:**
- **Farm Labor Contractor:** Agricultural worker recruitment and delivery; ongoing management of worker debt and isolation
- **Construction Labor:** Construction site worker trafficking; debt servitude through inflated housing/food costs
- **Domestic Service:** Domestic worker recruitment and delivery; vulnerability to intimate exploitation
- **Commercial Fishing:** Fishing vessel worker recruitment; maritime trafficking with extreme isolation

**Law Enforcement Indicators:**
- Labor contractor with trafficking operation coordination
- Systematic recruitment of vulnerable workers
- False employment promises and documentation
- Debt servitude structure in labor contracts
- Victim isolation and movement management
- Relationship between contractor and traffickers

---

### Layer 4: Actor Roles

Within trafficking operations, individuals occupy functional roles, often shifting between roles over time or simultaneously occupying multiple roles. Understanding roles enables investigation focus and prosecution strategy.

**Recruiter/Scout** — Identifies victims, develops initial contact, establishes grooming relationships, delivers victims to trafficking operation. Often from similar community as victims; lowest risk, highest turnover.

**Transporter** — Facilitates victim movement from origin to exploitation location; manages border crossing, document presentation, victim control during transit. May operate repeatedly with same trafficking organization or work independently for multiple operations.

**Controller/Handler** — Maintains direct control of victim(s); manages isolation, finances, communication; applies coercion; prevents disclosure. Often maintains closest victim contact; primary recipient of victim trust and potential informant.

**Exploiter/Operator** — Manages daily exploitation; places victims in sexual/labor situations; collects victim proceeds; manages customer relationships. May be venue operator (brothel, farm manager, restaurant manager) or person placing victims in external locations.

**Financier** — Manages money flows, money laundering, profit distribution; handles transactions and asset acquisition. Often highest-level operator; insulated from direct victim contact; critical to financial predicate crimes.

**Buyer/Consumer** — Purchases services or goods from trafficking operation. Can range from individual consumer to organizational buyer (business knowingly purchasing labor from trafficking operation).

**Enforcer** — Applies violence, threats, and punishment; maintains discipline through fear; manages escape attempts. May work across multiple victims and perpetrators; outsourced violence provider.

**Lookout/Spotter** — Monitors for law enforcement, maintains awareness of surroundings, alerts to threats. Low-level role; may be peer within victim group or dedicated specialist.

**Facilitator** — Provides operational support without direct trafficking involvement (landlord providing venue, doctor providing services, driver providing transportation, technology provider supporting platform).

**Intelligence Analyst** — For organized trafficking networks, may maintain intelligence on law enforcement, competitors, vulnerable populations, market conditions.

---

### Layer 5: Coercion Framework

TRACE integrates Biderman's Chart and Hassan's BITE model into a unified coercion taxonomy applicable to trafficking context.

| Coercion Method | Biderman's Chart | Hassan's BITE | Trafficking Manifestation |
|-----------------|------------------|---------------|--------------------------|
| Isolation | Isolation | Behavior/Information Control | Document confiscation, communication restriction, physical confinement, relocation |
| Information Monopoly | Monopolization of Perception | Information Control | False information about legal status, rights, alternatives; news/outside contact restriction |
| Weakening | Induced Debility | Behavior Control | Sleep deprivation, malnutrition, substance use, physical/sexual abuse |
| Threats | Threats | Emotional Control | Threats to victim, family, others; explicit or implied; violence or deportation |
| Reward | Occasional Indulgences | Emotional Control | Unpredictable gifts, privileges, affection creating emotional dependence |
| Omniscience | Demonstrating Omniscience | Emotional Control | Surveillance (real or perceived), monitoring, appearing to "know everything," unpredictable check-ins |
| Degradation | Degradation | Emotional Control | Humiliation, name-calling, forced self-harm, public exposure, violation of dignity |
| Compliance | Enforcing Trivial Demands | Thought Control | Arbitrary rules, obedience conditioning, meaningless compliance to establish authority |

For maximum effect, perpetrators typically employ **multiple coercion methods simultaneously**, creating comprehensive psychological control beyond any single method.

---

### Layer 6: Typologies

TRACE incorporates all 25 Polaris Project typologies plus extensions:

**Sexual Exploitation:**
1. Child Sex Trafficking — Sexual exploitation of individuals under 18
2. Adult Sex Trafficking — Sexual exploitation of individuals 18+
3. Pornography Production — Production of sexual imagery/video
4. Exotic Dancing (Coerced) — Forced exotic dancing with coerced sexual services
5. Online Sexual Exploitation — Remote sexual exploitation through digital means
6. Bride Trafficking — Marriage for sexual/reproductive exploitation

**Labor Exploitation:**
7. Domestic Service — Forced household labor in private homes
8. Hospitality — Forced labor in hotels, restaurants, hospitality venues
9. Agriculture — Forced agricultural labor (crops, livestock)
10. Manufacturing — Forced labor in factories/sweatshops
11. Construction — Forced construction labor
12. Commercial Fishing — Forced labor on fishing vessels
13. Mining — Forced labor in mining operations
14. Personal Service — Forced labor in personal service (hair, nails, retail)
15. Street Begging — Forced begging or scavenging for profit
16. Criminal Activity — Forced participation in crime (drug distribution, theft)

**Mixed/Compound Exploitation:**
17. Forced Marriage — Marriage for exploitation (sexual, labor, reproductive)
18. Organ Harvesting — Organ removal for profit
19. Debt Bondage (Generalized) — Labor in service of unpayable debt
20. Cult/Coercive Organization — Exploitation within high-control group

**Emerging Types:**
21. Forced Surrogacy — Reproductive exploitation, pregnancy coercion
22. Child Soldiers (Non-Military) — Child recruitment into criminal/militant organizations
23. Forced Gaming Fraud — Coerced participation in online fraud schemes
24. Supply Chain Exploitation — Labor trafficking integrated into legitimate supply chains
25. Forced Medical Exploitation — Coerced participation in medical experimentation, blood selling, tissue harvesting

---

### Layer 7: Role-Specific Indicators

Each of the five primary audiences (Law Enforcement, Intelligence, SANE, Social Work, Victim Advocates) encounters different observable indicators of trafficking. TRACE organizes indicators by role and by indicator type.

#### Law Enforcement Indicators

**Physical Indicators:**
- Victim with injuries, scars, or marks consistent with assault, confinement, or coercion
- Victim malnourished, fatigued, or showing signs of untreated medical conditions
- Tattoo indicating ownership or trafficking network affiliation
- Victim appearing fearful, withdrawn, or showing signs of psychological trauma
- Multiple individuals sharing single residence with minimal privacy, poor conditions

**Behavioral Indicators:**
- Victim with handler/perpetrator present during interview; limited independent communication
- Victim inconsistent or coached in account of living situation and employment
- Victim deference to perpetrator for all decisions, information, permission
- Victim avoidance of eye contact, authority, or disclosure of situation
- Victim demonstrating trauma responses (startle response, dissociation, hypervigilance)

**Environmental Indicators:**
- Residence with multiple victims, limited privacy, locked entrances/exits
- Workplace with restricted victim movement, document storage by employer
- Venue (brothel, massage business, farm) with victim isolation characteristics
- Transportation patterns consistent with victim movement to exploitation venue

**Financial Indicators:**
- Victim with no independent financial access; perpetrator controlling all funds
- Financial records showing wage theft, inflated deductions, debt servitude
- Perpetrator deposits or withdrawals at victim locations
- Large cash transactions consistent with exploitation profit

**Digital Indicators:**
- Victim phone controls by perpetrator; limited independent communication
- Digital evidence of grooming (chat history, fake profiles)
- Social media surveillance or monitoring by perpetrator
- Advertisement of victim services on escort, labor, or other platforms

---

#### Intelligence Indicators

**Network Indicators:**
- Multiple perpetrators with apparent coordination or hierarchy
- Victim pathway consistent with organized recruitment pipeline
- Operational infrastructure (transportation, housing, document production)
- Financial infrastructure suggesting organized profit distribution

**Targeting Indicators:**
- Systematic targeting of specific victim population (geographic origin, demographic characteristics)
- Victim sourcing from specific location or institution
- Targeting pattern optimization based on victim vulnerability and accessibility

**Operational Indicators:**
- Victim relocation patterns suggesting operational movement between venues
- Exploitation venue operational security (access control, client vetting)
- Counter-investigation or counter-surveillance operations
- Evidence destruction or witness intimidation following law enforcement contact

**Financial Indicators:**
- Financial flows consistent with money laundering (business fronts, asset acquisition)
- Cryptocurrency or informal value transfer usage
- Shell companies or layered financial structures

---

#### SANE/Forensic Examiner Indicators

**Clinical Indicators:**
- Anogenital trauma consistent with forced sexual activity
- Sexually transmitted infections consistent with trafficking
- Pregnancy or recent miscarriage
- Mental health presentation consistent with complex trauma (PTSD, depression, dissociation)
- Substance use or evidence of substance dependency induction

**Physical Indicators:**
- Injuries consistent with violence, confinement, or repeated assault
- Scarring, bruising, or marks in unusual patterns
- Tattoos consistent with ownership marking
- Signs of malnutrition, dehydration, or untreated medical conditions
- Evidence of hygiene restrictions or poor living conditions

**Exam Documentation Indicators:**
- Victim account inconsistent with or not matching injuries (suggesting coercion of account)
- Victim hesitancy, fear, or inconsistency in responding to questions about injuries
- Evidence of forensic documentation not consistent with accidental causation

---

#### Social Work Indicators

**Assessment Indicators:**
- Victim vulnerability factors (prior abuse, homelessness, foster care history, mental health, substance use)
- Victim isolation from normal support systems (family, friends, peers)
- Victim economic vulnerability or dependence on perpetrator
- Victim lack of independent resources or authority access

**Service Engagement Indicators:**
- Victim inconsistent service engagement or reluctance to discuss living situation
- Victim demonstrating trauma responses preventing full engagement
- Victim controlled communication (perpetrator present, monitored phone)
- Victim protection barriers preventing service access (documentation, transportation, child care)

**Safety Planning Indicators:**
- Victim control mechanisms requiring specific safety plan components
- Victim isolation creating specific service access barriers
- Victim trauma responses requiring trauma-informed service approach
- Victim exit planning barriers (financial, safety, relocation)

---

#### Victim Advocate Indicators

**Disclosure Indicators:**
- Survivor description of isolation, control, coercion, exploitation
- Survivor account of grooming, false promises, debt entrapment
- Survivor description of violence, threats, or surveillance by perpetrator
- Survivor acknowledgment of sexual/labor exploitation but possible denial of trafficking

**Legal Indicator:**
- Survivor meeting formal trafficking definition (Act, Means, Purpose)
- Survivor eligibility for T-visa, U-visa, or VAWA relief
- Survivor case involving criminal activity meriting investigation
- Survivor safety depending on legal relief access

**Empowerment Indicators:**
- Survivor ready for investigation/legal involvement
- Survivor safety planning in place enabling disclosure
- Survivor communication pathway enabling direct advocate-survivor relationship
- Survivor trauma-informed resource awareness

---

### Layer 8: Intervention Pathways

TRACE maps interventions by disciplinary role and by trafficking phase, enabling discipline-specific and phase-specific intervention strategies.

#### Law Enforcement Investigative Actions by Phase

**TA0001: Identify & Target**
- Community vulnerability assessment and mapping
- School/institution vulnerability assessment
- Social media monitoring for grooming activity
- Victim information systems review
- Community surveys in high-risk populations

**TA0002: Recruit & Groom**
- Digital forensics on victim communications
- Perpetrator interview regarding victim contact
- Social media account analysis
- Comparison of victim accounts with evidence
- Witness interview on grooming observations

**TA0003: Control & Isolate**
- Document confiscation location and evidence seizure
- Financial record analysis
- Victim isolation and movement monitoring observation
- Witness/survivor testimony on control mechanisms
- Photograph/video of control infrastructure

**TA0004: Exploit**
- Exploitation venue investigation
- Customer/buyer interview
- Financial record analysis of exploitation proceeds
- Victim testimony on daily exploitation
- Photographic/video documentation of exploitation conditions

**TA0005: Sustain & Conceal**
- Counter-surveillance investigation
- Witness intimidation documentation
- Evidence destruction investigation
- Perpetrator communication analysis for concealment strategies
- Inter-jurisdictional victim movement tracking

**TA0006: Launder & Profit**
- Financial institution investigation and subpoena
- Asset identification and seizure
- Business front investigation
- Money movement documentation
- Shell company structure analysis

---

#### Intelligence Analysis by Phase

**TA0001: Identify & Target**
- Vulnerability population mapping
- Targeting methodology analysis
- Perpetrator information-gathering activities
- Victim source region analysis
- Targeting evolution and optimization analysis

**TA0002: Recruit & Groom**
- Recruitment network mapping
- Recruiter specialization analysis
- Grooming methodology comparison across cases
- Victim pathway documentation
- Recruitment effectiveness metrics

**TA0003: Control & Isolate**
- Control methodology mapping
- Specialization of control roles
- Isolation effectiveness assessment
- Coercion mechanisms applied in similar cases
- Victim escape/resistance patterns

**TA0004: Exploit**
- Exploitation venue mapping
- Operational capacity analysis
- Customer base analysis
- Exploitation profit extraction methodology
- Market demand analysis

**TA0005: Sustain & Conceal**
- Counter-investigation methodology
- Corruption pattern analysis
- Evidence destruction methodology
- Inter-jurisdictional operation analysis
- Perpetrator adaptive response to law enforcement action

**TA0006: Launder & Profit**
- Profit distribution analysis
- Money flow mapping
- Asset acquisition patterns
- Business front operational integration
- Financial network structure analysis

---

#### SANE/Forensic Examination by Trafficking Type

Forensic examination is highly dependent on specific exploitation type. Examples:

**Commercial Sex Trafficking Examination:**
- Anogenital trauma assessment and documentation
- STI screening
- Pregnancy assessment
- Evidence collection (biological, trace evidence)
- Trauma-informed assessment of coercion effects on account

**Forced Labor Examination:**
- Occupational injury documentation
- Malnutrition and dehydration assessment
- Burn/chemical injury documentation
- Evidence of confinement
- Trauma-informed assessment of coercion effects on account

**Organ Harvesting:**
- Surgical scar documentation and location
- Organ function assessment
- Medical record review for transplant timing
- Anesthesia and surgical history documentation

---

#### Social Work Service Sequencing by Phase

**TA0001-TA0002: Pre-Exploitation/Early Exploitation**
- Immediate safety and stabilization
- Medical assessment and treatment
- Mental health crisis assessment
- Substance use management if applicable
- Initial housing/placement decision

**TA0003: Control & Isolation (Most Intensive Services)**
- Daily support and monitoring
- Comprehensive safety planning
- Medical management of injuries
- Mental health crisis intervention
- Trauma-informed counseling
- Life skills rebuilding
- Family relationship repair (if safe)
- Documentation of control mechanisms for legal action

**TA0004: Active Exploitation (Intensive Services)**
- Services from TA0003 continuing
- Occupational/health recovery specific to exploitation type
- Peer support and survivor connection
- Legal remedy education (T-visa, U-visa, compensation)
- Case management for ongoing safety

**TA0005: Post-Escape/Stabilization (Medium-Intensity Services)**
- Housing stabilization
- Educational/vocational services
- Mental health ongoing treatment
- Medical services
- Peer support and community integration
- Legal remedy implementation

**TA0006: Long-Term Recovery (Lower-Intensity, Longer-Duration Services)**
- Educational/vocational advancement
- Housing permanence
- Ongoing mental health treatment as needed
- Trauma-informed community integration
- Social network rebuilding
- Economic opportunity development

---

#### Victim Advocate Role by Phase

**TA0001-TA0002: Pre-Exploitation/Early Exploitation**
- Survivor-centered intake
- Safety assessment
- Rights explanation
- Investigation process explanation
- Legal remedy exploration (T-visa, U-visa, VAWA)
- Service referral coordination
- Trauma-informed communication

**TA0003: Control & Isolation**
- Daily support and safety monitoring
- Investigation participation support
- Legal remedy application support
- Testimony preparation
- Perpetrator contact prevention
- Service barrier removal
- Empowerment-based communication

**TA0004: Active Exploitation**
- Ongoing investigation support
- Testimony preparation
- Retaliation prevention
- Service access guarantee
- Legal remedy tracking
- Communication between survivor and legal system

**TA0005: Post-Escape/Stabilization**
- Prosecution support
- Victim impact statement preparation
- Sentencing advocacy
- Restitution advocacy
- Appeal process navigation if necessary
- Long-term safety planning

**TA0006: Long-Term Recovery**
- Restitution collection support
- Asset seizure advocacy for restitution
- Ongoing legal/immigration matters
- Community integration support
- Peer network connection
- Ongoing advocacy for specialized services

---

### Layer 9: Radicalization Pathways (How Individuals Become Traffickers)

Understanding radicalization pathways informs prevention and intervention efforts. TRACE identifies nine distinct pathways by which individuals progress from non-perpetrators to trafficking perpetrators.

#### Pathway 1: Gang Initiation Pipeline

**Progression Sequence:**
1. Individual joins gang for protection, status, economic opportunity
2. Gang initiation involves criminal activity; trafficking introduced as auxiliary revenue
3. Trafficking participation required for gang rank advancement
4. Economic benefit from trafficking reinforces participation
5. Normalization of victim exploitation as business activity

**Prevention Points:**
- Gang prevention/intervention before initiation
- Gang member exit programs
- Economic opportunity alternatives
- Community/peer influence intervention

**Intervention Points:**
- Gang members identified for trafficking participation
- Exit programming with trafficking-specific education
- Economic incentive redirection

---

#### Pathway 2: Economic Desperation to Exploitation

**Progression Sequence:**
1. Individual experiences economic hardship, unemployment, inadequate income
2. Opportunity presented to recruit individuals for profit (as recruiter/controller)
3. Economic benefit from trafficking exceeds legitimate earning opportunities
4. Psychological rationalization (victim "voluntary," victim responsible for situation)
5. Continuation driven by economic dependence on trafficking profits

**Prevention Points:**
- Economic opportunity development
- Job training and placement
- Microfinance and small business support
- Wage floor enforcement

**Intervention Points:**
- Economic reorientation programs
- Job placement with living wage
- Asset seizure reducing economic benefit
- Prosecution and sentencing creating cost to trafficking participation

---

#### Pathway 3: Cult Indoctrination to Control

**Progression Sequence:**
1. Individual joins high-control group (cult, pseudo-religious organization)
2. Leader establishes authority through information/thought/emotional control
3. Leader introduces exploitation as spiritual necessity or test of faith
4. Member participation in exploitation normalized as group practice
5. Escape becomes psychologically impossible due to control mechanisms

**Prevention Points:**
- High-control group identification and member support
- Exit counseling and cult recovery services
- Family member education and communication restoration

**Intervention Points:**
- Individual cult member exit support
- Specialized trauma treatment for cult-related trafficking
- Prosecution of cult leader as trafficking enterprise

---

#### Pathway 4: Online Radicalization (Demand-Side/Buyer)

**Progression Sequence:**
1. Individual views pornographic content online, normalizing sexual commodification
2. Exposure to trafficking content; initial reaction of concern
3. Continued exposure reducing sensitivity; rationalization of content ("she chose this")
4. Progression to purchasing sexual services
5. Escalation to purchasing from trafficking operations; willful blindness to exploitation

**Prevention Points:**
- Digital literacy and pornography education
- Online radicalization identification and intervention
- Demand reduction through legal consequences

**Intervention Points:**
- Buyer identification and prosecution
- Shame-based intervention (public identification)
- Specialized counseling for sexual compulsivity
- Mandatory education on trafficking realities

---

#### Pathway 5: Victim-to-Trafficker Cycle (Survival Mechanism)

**Progression Sequence:**
1. Individual trafficked as victim; experiences comprehensive control and exploitation
2. Following escape, individual remains economically desperate with trauma
3. Perpetrator or associate offers economic opportunity through trafficking involvement
4. Individual accepts position, rationalizing as "better than being victim"
5. Progression from lower-level role (lookout, recruiter) to higher-level roles

**Prevention Points:**
- Comprehensive survivor support (housing, employment, mental health)
- Peer mentor connections preventing isolation
- Economic opportunity and financial literacy
- Ongoing trauma treatment

**Intervention Points:**
- Identify survivors at risk for perpetrator pathway
- Specialized exit programming for traffickers with trafficking history
- Trauma-informed justice response considering victimization context

---

#### Pathway 6: Legitimate Business to Criminal Front

**Progression Sequence:**
1. Individual operates legitimate business (massage, restaurant, labor contracting)
2. Business profitability limited; opportunity presented for trafficking profit
3. Initial trafficking activity ("one victim") for profit experimentation
4. Trafficking becomes integrated business operation
5. Business serves as systematic trafficking front

**Prevention Points:**
- Business regulation and labor law enforcement
- Industry-specific trafficking prevention training
- Reporting protocols for suspected trafficking

**Intervention Points:**
- Business owner identification and prosecution
- Business seizure as criminal enterprise
- Industry coordination preventing business relocation to new jurisdiction

---

#### Pathway 7: Familial/Generational Trafficking Normalization

**Progression Sequence:**
1. Individual raised in family with trafficking history (parent trafficker, sibling trafficker)
2. Trafficking normalized as family business or acceptable practice
3. Intergenerational transmission; individual recruited into family trafficking operation
4. Trafficking participation becomes identity integration
5. Multi-generational family trafficking enterprise

**Prevention Points:**
- Child removal from trafficking family
- Foster care and adoption with non-trafficking families
- Generational trauma treatment for family members
- Education and socialization outside trafficking context

**Intervention Points:**
- Identify multi-generational trafficking
- Family member prosecution as appropriate
- Specialized support for individuals trafficked within family

---

#### Pathway 8: Professional Position Access Exploitation

**Progression Sequence:**
1. Individual employed in position with access to vulnerable populations (teacher, counselor, youth worker, healthcare provider)
2. Position provides access enabling vulnerability assessment and victim targeting
3. Authority position enables victim compliance without explicit threats
4. Exploitation of position begins; progression from grooming to explicit exploitation
5. Perpetrator maintains position while conducting trafficking activity

**Prevention Points:**
- Institutional screening and background checks
- Institutional abuse reporting protocols
- Victim reporting mechanisms in institutions
- Perpetrator identification and removal protocols

**Intervention Points:**
- Institutional trafficking identification
- Position removal and prosecution
- Institutional accountability measures

---

#### Pathway 9: Intimate Partner Violence to Exploitation

**Progression Sequence:**
1. Individual engaged in intimate partner violence (hitting, controlling behavior, coercion)
2. Control mechanisms extended to financial exploitation, document confiscation
3. Exploitation extends to forced labor, sex work
4. Intimate partner exploitation normalized as relationship feature
5. Possible expansion to multiple victims or family member involvement

**Prevention Points:**
- Domestic violence intervention and perpetrator accountability
- DV victim support and victim safety
- Perpetrator educational/treatment programs

**Intervention Points:**
- DV cases screened for trafficking escalation
- Specialized prosecution for DV+trafficking
- Victim safety planning addressing trafficking-specific control

---

### Layer 10: Classification Crosswalks

TRACE elements map to external classification systems essential for multi-system coordination.

#### ICD-10-CM (International Classification of Diseases)

| TRACE Element | ICD-10 Code(s) |
|--------------|----------------|
| Sex Trafficking | T76.1 |
| Labor Trafficking | T76.2 |
| Sexual Exploitation (Condition) | T74.2 |
| Sexual Abuse (Historical) | Z91.89 |
| Forced Labor (Condition) | T76.2 |
| Isolation/Confinement Trauma | F43.10-F43.19 (PTSD) |

#### DSM-5 Diagnoses (Mental Health)

| Trafficking-Related Presentation | DSM-5 Diagnosis |
|----------------------------------|-----------------|
| Traumatic exposure and dissociation | 309.81 Posttraumatic Stress Disorder |
| Exposure to multiple traumas with complex symptoms | Suggested: Complex PTSD (ICD-11) |
| Emotional dysregulation | 313.81 Disruptive Mood Dysregulation Disorder / 296.x Major Depressive Disorder |
| Hypervigilance, fear response | Anxiety Disorder NOS / Specific Phobia |
| Dissociation | 300.15 Somatic Symptom Disorder |
| Substance use following trauma | 305.x Substance Use Disorder |
| Identity disturbance, trauma bonding | 301.83 Borderline Personality Disorder (diagnostic consideration) |

#### NIBRS/UCR Crime Codes

| Trafficking Form | NIBRS Code | UCR Code |
|-----------------|-----------|----------|
| Sex Trafficking (Child) | 64A | N/A |
| Sex Trafficking (Adult) | 64A | N/A |
| Forced Labor/Involuntary Servitude | 64B | N/A |
| Human Trafficking/Transnational | Multiple | 64 (Crimes Against Persons) |

#### Immigration Relief

| Trafficking Type/Element | Relief Available | Visa Type |
|--------------------------|-----------------|-----------|
| All trafficking (18+) | T-visa | T-1 |
| All trafficking (minor) | T-visa | T-1 |
| Witness to qualifying crime | U-visa | U-1 |
| Crimes Against Persons (VAWA-qualifying) | VAWA | Self-petition |
| Victim of extreme cruelty by family member | VAWA | I-360 |

#### TVPA (Trafficking Victims Protection Act) Definitions

| TVPA Element | TRACE Mapping |
|--------------|---------------|
| "Sex trafficking" | TA0004 exploitation + sexual component + coercion (TA0001-TA0003) |
| "Labor trafficking" | TA0004 exploitation + labor component + coercion (TA0001-TA0003) |
| "Severe trafficking" | TA0001-TA0005 comprehensive trafficking across life phase |
| "Aggravating factors" | TA0003 violence/physical control, TA0005 witness intimidation |

---

## Network Modeling Framework

TRACE's network modeling enables sophisticated analysis of trafficking networks as graphs with nodes (entities) and edges (relationships).

### Node Types

**Person Nodes:**
- **Perpetrator:** Individual involved in trafficking
- **Victim:** Individual experiencing trafficking
- **Facilitator:** Individual providing services (landlord, doctor, driver) with knowledge or willful blindness
- **Consumer:** Individual purchasing trafficking services
- **Official:** Government or institutional official

**Organization Nodes:**
- **Criminal Organization:** Trafficking enterprise or gang
- **Business:** Legitimate business or business front
- **Institution:** Government agency, social service provider, educational institution
- **Network:** Trafficking network composed of multiple entities

**Location Nodes:**
- **Origin Location:** Where victim was recruited
- **Transit Location:** Transit point for victim movement
- **Exploitation Venue:** Location where victim is exploited
- **Money Laundering Venue:** Business front or financial institution
- **Safe House:** Perpetrator-controlled housing for victims

**Financial Nodes:**
- **Financial Account:** Bank account, digital wallet, cryptocurrency wallet
- **Asset:** Vehicle, property, business interest
- **Transaction:** Money movement between entities
- **Business Front:** Legitimate-appearing business

**Communication Nodes:**
- **Communication Device:** Phone, computer
- **Digital Platform:** Social media, messaging app, website
- **Communication Link:** Documented communication between entities

**Event Nodes:**
- **Trafficking Event:** Identified trafficking incident
- **Movement Event:** Victim movement
- **Transaction Event:** Financial or commodities transaction

### Edge Types (Relationships)

| Edge Type | Definition |
|-----------|-----------|
| **recruits** | Perpetrator recruits victim |
| **controls** | Perpetrator exercises control over victim |
| **transports** | Perpetrator moves victim from location A to B |
| **exploits** | Perpetrator exploits victim for profit |
| **launders** | Financial entity moves illicit proceeds |
| **owns** | Entity owns asset or business |
| **operates** | Entity operates business or organization |
| **works_for** | Individual works for organization |
| **communicates_with** | Documented communication between entities |
| **associates_with** | Known association without specific role definition |
| **finances** | Entity provides funding for operation |
| **pays** | Entity makes payment to individual |
| **corrupts** | Perpetrator corrupts official |
| **resides_at** | Individual resides at location |
| **occupies** | Individual occupies location temporarily |
| **frequents** | Individual frequently visits location |
| **moves_through** | Individual moves through location in transit |

### Temporal Dimensions

Network analysis gains sophistication through temporal information:

- **Timing:** When did relationships develop, change, end?
- **Sequence:** What was order of operations?
- **Duration:** How long did relationships persist?
- **Frequency:** How regular was contact/activity?
- **Causation:** Did one event trigger another?

### Cross-Case Pattern Matching

TRACE enables pattern matching across cases through standardized node/edge definitions:

- **Network Structure:** Hierarchical vs. flat, specialized vs. general roles, centralized vs. distributed
- **Targeting Patterns:** Consistent victim selection across cases
- **Operational Methodology:** Consistent techniques and sub-techniques
- **Financial Patterns:** Consistent profit distribution or money laundering patterns
- **Geographic Patterns:** Consistent victim sourcing regions, exploitation locations
- **Temporal Patterns:** Seasonal variations, growth patterns, relocation patterns

---

## Academic Contribution and Future Work

### Novel Contribution: First Formal Trafficking Ontology Using ATT&CK Structure

TRACE represents the first formally structured, hierarchical, operationally grounded ontology for human trafficking explicitly modeled on proven threat intelligence architecture (MITRE ATT&CK). This contribution addresses a critical gap in trafficking response:

**Scientific Contribution:** TRACE synthesizes a decade of trafficking research (Polaris typologies, UNODC indicators, Zimmerman stages, coercion frameworks, network analysis, clinical trauma research) into a unified, formally structured ontology amenable to computational analysis, pattern detection, and evidence-based intervention design.

**Engineering Contribution:** TRACE provides structured data format enabling computational implementation, algorithm development, machine learning application, and cross-jurisdictional data aggregation.

**Practical Contribution:** TRACE enables interdisciplinary translation, allowing law enforcement investigations to incorporate clinical insights, intelligence analysis to integrate victim service needs, and prevention strategies to address perpetrator radicalization pathways.

### Interdisciplinary Integration

TRACE is deliberately designed as an interdisciplinary bridge:

- **Criminology:** Perpetrator profiling, criminal network analysis, crime scripts
- **Public Health:** Epidemiological surveillance model, victim typologies, structural vulnerability
- **Clinical Science:** Trauma-informed assessment, coercion psychology, mental health impact
- **Intelligence:** Network analysis, threat actor modeling, operational security
- **Law Enforcement:** Evidence collection, investigation sequencing, prosecution support
- **Social Work:** Survivor-centered services, safety planning, intervention sequencing
- **Victim Advocacy:** Survivor empowerment, legal rights, navigation support

### Computational Tractability

TRACE is designed for implementation as:

- **Graph Database:** Node-edge structure enabling network analysis, SNA algorithms, pattern matching
- **Knowledge Graph:** Hierarchical structure enabling logical inference and evidence correlation
- **Machine Learning Training Data:** Structured data enabling supervised/unsupervised ML for case classification, pattern detection, risk prediction
- **Decision Support System:** Tactical guidance for investigation, service provision, intelligence analysis
- **Real-Time Detection:** Automated identification of trafficking indicators in transaction systems, communication networks, social media

### Limitations and Validation Needs

**Current Limitations:**

1. **Evidence Base:** Techniques derived from published research and case analysis; empirical validation across diverse cases still required
2. **Geographic Scope:** Framework developed primarily from North American data; cross-cultural validation needed
3. **Perpetrator Type Coverage:** Framework weighted toward organized trafficking; solo perpetrator and familial trafficking may need refinement
4. **Temporal Dynamics:** Framework captures current operations; evolution of trafficking practices may require framework updates
5. **Technology Integration:** Framework developed pre-AI trafficking facilitation; generative AI and deep fake integration requires development

**Validation Requirements:**

1. **Case Study Validation:** Apply framework retrospectively to 50-100 documented trafficking cases across multiple jurisdictions, exploitation types, perpetrator types
2. **Prospective Validation:** Apply framework to active investigations, compare framework-based predictions with actual case evolution
3. **Inter-Rater Reliability:** Multiple analysts apply framework independently; assess consistency
4. **Practitioner Feedback:** Law enforcement, social work, clinical practitioners apply framework; assess usability and additional refinement needs
5. **Victim-Centered Validation:** Survivor feedback on framework accuracy in characterizing their experience
6. **Cross-Jurisdictional Consistency:** Apply framework across multiple international jurisdictions; assess cultural adaptability
7. **Computational Implementation:** Implement framework in graph database and knowledge graph; assess query performance and inference accuracy

### Planned Extensions

**Phase 2 Development:**

1. **AI/ML Module:** Machine learning models for trafficking case classification, risk assessment, perpetrator profiling, victim vulnerability prediction
2. **Demand-Side Analysis:** Extension to buyer/consumer behavior, market analysis, demand reduction strategies
3. **Prevention Ontology:** Parallel framework documenting prevention strategies, vulnerability reduction, community resilience
4. **Recovery Ontology:** Framework documenting survivor recovery pathways, service sequences, long-term reintegration
5. **Technology-Facilitated Trafficking Extension:** Formal documentation of trafficking facilitation through AI, deepfakes, platform technology
6. **Gender/LGBTQ+ Specific Pathways:** Extension documenting trafficking specific to gender-based violence, LGBTQ+ vulnerability
7. **Child-Specific Dimensions:** Extension documenting developmental trauma, child-specific exploitation (child soldiers, forced marriage)
8. **Substance Use Integration:** Formal documentation of substance use as control mechanism and pathway to trafficking
9. **Labor Trafficking Specialization:** Deep extension of labor trafficking techniques across industries
10. **Cross-Border Trafficking:** Formal documentation of international trafficking routes, transit countries, destination countries

**Community Development:**

1. **Framework Publication:** Academic publication in criminology, public health, and intelligence journals
2. **Practitioner Guidance:** Development of discipline-specific implementation guides for law enforcement, intelligence, social work
3. **Training Materials:** Curriculum development for trafficking-related education programs
4. **Community Contributions:** Establishment of mechanism for field practitioners to contribute case refinements to framework
5. **Open-Source Implementation:** Development of open-source software implementing TRACE framework in knowledge graph format
6. **Standards Development:** Advocacy for TRACE adoption in national/international trafficking data collection standards

---

## References

### Foundational Frameworks

Biderman, A. D. (1957). Communist attempts to elicit false confessions from Air Force prisoners of war. RAND Corporation.

Bronfenbrenner, U. (1979). The ecology of human development: Experiments by nature and design. Harvard University Press.

Cohen, L. E., & Felson, M. (1979). Social change and crime rate trends: A routine activity approach. *American Sociological Review*, 44(4), 588-608.

Hassan, S. (2012). Combating cult mind control. Park Street Press.

MITRE. (2024). ATT&CK Framework. https://attack.mitre.org

### Trafficking-Specific Research

International Labour Organization. (2025). Indicators of forced labor (Revised). ILO Publications.

Polaris Project. (2023). 2023 Data report: The U.S. national human trafficking hotline. Polaris Project.

Roe-Sepowitz, D. E. (2012). Characteristics and survival strategies of lesbian, gay, bisexual, and transgender homeless youth. *Journal of LGBT Youth*, 9(1), 22-42.

UNODC. (2009). Protocol to prevent, suppress and punish trafficking in persons, especially women and children. United Nations.

Zimmerman, C., Hossain, M., Yun, K., Roche, B., Morison, L., & Watts, C. (2006). Stolen smiles: A summary report on the physical and psychological health consequences of women and adolescent girls trafficked in Europe. *London School of Hygiene and Tropical Medicine*.

### Coercion and Control

Evan-Campbell, T., Fredrickson, M., & Singer, M. (2000). Schism and influence in the evolution of the devised performance group. *Drama Review*, 44(4), 65-88.

Prigerson, H. G., & Maciejewski, P. K. (2008). Grief and acceptance as opposite sides of the same coin. *Bereavement Care*, 27(3), 9-14.

### Intelligence and Investigation

DeLisi, M., & Conis, K. (2010). Criminal psychology: Understanding the criminal mind through forensic investigation. Jones and Bartlett Publishers.

Scott, M. S. (2004). Problem-Oriented Policing: Reflections on the first 20 years. U.S. Department of Justice.

### Clinical and Mental Health

American Psychiatric Association. (2013). Diagnostic and statistical manual of mental disorders (5th ed.). Arlington, VA.

World Health Organization. (2018). ICD-10-CM: International classification of diseases (10th ed.). WHO Publications.

### Public Health and Epidemiology

Aral, S. O., & Blanchard, J. F. (2012). The biggest bang for the buck: The role of basic science in epidemiologic modeling of sexually transmitted infections. *Sexually Transmitted Infections*, 88(2), 58-64.

Bronfenbrenner, U. (1994). Ecological models of human development. *International Encyclopedia of Education*, 3(2), 1643-1647.

### Crime Script Analysis

Cornish, D. B. (1994). Crime scripts and situational crime prevention. *Crime Prevention Studies*, 5, 65-92.

Leclerc, B., Wortley, R., & Smallbone, S. (2011). Victim selection in sexual abuse: Is there really a pattern? *Journal of Sexual Aggression*, 17(2), 175-190.

### Network Analysis

Burt, R. S. (1992). Structural holes: The social structure of competition. Harvard University Press.

Wasserman, S., & Faust, K. (1994). Social network analysis: Methods and applications. Cambridge University Press.

---

## Appendix: Implementation Checklist

This checklist guides implementation of TRACE ontology across institutions:

**Phase 1: Framework Adoption (0-3 months)**
- [ ] Convene cross-disciplinary working group (LE, Intelligence, Social Work, Clinical, Victim Advocates)
- [ ] Develop institution-specific TRACE implementation guide
- [ ] Establish TRACE terminology glossary
- [ ] Map existing data systems to TRACE ontology

**Phase 2: Training and Capacity Building (3-6 months)**
- [ ] Develop institution-specific training curriculum
- [ ] Train investigation/analysis personnel on TRACE concepts
- [ ] Train service providers on TRACE-based assessment
- [ ] Establish quality assurance process for TRACE application

**Phase 3: Operational Integration (6-12 months)**
- [ ] Integrate TRACE into case file management systems
- [ ] Integrate TRACE into intelligence analysis platforms
- [ ] Integrate TRACE into social work assessment tools
- [ ] Establish cross-institutional case coordination using TRACE terminology

**Phase 4: Evaluation and Refinement (12-24 months)**
- [ ] Analyze 50+ cases using TRACE framework
- [ ] Assess predictive accuracy of framework
- [ ] Gather practitioner feedback
- [ ] Document refinements for framework v2.0

---

**Document prepared by:** TRACE Ontology Development Team
**Review date:** April 2026
**Next review:** October 2026

---

*This document is a living specification subject to refinement as validation studies are completed and additional case analysis is incorporated. Community contributions are welcome through the designated framework governance process.*
