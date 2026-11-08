# WorkshopNest

> Grain-aware cutting-layout optimization for small workshops.

**Current state:** Documentation starter / proposed product. The presence of this README does **not** mean the software has been implemented, deployed, used. Update this status to reflect real work.

## What it is

WorkshopNest is a proposed specialist software tool for Cabinetmakers, carpenters, small CNC shops, and furniture makers. Small workshops need useful cut plans with grain and offcut constraints without buying complex manufacturing suites. The intended differentiation is: A focused, offline 2D sheet-cutting optimizer with transparent constraints and measurable waste.

## Intended users and use cases

- Nest a fictional cabinet into standard sheets
- Show why a grain-restricted part cannot rotate
- Compare utilization with and without reusable offcuts

## Planned features

- Import rectangular cut lists and standard board inventories from CSV
- Respect kerf, material type, grain direction, and rotation restrictions
- Apply explainable heuristic nesting to minimize sheet use
- Produce print-ready numbered cut maps and offcut inventory
- Compare alternative cutting strategies and report material waste

## Proposed technology

Rust for optimization engine, TypeScript/Svelte for UI, Tauri for desktop packaging, Rust tests

These technologies are *planned*, not a claim that dependencies have already been installed or code has been written. Revise this section when actual implementation decisions are made.

## Proposed architecture

- Typed part/board/constraint model
- Bin-packing heuristic and repeatable seed options
- SVG plan renderer and CSV import/export
- Desktop workflow with saved projects

See [TECHNICAL_PLAN.md](TECHNICAL_PLAN.md) for technical boundaries and acceptance tests.

## Running locally

**Not yet runnable.** This package contains documentation templates, not software. When a functioning implementation is available, replace this paragraph with tested prerequisites, install instructions, a verified executable command, and a reproducible example using `Synthetic cabinet and shelf cut lists with no real customer data.`

## Data boundaries and exclusions

CNC machine control, industrial safety guarantees, customer names or production orders. All public examples should use Synthetic cabinet and shelf cut lists with no real customer data.

## Known limitations / validation risks

2D cutting is computationally hard; document heuristic limitations and kerf modeling clearly.

## Development roadmap

Work is broken into estimated, not-yet-completed milestones in [ROADMAP.md](ROADMAP.md). They are *planning estimates*, not an assertion that development has begun or that work will definitely be performed.

## Business direction

Potential commercial extensions: Pro desktop features, specialized machine exporters, and professional support. 

## Contributing and licensing

License: [Mozilla Public License 2.0](LICENSE) (`MPL-2.0`). The distribution contains the complete license text. Any future source files can include the SPDX identifier `MPL-2.0` and the Exhibit A notice where appropriate. Rights in contributions and project ownership must be verified before licensing.

