# Agile User Stories & Acceptance Criteria — Inventory Management & Process Improvement

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## INV-US-01 — Receiving Clerk
**User story:** As a Receiving Clerk, I want to capture delivered goods with a supplier reference so that stock is reflected promptly and errors can be traced.

**Linked requirement:** INV-FR-01

**Acceptance criterion:** Given a known SKU and positive quantity, when I submit a valid receipt, then the ledger records the movement and displays the new balance.

## INV-US-02 — Receiving Clerk
**User story:** As a Receiving Clerk, I want to be warned when I enter an invalid SKU or quantity so that I can correct errors before posting.

**Linked requirement:** INV-FR-02

**Acceptance criterion:** Given an unknown SKU or non-positive quantity, when I submit the form, then the system blocks posting and displays a specific validation message.

## INV-US-03 — Sales Coordinator
**User story:** As a Sales Coordinator, I want to see the current available quantity so that I can confirm orders based on up-to-date data.

**Linked requirement:** INV-FR-08

**Acceptance criterion:** Given a posted stock movement, when I search for that SKU, then I see the updated on-hand quantity.

## INV-US-04 — Warehouse Supervisor
**User story:** As a Warehouse Supervisor, I want to approve a documented correction so that inventory discrepancies are accountable.

**Linked requirement:** INV-FR-06

**Acceptance criterion:** Given an adjustment with a reason, when an authorised supervisor approves it, then the stock ledger records the approved movement and approver.

## INV-US-05 — Operations Manager
**User story:** As a Operations Manager, I want to review low-stock items so that I can plan replenishment.

**Linked requirement:** INV-FR-05

**Acceptance criterion:** Given stock falls to or below reorder level, when the transaction commits, then the SKU appears in the low-stock list.

## INV-US-06 — System Administrator
**User story:** As a System Administrator, I want to inspect changes by user and SKU so that I can investigate discrepancies.

**Linked requirement:** INV-FR-07

**Acceptance criterion:** Given any completed stock posting, when an authorised user views its history, then actor, timestamp, reference and before/after quantities are visible.

