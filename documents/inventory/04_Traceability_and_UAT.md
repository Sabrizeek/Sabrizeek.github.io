# Traceability, UAT & KPIs — Inventory Management & Process Improvement

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## Requirements traceability matrix
| Requirement | User story | UAT test |
| --- | --- | --- |
| INV-FR-01 | INV-US-01 | INV-UAT-01 |
| INV-FR-02 | INV-US-02 | INV-UAT-02 |
| INV-FR-03 | Direct validation | INV-UAT-03 |
| INV-FR-04 | Direct validation | INV-UAT-04 |
| INV-FR-05 | INV-US-05 | INV-UAT-05 |
| INV-FR-06 | INV-US-04 | INV-UAT-06 |
| INV-FR-07 | INV-US-06 | INV-UAT-07 |
| INV-FR-08 | INV-US-03 | INV-UAT-08 |

## User acceptance testing scenarios
| Test ID | Scenario | Test input | Expected outcome | Requirement | Story |
| --- | --- | --- | --- | --- | --- |
| INV-UAT-01 | Receive valid goods | Known SKU, quantity 25 | Receipt saved; available stock +25 | INV-FR-01 | INV-US-01 |
| INV-UAT-02 | Block invalid receipt | Quantity -2 | Validation error; no posting | INV-FR-02 | INV-US-02 |
| INV-UAT-03 | Prevent overselling | Issue exceeds on-hand balance | Transaction blocked; no negative quantity | INV-FR-03 | INV-US-03 |
| INV-UAT-04 | Read updated balance | Post receipt, refresh stock view | Displayed balance matches ledger | INV-FR-04 | INV-US-03 |
| INV-UAT-05 | Low-stock threshold | Issue reduces stock to reorder level | SKU listed as low stock | INV-FR-05 | INV-US-05 |
| INV-UAT-06 | Supervisor adjustment | Submit with reason, approve | Posting saved with approval details | INV-FR-06 | INV-US-04 |
| INV-UAT-07 | Review audit history | Find completed posting | Actor, time and balance change visible | INV-FR-07 | INV-US-06 |
| INV-UAT-08 | Export summary | Search SKU and export report | Export reflects current on-hand figures | INV-FR-08 | INV-US-03 |

## KPI definitions
| Measure | Calculation | Target type |
| --- | --- | --- |
| Inventory accuracy rate | 1 - (absolute quantity discrepancies across counted SKUs / physical units counted); report as % | Illustrative pilot target: 98% or higher |
| Update latency | Median time between physical receipt confirmation and visible system balance | Pilot objective: within 1 minute |
| Unapproved adjustment count | Adjustments posted without authorisation | Control objective: zero |

## UAT status
**Test scenarios authored and reviewed as a case-study deliverable.** They have not been executed against a production system.
