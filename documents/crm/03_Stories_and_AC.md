# Agile User Stories & Acceptance Criteria — CRM & Customer Service Optimisation

> **Document type:** Completed independent Business Analysis case study — simulated business scenario.
> **Prepared:** November 2026 · **Author:** Sabri Mazahim · **Version:** 1.0

## CRM-US-01 — Sales Agent
**User story:** As a Sales Agent, I want to register a new enquiry in one shared location so that my colleagues can see the latest information.

**Linked requirement:** CRM-FR-01

**Acceptance criterion:** Given required contact fields and an enquiry category, when I save a new lead, then it receives a unique ID, owner and capture timestamp.

## CRM-US-02 — Sales Agent
**User story:** As a Sales Agent, I want to receive possible duplicate warnings so that I can avoid fragmented customer history.

**Linked requirement:** CRM-FR-02

**Acceptance criterion:** Given a matching phone or email, when I enter contact details, then a potential-duplicate warning appears before save.

## CRM-US-03 — Team Leader
**User story:** As a Team Leader, I want to assign and reassign a named lead owner so that responsibility is unambiguous.

**Linked requirement:** CRM-FR-03

**Acceptance criterion:** Given an unassigned lead, when I choose a valid active owner, then the lead displays the owner and records the assignment.

## CRM-US-04 — Sales Agent
**User story:** As a Sales Agent, I want to record the next follow-up action and due date so that I can prioritise customer commitments.

**Linked requirement:** CRM-FR-05

**Acceptance criterion:** Given an active lead, when I save the next action and due date, then the task appears in my follow-up queue.

## CRM-US-05 — Team Leader
**User story:** As a Team Leader, I want to see an overdue follow-up list so that I can intervene before enquiries are neglected.

**Linked requirement:** CRM-FR-06

**Acceptance criterion:** Given a due date in the past and an incomplete action, when I open the overdue view, then the lead appears with its owner.

## CRM-US-06 — Service Coordinator
**User story:** As a Service Coordinator, I want to receive a complete sales-to-service handover so that service delivery can start with agreed context.

**Linked requirement:** CRM-FR-07

**Acceptance criterion:** Given a Won lead, when the handover checklist is completed and acknowledged, then its status changes to Handed over.

