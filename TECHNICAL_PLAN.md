# WorkshopNest - technical plan

**Planning document, not an implementation report.**

## Product objective

A focused, offline 2D sheet-cutting optimizer with transparent constraints and measurable waste.

## Intended system boundary

- **Input:** Synthetic cabinet and shelf cut lists with no real customer data.
- **Processing stages:** Typed part/board/constraint model; Bin-packing heuristic and repeatable seed options; SVG plan renderer and CSV import/export; Desktop workflow with saved projects.
- **Output:** A representative test set yields physically valid, documented cut plans.
- **Runtime / build stack (tentative):** Rust for optimization engine, TypeScript/Svelte for UI, Tauri for desktop packaging, Rust tests
- **Explicitly excluded:** CNC machine control, industrial safety guarantees, customer names or production orders.

## Functional modules

- Import rectangular cut lists and standard board inventories from CSV
- Respect kerf, material type, grain direction, and rotation restrictions
- Apply explainable heuristic nesting to minimize sheet use
- Produce print-ready numbered cut maps and offcut inventory
- Compare alternative cutting strategies and report material waste

## Demonstration and acceptance cases

**Test 1:** Nest a fictional cabinet into standard sheets

**Test 2:** Show why a grain-restricted part cannot rotate

**Test 3:** Compare utilization with and without reusable offcuts

## Safety, privacy, and provenance

1. Keep example datasets fictional, self-created, or appropriately licensed.
2. Run locally for the initial prototype; do not collect data on actual third parties.
3. Document origin and versions of external specifications and dependencies.
4. Exclude production credentials; put environment variable *names* only in `.env.example` if required later.
5. Do not make certification, legal compliance, professional safety, or performance guarantees without independent validation.

## Engineering unknowns and constraints

2D cutting is computationally hard; document heuristic limitations and kerf modeling clearly.

## Release definition

A first release requires a runnable prototype, verified README instructions, automated tests tied to the three demonstrations, the full LICENSE file, and an honest public GitHub development history. The roadmap estimates are hypotheses until reviewed during implementation.
