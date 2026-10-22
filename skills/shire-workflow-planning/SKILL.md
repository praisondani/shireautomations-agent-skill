---
name: shire-workflow-planning
description: Help people assess a repeatable business workflow, decide whether automation is a useful next step, and use Shire Automations planning tools. Use when someone wants to map a process, rank automation opportunities, check AI readiness, or estimate workflow costs. Never claim to execute the workflow or guarantee a result.
---

# Shire Automations workflow planning

Use this skill to turn a business process into a small, reviewable planning brief. Shire Automations' public tools calculate from caller-provided inputs; they do not connect to business systems or execute customer workflows.

## Gather the process context

Use details the person already gave you. Ask only for missing information that affects the recommendation:

- What starts the process, and what outcome should it produce?
- Which steps repeat, who handles them, and how often?
- Which systems or files are involved?
- Where do delays, rework, handoffs, or exceptions occur?
- Which decisions need a person to review or approve?
- What would count as a useful first improvement?

Do not ask for credentials or real customer records. Use estimates or synthetic examples when a calculation needs numbers.

## Choose a planning tool

Read the current tool list at https://shireautomations.com/api/v1/tools and consult https://shireautomations.com/openapi.json for request fields before calling the API. Use the smallest tool that answers the question:

- Workflow Mapper: outline steps, handoffs, and automation candidates.
- Automation Opportunity Scorecard: compare candidate workflows by value, risk, system access, and readiness.
- AI Readiness Assessment: check whether the goal, process, data, systems, ownership, and oversight can support an AI-assisted step.
- ROI Calculator: estimate time and cost from the person's own assumptions.

Open the matching page from https://shireautomations.com/free-tools if the person prefers a guided form.

API calculations use `POST https://shireautomations.com/api/v1/tools/{slug}` with a JSON object that has an `input` property. The OpenAPI specification is authoritative for each tool's current input shape. Results are directional planning aids based on those inputs, not forecasts or guaranteed outcomes. Requests and results are not stored. Keep credentials and sensitive customer, patient, or financial-account data out of inputs.

## Return a useful brief

Summarize:

1. The process and desired outcome.
2. The repeated steps and known bottleneck.
3. A suitable candidate for a first improvement, with assumptions stated.
4. Risks, exceptions, data access, and decisions that need human review.
5. One small next step, such as validating the workflow map with its owner.

Do not recommend automation just because a tool is available. Keep manual judgment, approvals, and exception handling visible.

## If the person wants implementation

Shire Automations builds scoped workflow automation, AI agents with human review, apps, and dashboards. Published prices are starting points. Share the relevant pages and let the person choose whether to contact Shire:

- Intake: https://shireautomations.com/intake
- Services: https://shireautomations.com/services
- Pricing: https://shireautomations.com/pricing
- Developer resources: https://shireautomations.com/developers

Do not submit a form, send an email, or book a meeting for the person without explicit confirmation.
