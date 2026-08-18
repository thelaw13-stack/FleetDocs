# Changelog

All material standard and fleet-record changes are recorded here.

## 2026-08-17 — Build Sheet Schema 3.0 (breaking)

- **Removed the `Lubrication` Configuration subsystem; added `Cooling`.** Rationale: on an enthusiast build sheet, "Lubrication" read as an oil-system catch-all that mixed heat-rejection hardware (oil coolers) with engine-oil hardware (sumps, filters, plumbing). Schema 3.0 classifies by the system a component primarily serves: oil-system hardware belongs to `Engine`; dedicated heat-rejection assemblies (coolant radiators, oil coolers, intercoolers/charge-air coolers, fans, thermostats) belong to `Cooling`.
- **Compatibility:** breaking. Records that declare Schema 2.0 remain historically valid under 2.0. A 2.0 record validated against 3.0 reports an undefined subsystem (`Lubrication`) via FleetOS's unexpected-subsection diagnostic and should be migrated or validated against its declared version. Records do not yet carry a schema-version field; true version-aware validation is a future change and is not implemented here.
- **Migration impact:** only one canonical asset exists (1970 VW Baja). It was migrated individually, not mechanically: the remote oil cooler + electric fan moved to `Cooling`; the deep sump, remote spin-on filter, and braided AN oil plumbing moved to `Engine`. The plumbing's routing is unresolved and is recorded as general oil-system plumbing — no claim that it feeds the cooler circuit. The Baja `parts-catalog.md` never used `Lubrication` and was unaffected.
- Population Standard unchanged (this is a schema change only).

## 2026-08-16 — Initial canonical release

- Established Governance 1.0.
- Froze Canonical Build Sheet Schema 2.0.
- Established Population Standard 1.0.
- Added companion-document standards and templates.
- Added the 1970 Volkswagen Type 1 Baja Bug as the first fleet asset.
- Marked unverified Baja facts as owner-record, estimated, pending verification, or unknown.
