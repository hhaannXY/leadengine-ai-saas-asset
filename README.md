LeadEngine AI

Status: Available for Acquisition

LeadEngine AI is an MVP with production infrastructure designed for AI-powered B2B lead generation, website analysis, and automated outreach workflows.

The platform combines business discovery, automated website auditing, AI-powered analysis, personalized outreach generation, SaaS authentication, usage limits, background processing, and billing infrastructure.

Technology Stack
Backend
FastAPI
Python 3.11+
PostgreSQL
SQLAlchemy
Alembic
Redis
Celery
Frontend
Next.js
TypeScript
Tailwind CSS
React
Infrastructure
Docker
Docker Compose
Nginx
Prometheus
Grafana
Flower
Core Capabilities
B2B business discovery
AI-powered website audits
SEO analysis
Performance analysis
SSL and domain checks
Conversion analysis
AI-generated business insights
Personalized cold email generation
LinkedIn message generation
Loom script generation
PDF report generation
Automated email delivery
Follow-up email scheduling
Multi-tenant user data isolation
Usage and plan limits
Stripe billing integration
White-label branding foundation
REST API
Background task processing
Lead Generation Workflow

The main workflow is implemented end-to-end:

User creates a campaign with targeting parameters.
The system searches for businesses matching the selected criteria.
Discovered leads are stored and scored.
A website audit can be triggered for a lead.
Multiple technical checkers analyze the website.
AI analyzes the collected audit data.
The system generates personalized outreach content.
A PDF audit report can be generated.
Outreach emails can be sent through the configured email provider.
Follow-up sequences can be scheduled.
Business Discovery

The platform supports multiple external data sources:

Google Places API
SerpAPI
Yelp Fusion API
Mock provider fallback

The discovery layer uses provider fallbacks so the application can operate in demo/mock mode when external API credentials are unavailable.

Lead information may include:

Business name
Website
Phone
Email
Address
City
State
Country
Rating
Review count
Business category
Source
Website Audit Engine

Website audits are performed through multiple independent checkers.

Technical Checks
SSL validity
Domain information
Website performance
SEO metadata
H1/title/meta analysis
Sitemap and robots.txt
Broken-link checks
Conversion elements
Contact forms
Phone CTAs
Chat/review elements

The checkers can run asynchronously as part of the audit workflow.

AI Layer

The AI layer currently supports:

OpenAI
Anthropic

OpenAI is used as the primary provider, with Anthropic available as an alternative/fallback provider.

AI is used for:

Website audit analysis
Identification of critical issues
Business-impact analysis
Recommended fixes
Priority scoring
Personalized email generation
LinkedIn message generation
Loom script generation

The code contains a provider abstraction layer, making it possible to add or replace providers without redesigning the entire application.

Current limitation: model names are configured in code rather than being fully runtime-configurable.

Background Processing

Background processing is implemented using:

Celery
Redis
Celery Beat

Separate task queues are used for workloads such as:

Website audits
Email delivery
Cleanup tasks
Follow-up sequences
Failed email retries

Tasks include retry mechanisms and scheduled execution.

SaaS / Authentication

The platform includes:

User registration
Login/logout
JWT authentication
HttpOnly cookies
Password hashing with bcrypt
Password reset
Email verification
User-level data isolation
Usage quotas
Subscription plans
Stripe billing integration

Current plans include:

Trial
Starter
Growth
Agency

Current limitation: the application currently uses a single user role. A separate role-based access-control system is not implemented.

Infrastructure

A production Docker Compose configuration is included with services for:

PostgreSQL
Redis
FastAPI backend
Next.js frontend
Celery workers
Celery Beat
Flower
Prometheus
Grafana
Nginx

Health checks and persistent volumes are configured.

The infrastructure provides a strong foundation for deployment, but additional operational hardening would be required for large-scale production use.

Testing & CI/CD

The current project does not contain a meaningful automated test suite.

Current state:

Automated unit tests: Not implemented
Integration tests: Not implemented
E2E tests: Not implemented
CI/CD pipeline: Not active
GitHub Actions: deployment template only

The application has been manually tested through the API and application interface.

Current Technical Limitations

The project is an MVP and has several areas that a buyer may want to develop further:

No meaningful automated test coverage
No active CI/CD pipeline
Basic scraping rather than sophisticated crawling
No JavaScript browser rendering for scraping
Limited request/concurrency management
No automated database backup strategy
No disaster-recovery system
No horizontal scaling configuration
No centralized log aggregation
No advanced role/permission system
AI model names are not fully runtime-configurable

These are primarily operational and scaling improvements, rather than a requirement to redesign the core architecture.

Documentation

The repository contains technical and project documentation covering areas such as:

Installation
Deployment
Architecture
Features
API configuration
Security
Privacy
Terms of Service
SLA
Project setup
Acquisition Includes

The acquisition includes:

Full source code
Complete GitHub repository
Backend
Frontend
Database schema
Docker configuration
Deployment configuration
API configuration
Documentation
Architecture
Intellectual property transfer
Product demonstration

The codebase uses standard open-source frameworks and libraries.

Third-party API credentials and external service accounts are not included in the acquisition and would need to be configured by the buyer.

Current Product Position

LeadEngine AI should be considered a functionally developed MVP with production infrastructure, rather than a mature enterprise SaaS.

Its primary value for a technical buyer is the existing:

Software architecture
Lead-generation workflow
Website audit engine
AI integration layer
SaaS foundation
Background-processing infrastructure
Billing integration
Docker deployment environment
Documentation

A technical team can use the existing foundation to continue development, integrate the technology into an existing product, or develop it into a standalone SaaS.

Acquisition

LeadEngine AI is available for acquisition.

The transaction includes the complete software codebase and intellectual property.

Preferred transaction methods:

Escrow.com
Wire transfer

Other arrangements can be discussed privately.

Contact

Email:
midorimavpotoke@gmail.com

X:
https://x.com/17rainLF

This repository is provided as a technical overview of LeadEngine AI for acquisition discussions. The project is presented transparently as an MVP with production infrastructure and known areas requiring further development.
