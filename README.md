# bosque-digital-thread

> An independently reconstructed digital thread for Bosque County, Texas — built exclusively
> from public information requests and state data sources.

![Status](https://img.shields.io/badge/status-MVP--in--development-purple)
![Operator](https://img.shields.io/badge/operator-squidWorks--LLC-6d4aff)
![Parent](https://img.shields.io/badge/a--H.%20H.%20Holdings%20Company-grey)

**Owned & operated by squidWorks, an H. H. Holdings Company entity.**

---

## 🧭 What is this?

**bosque-digital-thread** is an independent platform that reconstructs the operational
trail of Bosque County, Texas government — permits, minutes, assets, budgets, payments —
from **publicly available sources**: public information requests, published records, and
state-level databases.

No county contracting, no cooperation, no interlocal agreement. This is built from what
any citizen of the United States can lawfully access.

> Every county record traces through **paper, spreadsheets, and siloed systems** — with no
> connected audit trail. We build the connected layer, publicly.

---

## 🏢 Model

```
H. H. Holdings Company
        │
        └─▶ squidWorks
             (owns & operates the platform)
                    │
                    └─▶ bosque-digital-thread
                         (public-source reconstruction of
                          Bosque County, Texas government)
```

- **No county contracting.** No interlocal agreement, no service contract, no data-sharing
  MOU. Purely public-records-driven.
- **Data sources are public.** Everything in the platform derives from publicly available
  information — published minutes, published agendas, statutory disclosures, state
  agency datasets, and public information requests.
- **No official status.** This platform is independent of Bosque County and is not
  endorsed by, affiliated with, or operated on behalf of Bosque County, Texas.

---

## 🧱 The Four Elements (independent reconstruction)

| Element                     | Adaptation                                                          |
|-----------------------------|---------------------------------------------------------------------|
| Digital Engineering Ecosystem | Open data portals, state agency APIs, county-published records   |
| Digital Models              | Canonical entity models (JSON schemas) stitching public records    |
| Digital Thread              | Append-only event log keyed by `county_object_id`                  |
| Digital Artifacts           | Auto-generated views: permit lookups, project trackers, extracts   |

---

## 🎯 MVP Scope

Two end-to-end threads sharing one backbone:

**Thread A — Road & Bridge Project (Precincts 1–4)**

Reconstructed from published county court minutes, court administrator records,
purchasing disclosures, and GIS data.

**Thread B — OSSF (Septic) Permit**

Reconstructed from state-authorized OSSF program filings and inspection disclosures.

---

## 📋 Data Sources

- Published county agendas, minutes, and budget documents
- County auction, procurement, and PO disclosures
- State agency disclosures (e.g., environmental, licensing, permitting data)
- Statutorily required public disclosures
- Open records responses obtained via the Texas Public Information Act
  (Texas Gov't Code Ch. 552)

---

## 🧮 Approach

1. **Harvest** — pull published records and disclosures from public portals.
2. **Request** — where records aren't proactively published, submit public
   information requests under Texas Gov't Code ch. 552.
3. **Normalize** — map records onto the canonical entity model.
4. **Stitch** — link records by object ID across departments, offices, and
   precincts.
5. **Publish** — auto-generate views: project trackers, permit lookups,
   timeline visualizations.

---

## ⚖️ Legal & Compliance Notes (Texas)

- **Civil application.** This platform is a civic, educational, and transparency
  project for citizens — not a commercial data product. Its application is civil
  and public in nature.
- **Public information access.** Where feasible, requests are framed to qualify for
  reduced or waived fees under civil-application mechanisms where they exist in
  Texas practice. We pursue lawful cost minimization, not evasion.
- **Sources:** all claims trace to public records, filed requests, or reported
  government disclosures. Nothing is extrapolated.
- **Lawfulness:** no bypassing of access controls, scraping behind auth, or
  scraping of non-public data. Only public documents and public interfaces.

---

## ⚖️ Boundaries

- **Not affiliated** with Bosque County, Texas government.
- **Not a replacement** for official records; official sources are authoritative.
- **No implied endorsement** by Bosque County, any elected official, or staff.

---

## 🚀 Getting Started

```bash
git clone https://github.com/squidWorks/bosque-digital-thread.git
cd bosque-digital-thread

# Local dev stack (planned)
docker compose up
```

> 🔨 **Note:** the repository is bootstrapping. Schema drafts, data-collection
> runbooks, and pilot extracts are landing incrementally.

---

## 📁 Repository Layout (planned)

```
/sources      Registered public data sources & extraction runbooks
/etl          Normalization, stitching, entity resolution pipeline
/schemas      Canonical entity definitions (Asset, CaseRequest, CourtAction, ...)
/artifacts    Auto-generated artifacts (agenda packets, permit lookups, trackers)
/docs         Methodology, compliance notes, methodology ADRs
/pilot        OSSF permit proof-of-concept runbook
```

---

## 👥 Governance

- **Operator:** squidWorks — builds and operates the platform.
- **Methodology record:** ADRs in `/docs/adrs` document data-source decisions,
  normalization rules, and public-exposure scopes.

---

## 🤝 Contributing

Contributions to methodology, data sourcing, or analysis are welcome:

1. Open an issue describing the proposed change.
2. Schema changes require an ADR.
3. All claims require a cited, accessible public source.

---

## 📄 License

Licensing TBD. All underlying public records remain the property of their
respective public bodies.

---

<div align="center">
  <sub>Built with 🦑 by <strong>squidWorks</strong> · an H. H. Holdings Company entity</sub><br>
  <sub>Public information, reconstructed for the citizens of America.</sub>
</div>
