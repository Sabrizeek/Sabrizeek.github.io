# Business Requirements Document (BRD) — CRM & Customer Service Optimisation

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Executive summary
A complete customer-operations BA documentation exercise for centralising enquiries, clarifying ownership and preventing missed follow-ups.

## Business setting
Illustrative Sri Lankan B2B service provider (fictional case organisation). This is a scenario developed for the portfolio, not a commissioned client engagement.

## Current-state problem
Customer enquiries arrived through email, telephone and messaging, and agents tracked activity in personal notes or spreadsheets. Team leaders had limited visibility of who owned each lead, when the next follow-up was due and whether a service request had been handed over.

## Objective
Provide a shared source of truth for enquiries and follow-ups, with clear accountability and measurable customer-response workflows.

## In scope
Manual enquiry registration, duplicate detection, lead status and ownership, next-action dates, reminders, escalation, service handover checklist, audit trail and funnel reporting.

## Out of scope
Full email/WhatsApp API integration, automated quotation pricing, billing, AI lead scoring, phone recording and a deployed production CRM.

## Stakeholders and responsibilities
| Role | Responsibility |
| --- | --- |
| Sales Agent | Registers enquiries, qualifies leads and schedules follow-ups |
| Team Leader | Monitors ownership, approves escalations and reviews workload |
| Service Coordinator | Accepts approved handovers and tracks service readiness |
| Business Manager | Reviews response time, conversion stages and overdue tasks |
| System Administrator | Configures roles, statuses and retention settings |

## Current-state workflow (AS-IS)
1. Customer calls, emails or messages
2. Agent notes enquiry privately
3. Follow-up date kept in notebook
4. Team lead asks for manual status
5. Service handover via ad hoc message

## Proposed future-state workflow (TO-BE)
1. Log enquiry in shared queue
2. Check duplicate and assign owner
3. Set next action and due date
4. Monitor alerts and escalation queue
5. Complete structured service handover

## Gap analysis
| Gap | AS-IS | TO-BE | Business reason |
| --- | --- | --- | --- |
| Fragmented enquiry records | Personal notes and inboxes | Shared enquiry record with unique ID | Improve visibility |
| Missed follow-ups | Reminder depends on memory | Due-date reminder and overdue queue | Reduce overlooked tasks |
| Unclear accountability | No consistent owner | Required lead owner and state changes | Improve ownership |
| Handover gaps | Unstructured service messages | Minimum checklist and acknowledgement | Improve traceability |

## Business rules
- A lead must have exactly one active owner.
- Each open lead must have a next-action date or an explicit documented exception.
- A lead cannot be moved to Won without a recorded service handover checklist.
- Reopening a closed lead requires a reason; status history must remain available.

## KPIs (illustrative targets, not achieved results)
| KPI | Definition | Pilot objective |
| --- | --- | --- |
| On-time follow-up rate | Completed follow-ups by due date / all due follow-ups × 100 | Illustrative pilot target: 90% or higher |
| First-response time | Median time from enquiry capture to first recorded response | Review baseline then agree target |
| Overdue open-lead count | Open leads with incomplete actions past their due date | Pilot objective: declining weekly trend |

## Risks and mitigations
| Risk | Mitigation |
| --- | --- |
| Duplicate contact data | Define matching rules and manual merge permissions |
| Agent adoption | Pilot shared queue with team-led review |
| Sensitive contact information | Role access and retention review |
| Ambiguous lead stages | Agree a concise status dictionary before UAT |
