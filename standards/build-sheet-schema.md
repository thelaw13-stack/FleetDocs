# Fleet Canonical Build Sheet Schema

Version 3.0

## Purpose

Provide one consistent, copyable, human-readable dashboard for every fleet asset. It answers: **What is this asset today?**

## Immutable section order

1. Title and subtitle
2. At a Glance — Status, ODO, Role, Next Service, Value
3. Identity — Purpose, Mission
4. Asset — Year, Make, Model, Trim, VIN, Color, Engine, Transmission, Fuel, Power, Primary Shop, Notes
5. Configuration — Engine, Fuel, Cooling, Exhaust, Drivetrain, Suspension, Brakes, Body, Interior, Electrical, Wheels / Tires
6. Maintenance — Status, Last Service, Current State, Next
7. Wishlist — Priority A, B, C
8. Ownership Costs — Original Purchase, Transfer Value, Known Upgrades, Owner Investment, Maintenance, Insurance Repairs
9. History — brief index only
10. References — Vehicle History, Technical Specifications, Service Log, Parts Catalog, Photo Archive
11. Design Philosophy

Do not rename, add, remove, or reorder sections in an asset Build Sheet. Use `UNKNOWN`, `TBD`, `N/A`, or an empty subsection rather than changing the schema.

## Configuration subsystem classification

Classify a component by the system it **primarily serves**, not by the fluid passing through it.

- **ENGINE** — components primarily responsible for engine structure, internals, forced induction, crankcase ventilation, and the **oil (lubrication) system**: oil storage, filtration, circulation, pressure control, pumps, sumps, and general engine-oil plumbing.
- **COOLING** — thermal-management hardware whose primary function is heat rejection or temperature control: coolant radiators, oil coolers, intercoolers / charge-air coolers, dedicated fans, thermostats, and the lines and fittings that primarily serve one of those assemblies.

Supporting hardware (hoses, lines, fans, fittings) follows the assembly it primarily serves. Do not split one purchased assembly into invented separate parts; record the kit under the subsystem matching its principal function and describe the rest in the item detail.

## Version note

Schema 3.0 removed the `Lubrication` Configuration subsystem and added `Cooling` (a breaking change from 2.0). Oil-system hardware moves to `Engine`; dedicated heat-rejection assemblies move to `Cooling`. Records that declare Schema 2.0 remain historically valid under 2.0; a 2.0 record validated against 3.0 will report an undefined subsystem and should be migrated or validated against its declared version. See `CHANGELOG.md`.

The status legend belongs in the standard, not in every asset:

- GOOD — verified, healthy, or complete
- WISHLIST — planned or future upgrade
- ACTION — needs attention
- INFO — reference information
- HISTORY — historical record
