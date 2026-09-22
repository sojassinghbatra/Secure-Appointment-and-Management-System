# Secure Appointment Management System

A real-client system design project completed as part of a first-year Computer Science group project at Toronto Metropolitan University (2025–2026).

## 📋 Project Overview

A financial consultant client approached our group with a real-world business problem: their appointment scheduling, client follow-up, and workflow management processes were entirely manual, inefficient, and lacked proper data security.

Our team analyzed the client's workflow, identified the core pain points, and designed a comprehensive solution — a secure, three-tier CRM-style web application to automate appointment scheduling, follow-up reminders, and client data management.

> **Note:** This repository contains the full system design documentation across all project phases. The application is a proposed and designed solution, not a deployed codebase.

## 🎯 The Problem

The client faced three core challenges:

- **Scheduling inefficiencies** — Appointments were tracked manually with no automated reminders, increasing the risk of missed follow-ups.
- **No centralized client data management** — Client information was scattered across spreadsheets and email threads.
- **Security and compliance gaps** — Sensitive financial client information required stronger privacy and security controls.

## 💡 Proposed Solution

We designed a full-stack, three-tier web application with the following proposed technology stack:

| Component | Technology |
|---|---|
| Frontend | React.js |
| Backend | Node.js |
| Database | PostgreSQL |
| Authentication | Firebase Authentication |
| Email Notifications | SendGrid |
| SMS Reminders | Twilio |
| Privacy & Compliance | PIPEDA-focused design |

### Core Features Designed

- **Appointment Scheduling Module** — Calendar-based booking with conflict detection.
- **Automated Follow-up System** — SendGrid email and Twilio SMS reminders triggered by appointment status.
- **Role-Based Access Control** — Separate access levels for administrators, consultants, and clients.
- **Secure Client Portal** — Firebase Authentication with security-focused data handling.
- **Database Schema** — Normalized PostgreSQL schema with relationship mapping for clients, appointments, and follow-ups.
- **Privacy & Compliance Layer** — Designed around consent management, data retention policies, and audit logging.

## 🏗️ System Architecture

```text
┌─────────────────────────────────────────┐
│           React.js Frontend             │
│                                         │
│  Appointment UI • Client Portal         │
│  Admin Dashboard                        │
└──────────────────┬──────────────────────┘
                   │
                REST API
                   │
┌──────────────────▼──────────────────────┐
│            Node.js Backend              │
│                                         │
│  Business Logic • Authentication        │
│  Middleware • Notification Triggers     │
└──────────────┬───────────────┬──────────┘
               │               │
       ┌───────▼──────┐ ┌────▼──────────────┐
       │  PostgreSQL  │ │ Firebase Auth +   │
       │   Database   │ │ SendGrid / Twilio │
       └──────────────┘ └───────────────────
```

👤 My Contributions
Sojas Singh Batra

System architecture design
Database design and relationship mapping
Security specifications
Privacy and compliance requirements
Technical system design documentation

👥 Team
Sojas Singh Batra — System Architecture, Database Design, Security & Compliance Specifications
Group Members — Client Analysis, UI/UX Workflow Design, and Documentation
Course: First-Year Computer Science Group Project
Institution: Toronto Metropolitan University
Year: 2025–2026
📚 Key Learnings

Through this project, I practiced:

Conducting client analysis and translating business needs into technical requirements
Designing normalized relational database schemas
Understanding three-tier web application architecture
Applying privacy and security principles to system design
Considering PIPEDA requirements when designing data-handling processes
Collaborating within a team using defined roles and responsibilities
Creating technical documentation for a real-world business problem
🔮 Future Development

If implemented, the proposed system could be developed through the following steps:

Set up the Node.js backend and PostgreSQL database.
Build the React.js frontend and appointment calendar.
Implement Firebase Authentication and role-based access control.
Integrate SendGrid and Twilio for automated notifications.
Implement privacy, consent, data retention, and audit logging features.
Test the system against representative workflows and security requirements.
Deploy the application using suitable cloud infrastructure.
⚠️ Project Status

Status: System Design / Proposal

This repository documents the analysis, architecture, database design, security specifications, and implementation plan for the proposed system. The technologies listed above represent the proposed implementation stack and were not all implemented as part of this project.

📌 Disclaimer

This project was developed for academic purposes as part of a first-year Computer Science group project at Toronto Metropolitan University. Client information and project documentation should be treated as confidential where applicable.
