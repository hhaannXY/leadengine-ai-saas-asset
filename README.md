LeadEngine AI

AI-powered B2B Prospecting & Website Audit Platform

Status: Available for Acquisition

LeadEngine AI is a production-oriented SaaS platform designed for B2B lead generation, website analysis, AI-powered auditing, and multi-tenant workflows.

The public repository contains a technical overview of the platform. The complete functional source code is maintained in a private repository and is included in the acquisition.

1. Acquisition Overview

The buyer receives a complete software foundation that can be integrated into an existing product, internal sales workflow, marketing platform, or further developed as a standalone SaaS.

The main value of the acquisition is the existing architecture, implemented workflows, integrations, backend/frontend infrastructure, and source code, allowing a buyer to continue development without building the entire system from scratch.

2. Technology Stack
Backend
Python 3.11+
FastAPI
PostgreSQL
Redis
Celery
REST API
Frontend
Next.js
TypeScript
Tailwind CSS
Responsive web dashboard
Infrastructure
Docker
Docker Compose
Containerized application services
AI
OpenAI API
Anthropic API
Provider-based AI architecture
3. Core Platform Capabilities
B2B Lead Generation

The platform provides workflows for discovering potential business leads based on campaign parameters such as:

Location
Country
City
Business category
Lead volume

Campaigns can be created and processed through the platform dashboard.

Website Analysis

For discovered companies, the platform can perform automated website analysis covering areas such as:

Performance
SEO
Conversion-related issues
Critical website problems
Technical website issues

The resulting analysis is presented inside the dashboard.

AI Analysis

AI providers are used to analyze discovered website issues and generate actionable recommendations.

The platform can also generate personalized outreach based on the discovered problems of a specific company.

Multi-Tenant SaaS

The application includes a multi-tenant foundation designed around organizations/workspaces and isolated user data.

The architecture is designed so that the platform can serve multiple organizations from the same application infrastructure.

4. Lead Workflow

The primary workflow is:

Campaign Creation → Lead Discovery → Company Selection → Website Audit → AI Analysis → Recommendations → Personalized Outreach

A typical campaign starts with search parameters such as:

City
Country
Business category
Leads per day

After leads are discovered, a company can be selected and its website audit can be executed.

The resulting audit provides identified issues and AI-generated recommendations, which can then be used to create personalized outreach.

5. Engineering Architecture

The application is separated into frontend and backend services.

Backend

The FastAPI backend provides:

REST API endpoints
Authentication-related functionality
Organization/workspace management
Lead and campaign operations
Website audit operations
AI provider communication
Background task processing
Database interaction
Background Processing

Long-running operations are handled through background workers.

Redis is used as part of the queue/background-processing infrastructure, with Celery responsible for executing asynchronous tasks.

This allows resource-intensive operations such as lead processing and website analysis to run independently from the main API request lifecycle.

6. Data Layer

The platform uses PostgreSQL as its primary relational database.

The database layer contains the structures required for areas such as:

Users
Organizations/workspaces
Campaigns
Leads
Companies
Audits
AI-generated analysis
Application data

Database migrations and schema are included in the acquisition.

7. Authentication & Multi-Tenancy

The platform includes authentication and organization/workspace-oriented access control.

The architecture is designed around tenant separation so that multiple organizations can operate within the same SaaS environment.

Role-based access control (RBAC) is included where implemented within the application.

8. AI Provider Architecture

The platform integrates external AI providers through API-based communication.

Current providers include:

OpenAI
Anthropic

The architecture allows the AI layer to be developed independently from the rest of the application, making future provider changes or additional AI integrations possible without redesigning the entire platform.

9. External Integrations

The platform is designed to work with external services through APIs.

Depending on the deployed configuration, integrations can include services related to:

Business/lead discovery
Website analysis
AI processing
Email/outreach
Performance analysis

The exact API configuration, credentials, provider setup, and deployment environment are handled separately from the public repository and can be reviewed by a qualified buyer during technical due diligence.

10. Infrastructure & Deployment

The application is containerized using Docker.

The acquisition includes:

Docker configuration
Docker Compose configuration
Application services
Database configuration
Redis configuration
Deployment-related configuration

This provides a reproducible environment for local development and deployment.

11. Repository Structure
/backend
/frontend
/docker
/database
/docs


The private repository contains the complete functional implementation.

The public repository intentionally excludes proprietary production source code.

12. Acquisition Includes

The acquisition includes:

Complete private GitHub repository
Full functional source code
Backend source code
Frontend source code
Database schema
Database migrations
Docker configuration
Deployment configuration
REST API collection
Technical documentation
Architecture documentation
Existing application workflows
AI integration layer
Multi-tenant SaaS foundation
Intellectual property rights to the transferred work
Loom product demonstration

Third-party services, API accounts, subscriptions, and credentials are subject to their respective provider terms and are not represented as transferable assets unless explicitly agreed.

13. Current Product Status

LeadEngine AI is being offered as a technology acquisition.

The project does not currently have significant commercial traction or established recurring revenue.

The acquisition is therefore primarily focused on the technology, architecture, implemented functionality, source code, and intellectual property rather than an existing revenue-generating business.

14. Technical Due Diligence

For a serious buyer, additional technical information can be provided during the evaluation process, including:

Full lead-processing workflow
API and external-service configuration
AI provider implementation
Background worker architecture
Database structure
Authentication and multi-tenancy implementation
Deployment architecture
Repository structure
Relevant technical documentation

Access to the private repository can be provided as part of an appropriate technical evaluation process.

15. Demo

A Loom walkthrough demonstrates the main platform workflow:

Campaign → Lead Discovery → Company → Website Audit → AI Analysis → Personalized Outreach

The demonstration is available to prospective buyers.

16. Transaction

Preferred transaction methods:

Escrow.com
Wire transfer

Alternative arrangements can be discussed privately.

The final transaction structure, scope of transferred IP, and included assets will be agreed upon before completion of the acquisition.

17. Contact

LeadEngine AI

Email:
midorimavpotoke@gmail.com

X:
https://x.com/17rainLF
