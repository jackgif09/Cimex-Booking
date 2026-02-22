# Architecture

## Non-goals

- No microservices architecture at this stage
- No React/SPA frontend
- No public self-service registration

## Key Decisions

- Use ASP.NET Core MVC as the primary web architecture
- Use ASP.NET Core Identity for admin-only authentication/authorization
- Use Entity Framework Core as the data access layer
- Include `TenantId` on business tables to support future multi-tenant SaaS evolution

## Planned Folder Structure

```text
src/
  Web/
  Domain/
  Infrastructure/
tests/
```

## Coding Rules for AI

- One issue = one feature
- No refactors unless explicitly ticketed
- Prefer async Entity Framework Core APIs
- Keep controllers thin; business logic belongs in services
