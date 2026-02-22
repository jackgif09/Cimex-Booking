# Immediate Next Step Recommendation

## Recommended next step

Start **M2 — Domain and Data Foundation** by implementing the first vertical slice:

1. Create a `BookingRequest` domain entity in `src/Domain` with status, customer contact, requested service date, and audit timestamps.
2. Add an EF Core `DbContext` in `src/Infrastructure` and map the entity.
3. Wire PostgreSQL connection settings in `src/Web/appsettings*.json` and dependency injection in `Program.cs`.
4. Add the first migration and verify the app can create/update the database.

## Why this should be next

- The repository already has baseline architecture and documentation in place (M1 outcomes).
- Domain and persistence are prerequisites for both public booking intake (M4) and admin operations (M5).
- Identity setup (M3) is easier to validate once there is real data to protect.

## Definition of done for this step

- `BookingRequest` entity and supporting enums/value objects are committed.
- EF Core migration is generated and checked in.
- App starts successfully with database connectivity configured by environment.
- At least one automated test validates domain rules for booking creation.
