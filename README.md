pengineered disorder. Such a map can be of arbitrarily high rank and still computes no nonlinear function of its input history — high dimensionality is necessary but nowhere near sufficient. Whether a driven, open, disordered cavity becomes a genuine computational substrate is therefore a question about three *coupled* physical observables — dimensionality, fading memory, and a nonlinearity internal to the field evolution — that all enter through the same complex spectrum of quasinormal modes.

## The criterion

Stripped of reservoir-computing vocabulary, the computation question is a statement about the **Volterra kernels** of the input–output map. A linear system has only a first-order kernel (its Green's function); nonlinearity in the state evolution appears as a nonvanishing higher-order kernel. The physically meaningful requirement is that the second-order kernel be **nonzero, sourced by the intracavity field-dependence rather than by the detector, and supported over the photon lifetime**:

$$h_2(\tau_1,\tau_2)\neq 0,\qquad \operatorname{supp} h_2 \sim \tau_{\text{photon}}.$$

The open question is whether a single operating point satisfies all of the following at once:

- **Nonlinearity in the recurrence** — $h_2\neq 0$, intracavity-sourced, with $\operatorname{supp} h_2 \sim \tau_{\text{photon}}$
- **Dimensionality** — effective rank $r_{\text{eff}}=\mathcal{O}(N_{\text{modes}})$
- **Memory matched to drive** — spread of decay rates $\{\gamma_m\}$ comparable to the symbol rate
- **Modal individuality** — Thouless parameter $\delta=\bar\gamma/\Delta\omega=\mathcal{O}(1)$

The difficulty is that these pull against one another through shared physics: disorder raises dimensionality but adds radiative loss (shortening memory, driving $\delta$ past unity), and a nonlinearity strong enough to register in $h_2$ — gain saturation near threshold, for example — tends to induce mode competition that collapses the field onto a few modes and sends $r_{\text{eff}}\to 1$. Whether the favorable region is nonempty is the whole problem.

## Contents

| File | What it is |
|------|------------|
| `cavity-coexistence-note.html` | The note itself — self-contained, equations rendered with MathJax, light/dark theme with an `AUTO / LIGHT / DARK` toggle |
| `README.md` | This file |

## Viewing

Open `cavity-coexistence-note.html` in any browser. Equations and fonts load from CDNs (MathJax, IBM Plex), so an internet connection is needed on first view.

To serve it via GitHub Pages, rename or copy the file to `index.html` (or add one that links to it) and enable Pages on the repository; it will then render at the project's Pages URL. The page reads the device's `prefers-color-scheme` automatically and exposes a manual override.

## Status

Pre-experimental. This is a framing of a physics problem and a falsifiable criterion, not a result. A clean negative — a demonstration that no operating point satisfies the four conditions simultaneously — would be just as useful as a positive one.

## License

[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — no rights reserved. The framing, the equations, and the criterion are placed in the public domain. Build on them freely, without permission, attribution, or contact.

## Note on authorship

This note was developed with substantial AI assistance and is published without personal attribution, by design. The contribution is the framing: naming the deciding question, reducing it to a measurable kernel criterion, and scoping honestly what is established versus open.
