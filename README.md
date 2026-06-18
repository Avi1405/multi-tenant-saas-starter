# Multi-Tenant SaaS Starter

A product-style SaaS foundation with organizations, roles, billing, quotas, and audit logs.

## Why this repo exists

This project is meant to show that I can build software the way real product teams do: with tenant boundaries, permissions, billing, observability, and a clean admin experience.

## MVP

- User authentication and account creation
- Organization creation and invite flow
- Role-based access control for members and admins
- Tenant-aware data model with strict isolation
- Billing-ready subscription flow
- Usage quotas and plan limits
- Audit log for sensitive actions
- Email notifications for invites and billing events

## Build plan

### Phase 1: Core platform

- Set up auth and session handling
- Model users, organizations, memberships, and roles
- Enforce tenant boundaries in every query path
- Add invite acceptance and role management

### Phase 2: Product layer

- Add billing plans and subscription states
- Track usage and quotas per tenant
- Surface upgrade prompts and account status
- Add background jobs for billing and emails

### Phase 3: Operational quality

- Add audit logging for important actions
- Add admin views for tenant health and usage
- Add seeded demo data for easy walkthroughs
- Add tests for authorization and tenant isolation

### Phase 4: Polishing the product story

- Add onboarding steps for a new workspace
- Add a simple analytics panel for admins
- Add strong error states and empty states
- Add deployment notes and screenshots for the README

## Stretch goals

- SSO or social login
- Team provisioning hooks
- Exportable reports
- Usage alerts before plan limits are hit

## What success looks like

- The app feels like a real B2B product
- Tenant isolation is obvious and well tested
- Billing and roles are handled cleanly
- A recruiter can see product engineering, not just CRUD pages

## Notes for v1

Build one sharp vertical slice first: create an org, invite a member, restrict access, and show usage. That single flow will communicate far more than a long checklist of half-finished features.
