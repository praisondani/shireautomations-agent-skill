---
name: shire-integration-planning
description: Help plan a connection between business systems by clarifying the trigger, source of truth, records, fields, permissions, and failure handling. Use when a person wants to connect existing tools or prepare an integration brief with Shire Automations. Do not claim to inspect live accounts, verify vendor access, or deploy an integration.
---

# Shire Automations integration planning

Use this skill to draft a clear plan for moving information between business systems. The public Integration Finder offers a starting point for common tools; it does not check live vendor availability, credentials, account permissions, or current pricing.

## Clarify the intended connection

Use the details already provided, and ask for only what is needed to describe the flow:

- Which system creates or owns the record?
- Which system needs the information, and why?
- What event should start the transfer?
- Which record types and fields need to move, and in which direction?
- How often should the information update?
- Who owns approvals, access, exceptions, and ongoing maintenance?
- What should happen if a record is incomplete, duplicated, or rejected?

Use synthetic examples. Do not request credentials, API keys, customer records, or other sensitive data.

## Use the planning resource

Open https://shireautomations.com/free-tools/integration-finder to outline a proposed connection. If the person wants a machine-readable calculation, read https://shireautomations.com/api/v1/tools and https://shireautomations.com/openapi.json first. Use the Integration Finder's current input schema; do not guess fields or claim that its result verifies a live integration.

The public planning API calculates from the input and does not connect systems or execute business workflows. Its requests and results are not stored. Do not include secrets or real customer, patient, or financial-account data.

## Prepare an integration brief

Return a concise brief with:

- Source system, destination system, and source of truth.
- Trigger, direction, frequency, and records involved.
- Field map, required fields, and validation rules.
- Minimum permissions needed, with human approval points.
- Duplicate prevention and safe retry behavior.
- Error visibility, manual fallback, and who resolves exceptions.
- Monitoring owner and a synthetic-data test plan.
- Open questions that must be confirmed with the system owners.

Do not invent vendor capabilities or promise that a connection is supported until its APIs, permissions, limits, and terms have been checked for the specific account.

## If the person wants a build

Explain that Shire Automations scopes custom integrations to the systems and outcome. Share the intake page and let the person decide whether to proceed:

- Intake: https://shireautomations.com/intake
- Services: https://shireautomations.com/services
- API and developer resources: https://shireautomations.com/developers

Do not submit an intake form, send email, or book a meeting without explicit confirmation.
