# Swedish Municipal AI Compliance Checklist (2026)

[![Maintained by Sigfrid Systems](https://img.shields.io/badge/maintained%20by-Sigfrid%20Systems-blue)](https://sigfrid.ai)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

A practical compliance checklist for Swedish municipalities deploying AI systems. Covers GDPR Article 30 documentation and EU AI Act Article 50 transparency requirements.

**Maintained by [Sigfrid Systems](https://sigfrid.ai)** — AI compliance infrastructure for Swedish public sector.

---

## Quick Start

Use this checklist for **each AI system** that processes personal data in your municipality.

---

## GDPR Article 30: Processing Register Checklist

### Part 1: Basic Documentation

- [ ] AI system is identified and named in the processing register
- [ ] Responsible contact person for the AI system is specified
- [ ] Deployment date is documented
- [ ] Last update of documentation is noted

### Part 2: Purpose and Legal Basis

- [ ] Purpose of AI processing is clearly described
- [ ] Legal basis for processing is specified (consent, contract, legal obligation, public interest)
- [ ] Connection to business need is documented
- [ ] Any automated decision-making under Article 22 is noted

### Part 3: Personal Data Categories

- [ ] Categories of personal data handled by the AI system are listed
- [ ] Sensitive personal data (special categories) are identified
- [ ] Personal ID numbers (personnummer) are documented if processed
- [ ] Source of personal data is specified

### Part 4: Data Subjects

- [ ] Categories of data subjects are defined (citizens, employees, etc.)
- [ ] Estimated volume of data subjects is documented
- [ ] Geographic scope is specified

### Part 5: Data Sharing and Recipients

- [ ] AI vendor is documented as recipient/processor
- [ ] Data Processing Agreement (DPA) exists with AI vendor
- [ ] Sub-processors are identified
- [ ] Purpose for each sharing is specified

### Part 6: Third Country Transfers

- [ ] Transfer to third country is identified and documented
- [ ] Legal basis for transfer is specified (SCCs, adequacy decision, etc.)
- [ ] Specific countries where data is transferred are listed
- [ ] Security measures for transfer are described

### Part 7: Retention Periods

- [ ] Retention period for AI interaction logs is defined
- [ ] Retention period for training data is defined (if applicable)
- [ ] Deletion procedure is documented
- [ ] Legal justification for retention period exists

### Part 8: Security Measures

- [ ] Technical security measures are described (encryption, access control)
- [ ] Organizational measures are documented (training, policies)
- [ ] PII handling before data reaches AI model is described
- [ ] Logging and audit trail is implemented

---

## EU AI Act Article 50: Transparency Checklist

**Deadline: August 2, 2026**

### For AI-Generated Content

- [ ] Citizens are informed when interacting with an AI system
- [ ] AI-generated content is marked as such
- [ ] Disclosure mechanism is implemented at point of generation
- [ ] Disclosure is clear, understandable, and accessible

### For Chatbots and Virtual Assistants

- [ ] Clear indication that the user is interacting with AI (not a human)
- [ ] Disclosure appears before or at the start of interaction
- [ ] Accessibility requirements are met (screen readers, etc.)

### Documentation Requirements

- [ ] Technical documentation describes AI system capabilities
- [ ] Transparency mechanisms are documented
- [ ] Update procedures for disclosures are defined

---

## Common Compliance Gaps

Based on our audits of Swedish municipalities:

| Gap | Frequency | Risk Level |
|-----|-----------|------------|
| Missing AI vendor in processing register | 67% | High |
| No DPA with AI vendor | 43% | Critical |
| Undefined retention periods for AI logs | 58% | Medium |
| No DPIA for high-volume AI processing | 31% | High |
| Missing Article 50 disclosure mechanism | 89% | High (after Aug 2026) |

---

## Example: Municipal Chatbot Documentation

```yaml
Processing Activity: Citizen Inquiry Chatbot
Purpose: Answer citizen questions about municipal services
Legal Basis: Public interest (kommunallagen)
Data Categories:
  - Name
  - Contact details
  - Case numbers
  - Query content (may contain various personal data)
Data Subjects: Citizens contacting the municipality
Recipients:
  - AI Vendor: [Name], DPA signed [Date]
  - Hosting: Azure Sweden North
Third Country Transfer: No
Retention: 24 months (chat logs), anonymized statistics indefinitely
Security:
  - Encryption in transit (TLS 1.3) and at rest (AES-256)
  - Role-based access control
  - PII detection before AI processing
  - Complete audit logging
DPIA: Required, completed [Date], archived [Reference]
Article 50: Disclosure banner implemented [Date]
```

---

## Resources

### From Sigfrid Systems

- [Complete Article 50 Guide](https://sigfrid.ai/en/resources/article-50)
- [GDPR Article 30 Deep Dive](https://sigfrid.ai/en/resources/gdpr-article-30-checklist)
- [Shadow AI Mapping Guide](https://sigfrid.ai/en/resources/shadow-ai-mapping)
- [Compliance Calculator](https://sigfrid.ai/en/roi-calculator)

### Official Sources

- [GDPR Article 30 (EUR-Lex)](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
- [EU AI Act (EUR-Lex)](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
- [IMY Guidance (Swedish DPA)](https://www.imy.se/)
- [DIGG AI Guidance](https://www.digg.se/)

---

## Contributing

Found an error or have a suggestion? Open an issue or submit a PR.

This checklist is maintained by [Sigfrid Systems](https://sigfrid.ai) and licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

---

## About Sigfrid Systems

Sigfrid Systems provides AI compliance infrastructure for Swedish public sector. We help municipalities deploy AI safely with GDPR and EU AI Act compliance built in.

- **Website:** [sigfrid.ai](https://sigfrid.ai)
- **Contact:** kontakt@sigfrid.ai
- **Member of:** [AI Sweden](https://www.ai.se)

For automated compliance solutions, [contact us](https://sigfrid.ai/en/contact).
