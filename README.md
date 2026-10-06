# Coexistence Conditions for Computation in Driven Disordered Optical Cavities

**Status: work in progress, pre-experimental. Revision 2.3.2 (2026-10-05). Reference 5 (You, Arai & Sunada) has now been read; it challenges the attribution test in §4 and §5's first requirement. Revision 3 is in preparation.**

A short technical note on when a driven, open, disordered optical cavity can compute rather than merely project. It proposes a measurable test for nonlinearity inside the cavity — a necessary condition only — and lists the further requirements that would have to hold at the same operating point. Whether that operating point exists is the open problem the note is built around; nothing here claims it does.

The note is published as a single self-contained page: `index.html`.

## What the note argues

1. **The linearity constraint has a scope.** A linear cavity driven through its input field computes no nonlinear function of the input history, however high the rank of its map. That holds only when the data enter as the drive. When the data modulate the cavity's scattering potential, multiple scattering yields a nonlinear map from data to output with linear optics (structural nonlinearity).
2. **The kernel test, with the port and boundary declared.** Nonlinearity shows up as the lowest nonvanishing kernel of order two or higher, sourced inside a declared system boundary (input port to output field, before any detector), with support on the photon-lifetime scale. Second order is the usual probe, but symmetry can forbid it (a Kerr cavity with phase-sensitive readout has no second-order term), so the test does not stop there. It must also say where the input enters. Detector nonlinearity alone caps the achievable order at two, though passive reservoirs relying on it have still performed well on benchmark tasks. The test detects nonlinearity; it does not measure dimensionality, memory or task performance.
3. **Requirements of different kinds must coexist:** three necessary conditions (nonlinearity in the recurrence, memory matched to the drive, consistency), one threshold (readout above the noise floor) and one figure of merit (dimensionality). Modal overlap is reported as a diagnostic only. The requirements are coupled through one complex spectrum, so improving one tends to cost another. The note shows tensions, not that the requirements cannot all be met — and not that they are a complete account of computation.

## Revision history

**Revision 2.3.2 (2026-10-05)** — status update
- Reference 5 read in full. It reaches high-order nonlinear capacity with linear optical memory and no nonlinearity in the recurrence, which challenges §5's first requirement as a necessary condition and the attribution test in §4. Body text unchanged pending revision 3.

**Revision 2.3.1 (2026-10-05)** — DOI pass
- Resolved the DOIs for refs. 11 and 18 and the volume of ref. 17.
- Reading ref. 18 in full corrected an error from rev. 2.3: its spoken-digit result was simulated; the experiments were Boolean tasks with memory and header recognition.

**Revision 2.3 (2026-10-05)** — corrective, after external reviews by two AI instruments
- Retitled from "A Coexistence Criterion" to "Coexistence Conditions".
- Defined the system boundary, the memory scope (memory carried by the cavity field) and the time-invariance assumption; added a source term to Eq. (1).
- Gave r_eff an operational, noise-thresholded definition; corrected the claim that nonlinear order grows with photon lifetime.
- Renamed §4 "The kernel test", removed the claim that it collapses several properties into one, and added attribution controls.
- Softened the detector-nonlinearity argument with a counter-example (Vandoorne et al. 2014), admitted as an exception to the freeze.
- Labeled each requirement by kind, demoted modal overlap to a diagnostic, added a status-of-claims summary, and retitled §6 as a survey.

**Revision 2.2.2 (2026-10-05)** — corrective
- Audited every reference's provenance line. Several described search-result or third-party checks as primary-record checks; each now states who checked it and what was actually seen. No reference was found to be wrong.

**Revision 2.2.1 (2026-10-05)** — corrective
- Demoted the microwave scale-model section to an open item: it had entered the note as a full section before any thresholds were registered.
- Froze the note pending a full reading of reference 5, on which the gap claim in §4 depends.
- Both changes follow an internal review of epistemic drift across revisions 2 to 2.2.

**Revision 2.2 (2026-10-05)**
- Added a proposed microwave scale-model test as a section (demoted to an open item in 2.2.1).
- Added del Hougne & Lerosey (Phys. Rev. X, 2018) and two open items.

**Revision 2.1 (2026-10-04)**
- Generalized the kernel criterion from second order to the lowest nonvanishing kernel of order two or higher, with a symmetry caveat.
- Rewrote the overstated "random projection, not computation" sentence.
- Added the detector-nonlinearity ceiling and the information processing capacity framework (Dambre et al., 2012).
- Added a comparison with other reservoir classes as an open item.
- The first two changes respond to an external AI review of revision 2.

**Revision 2 (2026-10-04)**
- Scoped the linearity constraint to source-port encoding and added the structural route.
- Required the input port to be declared in the Volterra criterion.
- Withdrew the claim that gain saturation generically collapses dimensionality; replaced it with a weaker statement supported by the cited literature.
- Rewrote the noise condition: critical slowing down near an instability is treated as the main shared amplifier of signal and noise, with mode non-orthogonality (Petermann factor) as a secondary penalty.
- Added consistency as a sixth condition.
- Added an evidence section, an open-items section, and a verified reference list.
- Raised all small type to legible sizes (body text at least 1rem, utility text at least 0.72rem).

**Revision 1.** Original note: five conditions, no references.

## Open items

These are unresolved in revision 2 and are listed in §7 of the note.

1. Revise §4 and §5 in light of You, Arai and Sunada (*Opt. Express* 33, 24982, 2025), now read: its nonlinearity is encoder-side, not structural, but it computes without nonlinearity in the recurrence.
2. Find a source for Petermann-factor statistics in chaotic open cavities before making any claim about how they scale with modal overlap.
3. Check whether the structural-reservoir comparison in Venâncio et al. (arXiv:2609.02733) isolates the second modulator pass from its other hardware differences.
4. The noise argument rests on sensing results; a direct result for reservoir readout near a bifurcation is still needed.
5. Han et al. (*Laser Photonics Rev.* e03155) is in early view; recheck volume and issue before any archival version.
6. Write out how the kernel test classifies extreme learning machines and delay-based reservoirs.
7. The microwave scale-model test stays a proposal until numeric pass and kill thresholds are registered.
8. Argue for a link between resolved modes and computational capacity, or drop modal overlap entirely.
9. Build an evidence matrix (systems against requirements) from full texts only.

## Verification

Each of the 18 references was matched to its title and authors before deployment. A matched citation is not verified content, so the note records, under every reference, who checked it (Nils, Claude, or another AI instrument) and what was actually seen:

- **Full text read:** refs. 4, 5, 12 and 14 (PDFs supplied by Nils), ref. 18 (publisher page) and the preprint of ref. 2.
- **Record fetched or seen in search results:** most others. Where a claim in the note rests only on an abstract or excerpt (refs. 3, 8, 9, 15, 16), the line says so.

An earlier version of these lines described several search-result checks as primary-record checks. That was corrected in revision 2.2.2.

Checks were cross-run across several AI instruments and treated as readings, not authorities. Where instruments disagreed (one reported the DOI for Parto et al. as invalid), the disagreement was settled against the primary record (PMC13588183), not by majority.

## Before pushing to GitHub Pages

- [ ] Every font named in CSS is loaded (IBM Plex Sans, Serif and Mono via Google Fonts, with system fallbacks).
- [ ] Body text at least 1rem; smallest utility text at least 0.72rem.
- [ ] No `-webkit-font-smoothing: antialiased` on dark backgrounds.
- [ ] MathJax renders all equations, including (5a), (8a) and the revised (10).
- [ ] Opened on a real phone in light and dark modes.

## License

CC0 1.0 Universal. No rights reserved.
