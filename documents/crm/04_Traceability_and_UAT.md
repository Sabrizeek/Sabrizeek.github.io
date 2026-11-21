# Traceability, UAT & KPIs — CRM & Customer Service Optimisation

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Requirements traceability matrix
| Requirement | User story | UAT test |
| --- | --- | --- |
| CRM-FR-01 | CRM-US-01 | CRM-UAT-01 |
| CRM-FR-02 | CRM-US-02 | CRM-UAT-02 |
| CRM-FR-03 | CRM-US-03 | CRM-UAT-03 |
| CRM-FR-04 | Direct validation | CRM-UAT-04 |
| CRM-FR-05 | CRM-US-04 | CRM-UAT-05 |
| CRM-FR-06 | CRM-US-05 | CRM-UAT-06 |
| CRM-FR-07 | CRM-US-06 | CRM-UAT-07 |
| CRM-FR-08 | Direct validation | CRM-UAT-08 |

## User acceptance testing scenarios
| Test ID | Scenario | Test input | Expected outcome | Requirement | Story |
| --- | --- | --- | --- | --- | --- |
| CRM-UAT-01 | Create enquiry | Valid contact and source | Unique lead ID and capture time saved | CRM-FR-01 | CRM-US-01 |
| CRM-UAT-02 | Duplicate warning | Existing customer email | Duplicate warning appears before save | CRM-FR-02 | CRM-US-02 |
| CRM-UAT-03 | Set owner | Assign lead to active agent | Owner visible; history updated | CRM-FR-03 | CRM-US-03 |
| CRM-UAT-04 | Record stage | Move Qualified to Proposal | Stage updated with actor and time | CRM-FR-04 | CRM-US-03 |
| CRM-UAT-05 | Schedule follow-up | Save next action for tomorrow | Task appears for lead owner | CRM-FR-05 | CRM-US-04 |
| CRM-UAT-06 | Escalate overdue | Incomplete action with past due date | Overdue queue shows owner and age | CRM-FR-06 | CRM-US-05 |
| CRM-UAT-07 | Handover control | Won lead with missing checklist item | Handover blocked until required items provided | CRM-FR-07 | CRM-US-06 |
| CRM-UAT-08 | Manager report | Apply date range filter | Stage and overdue counts reflect selected period | CRM-FR-08 | CRM-US-05 |

## KPI definitions
| Measure | Calculation | Target type |
| --- | --- | --- |
| On-time follow-up rate | Completed follow-ups by due date / all due follow-ups × 100 | Illustrative pilot target: 90% or higher |
| First-response time | Median time from enquiry capture to first recorded response | Review baseline then agree target |
| Overdue open-lead count | Open leads with incomplete actions past their due date | Pilot objective: declining weekly trend |

## UAT status
**Test scenarios authored and reviewed as a case-study deliverable.** They have not been executed against a production system.
