# A Coexistence Criterion for Computation in Driven Disordered Optical Cavities

**Status: work in progress, pre-experimental. Revision 2 (2026-10-04).**

A short technical note on when a driven, open, disordered optical cavity can compute rather than merely project. It reduces the question to a measurable criterion on the second-order Volterra kernel of the input–output map, and lists the physical conditions that have to hold at the same operating point. Whether that operating point exists is the open problem the note is built around; nothing here claims it does.

The note is published as a single self-contained page: `index.html`.

## What the note argues

1. **The linearity constraint has a scope.** A linear cavity driven through its input field computes no nonlinear function of the input history, however high the rank of its map. That holds only when the data enter as the drive. When the data modulate the cavity's scattering potential, multiple scattering yields a nonlinear map from data to output with linear optics (structural nonlinearity).
2. **The criterion is a kernel, with the port declared.** Nonlinearity in the evolution shows up as a nonvanishing second-order kernel, sourced inside the cavity, with support on the photon-lifetime scale. The criterion must say where the input enters.
3. **Six conditions must coexist:** nonlinearity in the recurrence, dimensionality, memory matched to the drive, modal individuality, readout above the noise floor, and consistency (same input history, same output). They are coupled through one complex spectrum, so improving one tends to cost another.

## Revision history

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

1. Read You, Arai and Sunada (*Opt. Express* 33, 24982, 2025), the one located lead that may combine structural nonlinearity with optical memory.
2. Find a source for Petermann-factor statistics in chaotic open cavities before making any claim about how they scale with modal overlap.
3. Check whether the structural-reservoir comparison in Venâncio et al. (arXiv:2609.02733) isolates the second modulator pass from its other hardware differences.
4. The noise argument rests on sensing results; a direct result for reservoir readout near a bifurcation is still needed.
5. Han et al. (*Laser Photonics Rev.* e03155) is in early view; recheck volume and issue before any archival version.

## Verification

All 15 references passed the DOI gate before deployment: each DOI or arXiv identifier was resolved and matched to its claimed title and authors. The note lists the source of each check under the reference itself (publisher page, PMC record, arXiv record, full text, or author-resolved DOI). One reference (You et al.) is verified as a citation but not yet read, and the note says so where it is used.

Checks were cross-run across several AI instruments and treated as readings, not authorities. Where instruments disagreed (one reported the DOI for Parto et al. as invalid), the disagreement was settled against the primary record (PMC13588183), not by majority.

## Before pushing to GitHub Pages

- [ ] Every font named in CSS is loaded (IBM Plex Sans, Serif and Mono via Google Fonts, with system fallbacks).
- [ ] Body text at least 1rem; smallest utility text at least 0.72rem.
- [ ] No `-webkit-font-smoothing: antialiased` on dark backgrounds.
- [ ] MathJax renders all equations, including (5a) and (8a).
- [ ] Opened on a real phone in light and dark modes.

## License

CC0 1.0 Universal. No rights reserved.
