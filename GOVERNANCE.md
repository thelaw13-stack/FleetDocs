# Fleet Build Sheet Governance

Version 1.0

## Purpose

The Fleet Build Sheet System is governed by two independent artifacts:

1. Fleet Canonical Build Sheet Schema — defines **what exists**.
2. Fleet Population Standard — defines **how it is populated**.

The schema provides stability. The population standard provides continuous improvement.

## Rule 0 — Schema stability

The Build Sheet schema is the fleet database and should remain stable. Before changing it, ask whether the improvement can be achieved through the Population Standard. If yes, do not modify the schema.

## Change control

Schema changes are rare and require a documented rationale, compatibility review, schema version increment, migration impact, and a separate change from population improvements.

Population Standard changes require a documented rationale, before/after examples, a version increment, and preservation of existing Build Sheet compatibility whenever possible.

Companion standards version independently.

## Agent requirements

Every contributor shall:

1. Read this governance file and the current standards before editing a fleet record.
2. Preserve the canonical schema and section order.
3. Follow the latest Population Standard.
4. Never invent facts or promote assumptions to facts.
5. Distinguish `VERIFIED`, `ESTIMATED`, and `UNKNOWN`.
6. Keep a Build Sheet as a concise dashboard, not an encyclopedia.
7. Put chronology, engineering detail, receipts, and maintenance events in their companion records.
8. Propose schema changes separately from population improvements.
9. Never silently redesign the template in chat or in an asset record.
10. Treat FleetDocs as the canonical source; repository standards override remembered chat conventions.

## Companion documents

The Build Sheet references but does not replace Vehicle History, Technical Specifications, Service Log, Parts Catalog, Photo Archive, or receipts and invoices.
