# WorkshopNest - development roadmap

**Status:** Planned work only. None of the boxes are marked completed. Estimates are rough.

## Product-level acceptance criterion

A representative test set yields physically valid, documented cut plans.

## Estimated work breakdown

| Step | Milestone | Estimated hours | Observable outcome |
|---|---|---:|---|
| 1 | Specify geometry and input formats | 8 | Validated cut list and board schemas |
| 2 | Implement baseline nesting heuristic | 12 | Deterministic placements for sample datasets |
| 3 | Apply grain/kerf/rotation constraints | 10 | No placed part violates declared constraints |
| 4 | Create SVG cut sheet exporter | 9 | Printable and labeled layouts |
| 5 | Add offcuts and comparison | 9 | Material utilization metrics compare alternatives |
| 6 | Test, benchmark, and document | 10 | Benchmarks use synthetic boards only |
| | **Total estimated** | **58** | |

## Detailed milestones

### 1. Specify geometry and input formats (8 estimated hours)

- [ ] Deliverable: Validated cut list and board schemas.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 2. Implement baseline nesting heuristic (12 estimated hours)

- [ ] Deliverable: Deterministic placements for sample datasets.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 3. Apply grain/kerf/rotation constraints (10 estimated hours)

- [ ] Deliverable: No placed part violates declared constraints.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 4. Create SVG cut sheet exporter (9 estimated hours)

- [ ] Deliverable: Printable and labeled layouts.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 5. Add offcuts and comparison (9 estimated hours)

- [ ] Deliverable: Material utilization metrics compare alternatives.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

### 6. Test, benchmark, and document (10 estimated hours)

- [ ] Deliverable: Benchmarks use synthetic boards only.
- [ ] Add tests or demonstrations proving the deliverable works.
- [ ] Record a genuine development commit and update documentation only after the work occurs.

## QA and release gates

- [ ] A real runnable implementation exists, with verified setup commands in `README.md`.
- [ ] Automated tests pass in a clean environment and failures are actionable.
- [ ] Only fabricated, original, openly licensed, or otherwise authorized sample data is published.
- [ ] No passwords, API keys, secrets, customer records, or employer/client confidential artifacts appear in repository history.
- [ ] A source-linked change log and actual progress notes distinguish finished work from plans.
- [ ] The GitHub history preserves authentic work and authorship; do **not** manufacture or backdate commits.

## Parking lot and risks

- Technical: 2D cutting is computationally hard; document heuristic limitations and kerf modeling clearly.
- Commercial hypothesis (not validated): Pro desktop features, specialized machine exporters, and professional support.
- Beyond MVP: defer paid extensions and hosted features until the underlying product works.
