# Secure-Appointment-and-Management-System
A real-client system design project completed as part of a first-year Computer Science group project at Toronto Metropolitan University (2025–2026).


📋 Project Overview
A financial consultant client approached our group with a real-world business problem: their appointment scheduling, client follow-up, and workflow management processes were entirely manual, inefficient, and lacked data security. Sensitive client information was being handled without proper compliance measures.
Our team analyzed the client's workflow, identified the core pain points, and designed a comprehensive solution — a secure, three-tier CRM-style web application to automate appointment scheduling, follow-up reminders, and client data management.

Note: This repository contains the full system design documentation across all project phases. The application is a proposed and designed solution, not a deployed codebase.


🎯 The Problem
The client faced three core challenges:

Scheduling inefficiencies — appointments were tracked manually with no automated reminders, leading to missed follow-ups
No centralized client data management — client information was scattered across spreadsheets and email threads
Security & compliance gaps — sensitive financial client data was not handled in accordance with PIPEDA (Canada's federal privacy law)


💡 Proposed Solution
We designed a full-stack, three-tier web application with the following architecture:
LayerTechnologyFrontendReact.jsBackendNode.jsDatabasePostgreSQLAuthenticationFirebase AuthenticationEmail NotificationsSendGridSMS RemindersTwilioData CompliancePIPEDA-compliant data handling
Core Features Designed

Appointment Scheduling Module — calendar-based booking with conflict detection
Automated Follow-up System — SendGrid email + Twilio SMS reminders triggered by appointment status
Role-Based Access Control — admin, consultant, and client access tiers
Secure Client Portal — Firebase Authentication with encrypted data storage
Database Schema — normalized PostgreSQL schema with relationship mapping for clients, appointments, and follow-ups
PIPEDA Compliance Layer — consent management, data retention policies, and audit logging


📁 Repository Contents
FileDescriptionClient Identification.pdfInitial client intake — business context, pain points, and project scopephase2 DESIGN DOCUMENT.docxFull system design: architecture diagrams, database schema, UI/UX workflows, and data flow diagramsPhase3 (1).docxFinal solution proposal: security specifications, compliance requirements, and implementation roadmapProject DescriptionOriginal project brief and requirementsGROUP COLLABORATION AGREEMENT.pdfTeam roles, responsibilities, and collaboration terms

🏗️ System Architecture (Designed)
┌─────────────────────────────────────────┐
│           React.js Frontend             │
│   (Appointment UI, Client Portal,       │
│    Admin Dashboard)                     │
└──────────────────┬──────────────────────┘
                   │ REST API
┌──────────────────▼──────────────────────┐
│           Node.js Backend               │
│   (Business Logic, Auth Middleware,     │
│    Notification Triggers)               │
└──────┬───────────────────┬──────────────┘
       │                   │
┌──────▼──────┐    ┌───────▼────────────┐
│ PostgreSQL  │    │ Firebase Auth +    │
│  Database   │    │ SendGrid / Twilio  │
└─────────────┘    └────────────────────┘

👥 Team

Sojas Singh Batra — System Architecture, Database Design, Security & Compliance Specifications
Group members — Client Analysis, UI/UX Workflow Design, Documentation

Course: First-Year Computer Science Group Project, Toronto Metropolitan University
Year: 2025–2026

📚 Key Learnings

Conducting real client interviews and translating business needs into technical requirements
Designing normalized relational database schemas
Understanding three-tier web application architecture
Applying privacy legislation (PIPEDA) to system design decisions
Collaborating across a team with defined roles and a formal agreement


🔮 Future Development
If implemented, the next steps would be:

Set up Node.js backend with PostgreSQL connection
Build React.js frontend with appointment calendar component
Integrate Firebase Authentication for secure login
Configure SendGrid and Twilio for automated notifications
Deploy on cloud infrastructure (AWS or Vercel + Railway)
