# Roadmap

## M1 — Repository Foundation

- Establish repository scaffolding and baseline documentation
- Define architecture, coding rules, and development constraints
- Configure issue and pull request templates

## M2 — Domain and Data Foundation

- Define initial domain entities for bookings, services, and customers
- Add EF Core DbContext and baseline migrations
- Configure PostgreSQL connectivity and environment-based settings
- Add repository/service abstractions for core workflows

## M3 — Admin Identity Baseline

- Integrate ASP.NET Core Identity for admin-only authentication
- Seed initial admin account workflow for non-production environments
- Add role-based access guards for administrative areas
- Establish secure password and sign-in policies

## M4 — Booking Workflow (Public Intake)

- Implement customer booking request entry pages (MVC)
- Add server-side validation and anti-forgery protections
- Persist booking requests with status tracking
- Add basic confirmation messaging and audit timestamps

## M5 — Admin Portal Operations

- Build admin dashboard for viewing and filtering bookings
- Add booking lifecycle actions (approve, schedule, complete, cancel)
- Add customer details and service history views
- Add internal notes support for operational follow-up

## M6 — Deployment and Operations

- Prepare production configuration for AWS Elastic Beanstalk
- Add CI checks for build, tests, and migration safety
- Add structured logging and error handling policies
- Document deployment, rollback, and environment variable requirements

## M7 — SaaS Readiness

- Enforce tenant boundaries across business data access
- Add tenant-aware querying and service-layer guardrails
- Define onboarding approach for future tenant provisioning
- Document scaling path and architecture constraints before multi-tenant launch
