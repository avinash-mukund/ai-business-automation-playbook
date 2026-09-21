# AI Business Automation Playbook

![n8n](https://img.shields.io/badge/n8n-Orchestration-orange)
![AI](https://img.shields.io/badge/AI-Claude%20%2F%20OpenAI-blue)
![CRM](https://img.shields.io/badge/CRM-HubSpot%20%7C%20GHL%20%7C%20Salesforce-green)
![Status](https://img.shields.io/badge/Status-Active-success)

> Practical AI automation systems that turn repetitive business work into reliable, measurable workflows.

**Target markets:** Australia / New Zealand • APAC • Middle East

---

## Table of Contents
- [Overview](#overview)
- [Systems Included](#systems-included)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Repository Structure](#repository-structure)
- [Design Principles](#design-principles)
- [Who This Is For](#who-this-is-for)
- [Status](#status)

---

## Overview

This playbook documents end-to-end AI automation systems for high-impact business operations:

- Lead capture, qualification and follow-up
- Customer support automation
- Voice reception and appointment booking
- Dead lead reactivation
- CRM process automation
- Email and administrative workflows

Each system is built around a real operational problem and follows a consistent pattern:  
**Trigger → AI Processing → Business Logic → System Action → Human-in-the-loop (when needed)**

---

## Systems Included

| # | System | Description |
|---|--------|-------------|
| 01 | [AI Customer Support Automation](./01-ai-customer-support-automation) | Classify, respond and escalate support enquiries |
| 02 | [AI Voice Receptionist & Booking](./02-ai-voice-receptionist-booking) | Answer calls, book appointments, update CRM |
| 03 | [Dead Lead Reactivation](./03-dead-lead-reactivation) | Re-engage inactive leads with personalised sequences |
| 04 | [AI Lead Qualification & Follow-Up](./04-ai-lead-qualification-followup) | Instant qualification, scoring and nurturing |
| 05 | [CRM Automation](./05-crm-automation) | Lifecycle, data quality and cross-system sync |
| 06 | [Email & Admin Workflows](./06-email-admin-workflows) | Parse, classify, route and process operational email |

---

## Architecture

Every system in this playbook follows the same reliable structure:

```mermaid
flowchart LR
    A[Trigger<br>Form / Call / Email / Webhook] --> B[AI Processing<br>Classify • Extract • Decide]
    B --> C[Business Logic<br>Score • Route • Rules]
    C --> D[System Actions<br>CRM • Calendar • Messaging]
    D --> E[Human Review<br>Only when needed]
    E --> F[Logging & Measurement]
