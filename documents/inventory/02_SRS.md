# Software Requirements Specification — Inventory Management & Process Improvement

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Functional requirements
| ID | Capability | Actor | Requirement | Priority |
| --- | --- | --- | --- | --- |
| INV-FR-01 | Receipt capture | Receiving Clerk | The system shall record a goods receipt with SKU, quantity, supplier reference, timestamp and user ID. | Must |
| INV-FR-02 | Receipt validation | Receiving Clerk | The system shall reject unknown SKUs and zero or negative receipt quantities. | Must |
| INV-FR-03 | Stock issue | Sales Coordinator | The system shall post authorised stock issues and prevent negative available quantity. | Must |
| INV-FR-04 | Inventory ledger | Operations Manager | The system shall calculate on-hand balance from posted receipts, issues and approved adjustments. | Must |
| INV-FR-05 | Stock alert | Warehouse Supervisor | The system shall flag SKUs at or below reorder threshold after a successful transaction. | Should |
| INV-FR-06 | Adjustment approval | Warehouse Supervisor | The system shall require a reason and supervisor approval for manual quantity adjustments. | Must |
| INV-FR-07 | Audit log | System Administrator | The system shall retain user, time, SKU, previous balance, change and reference for each posting. | Must |
| INV-FR-08 | Inventory view | Sales Coordinator | The system shall provide searchable current balances and an exportable stock summary. | Should |

## Non-functional requirements
| ID | Category | Requirement |
| --- | --- | --- |
| INV-NFR-01 | Availability | The pilot solution should be accessible during warehouse operating hours, excluding planned maintenance. |
| INV-NFR-02 | Performance | A routine stock query should return within 3 seconds under an agreed pilot workload. |
| INV-NFR-03 | Security | Only authorised roles may post adjustments; all users require authenticated access. |
| INV-NFR-04 | Integrity | A receipt or issue must update both the ledger and current balance as one transaction. |
| INV-NFR-05 | Usability | Clerks should be able to record a standard receipt with a short guided form. |
| INV-NFR-06 | Traceability | Audit entries should remain readable and exportable by authorised managers. |

## Business rules
1. The same receipt reference cannot be posted twice for the same supplier and SKU without exception approval.
2. Available stock must not become negative as a result of a standard issue transaction.
3. Only a supervisor can approve a quantity adjustment; an approver cannot alter the posting audit history.
4. Low-stock status is evaluated after a successfully committed movement.

## Assumptions and exclusions
Supplier invoicing, accounting integration, multi-warehouse transfers, purchasing automation, mobile barcode device procurement and a working production application.

## Validation approach
Each functional requirement is mapped to one or more user stories and an acceptance test in the validation document. The specifications describe intended software behaviour; no operational implementation is claimed.
