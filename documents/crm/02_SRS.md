# Software Requirements Specification — CRM & Customer Service Optimisation

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Functional requirements
| ID | Capability | Actor | Requirement | Priority |
| --- | --- | --- | --- | --- |
| CRM-FR-01 | Enquiry intake | Sales Agent | The system shall register customer contact, channel, enquiry category, owner and timestamp. | Must |
| CRM-FR-02 | Duplicate warning | Sales Agent | The system shall warn about potential duplicates using email or mobile number before saving. | Should |
| CRM-FR-03 | Ownership | Team Leader | The system shall assign a named owner and track reassignment reason and timestamp. | Must |
| CRM-FR-04 | Lead stage | Sales Agent | The system shall record defined statuses from New to Qualified, Proposal, Won, Lost or Closed. | Must |
| CRM-FR-05 | Follow-up queue | Sales Agent | The system shall store next-action date, action description and completion status. | Must |
| CRM-FR-06 | Escalation | Team Leader | The system shall highlight overdue follow-ups to the owner and team leader. | Should |
| CRM-FR-07 | Handover | Service Coordinator | The system shall capture service scope, committed date, contact details and handover acknowledgement before marking Won leads as handed over. | Must |
| CRM-FR-08 | Reporting | Business Manager | The system shall show stage counts, owner workload and overdue follow-ups with a date filter. | Should |

## Non-functional requirements
| ID | Category | Requirement |
| --- | --- | --- |
| CRM-NFR-01 | Access control | Only authenticated staff may view customer contact records; role permissions apply to reassignment and reports. |
| CRM-NFR-02 | Performance | A filtered lead list should load within 3 seconds at an agreed test workload. |
| CRM-NFR-03 | Data quality | Contact email/mobile format checks should be applied at enquiry capture. |
| CRM-NFR-04 | Auditability | Every status and owner change should retain actor and timestamp. |
| CRM-NFR-05 | Usability | A new enquiry should require a short form with clearly marked mandatory fields. |
| CRM-NFR-06 | Privacy | Personal information export must be role-controlled and limited to the agreed business purpose. |

## Business rules
1. A lead must have exactly one active owner.
2. Each open lead must have a next-action date or an explicit documented exception.
3. A lead cannot be moved to Won without a recorded service handover checklist.
4. Reopening a closed lead requires a reason; status history must remain available.

## Assumptions and exclusions
Full email/WhatsApp API integration, automated quotation pricing, billing, AI lead scoring, phone recording and a deployed production CRM.

## Validation approach
Each functional requirement is mapped to one or more user stories and an acceptance test in the validation document. The specifications describe intended software behaviour; no operational implementation is claimed.
