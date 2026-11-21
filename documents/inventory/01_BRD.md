# Business Requirements Document (BRD) — Inventory Management & Process Improvement

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Executive summary
A complete business-analysis documentation exercise for replacing delayed paper-to-spreadsheet stock updates with a controlled, role-based inventory process.

## Business setting
Illustrative single-site wholesale distributor (fictional case organisation). This is a scenario developed for the portfolio, not a commissioned client engagement.

## Current-state problem
Goods were counted on arrival, written on paper and only entered into Excel at the end of a shift. Sales teams relied on potentially outdated availability figures, while missed entries and manual retyping created reconciliation risks.

## Objective
Make stock movement visible at the point of work, preserve an auditable history, and provide sales with a current availability view.

## In scope
A single-warehouse workflow for goods receipts, stock issues, controlled adjustments, minimum-stock alerts, role permissions, stock reports and audit trails.

## Out of scope
Supplier invoicing, accounting integration, multi-warehouse transfers, purchasing automation, mobile barcode device procurement and a working production application.

## Stakeholders and responsibilities
| Role | Responsibility |
| --- | --- |
| Warehouse Supervisor | Approves stock adjustments, reviews exceptions and reconciles counts |
| Receiving Clerk | Records delivered goods and verifies quantities |
| Sales Coordinator | Checks available stock before confirming orders |
| Operations Manager | Monitors stock accuracy and exception trends |
| System Administrator | Maintains roles, SKU master and audit access |

## Current-state workflow (AS-IS)
1. Supplier delivers goods
2. Manual count on paper
3. Paper retained until end of shift
4. Clerk retypes quantity into Excel
5. Sales team checks spreadsheet

## Proposed future-state workflow (TO-BE)
1. Receive goods and identify SKU
2. Validate quantity and scan/enter receipt
3. System updates ledger immediately
4. Sales sees current availability
5. Exceptions trigger review and audit

## Gap analysis
| Gap | AS-IS | TO-BE | Business reason |
| --- | --- | --- | --- |
| Delayed availability | End-of-shift spreadsheet entry | Event-driven stock posting | Prevent stale stock visibility |
| Data-entry errors | Paper-to-Excel retyping | SKU and quantity validation | Reduce rekeying exposure |
| Untracked adjustments | Edits without central history | Role-controlled stock adjustments with reason | Improve accountability |
| Reorder signals | Periodic manual check | Threshold alerts on ledger updates | Identify low stock earlier |

## Business rules
- The same receipt reference cannot be posted twice for the same supplier and SKU without exception approval.
- Available stock must not become negative as a result of a standard issue transaction.
- Only a supervisor can approve a quantity adjustment; an approver cannot alter the posting audit history.
- Low-stock status is evaluated after a successfully committed movement.

## KPIs (illustrative targets, not achieved results)
| KPI | Definition | Pilot objective |
| --- | --- | --- |
| Inventory accuracy rate | 1 - (absolute quantity discrepancies across counted SKUs / physical units counted); report as % | Illustrative pilot target: 98% or higher |
| Update latency | Median time between physical receipt confirmation and visible system balance | Pilot objective: within 1 minute |
| Unapproved adjustment count | Adjustments posted without authorisation | Control objective: zero |

## Risks and mitigations
| Risk | Mitigation |
| --- | --- |
| Incomplete SKU master | Pilot with data cleansing and signed-off SKU list |
| Unreliable connectivity | Document offline exception and reconciliation procedure |
| Staff adoption | Run receiving-clerk walkthroughs and staged training |
| Concurrent edits | Use transactional movement ledger and conflict checks |
