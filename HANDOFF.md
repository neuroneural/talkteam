# talkteam handoff

Updated: 2026-10-20. This file records the user's requirements and completed work. The causal learning section now follows the user's numbered screenshots. The user explicitly chose to skip number 7 and retain the equivalence-class slide as a hidden backup.

## Project and working files

- Workspace: `/Users/splis/Documents/talks/atlanta`
- Presentation repository: `/Users/splis/Documents/talks/atlanta/talkteam`
- Main deck: `/Users/splis/Documents/talks/atlanta/talkteam/index.html`
- Git remote: `git@github.com:neuroneural/talkteam.git`
- This is an existing Reveal.js HTML presentation. Edit the native HTML/CSS and preserve the working deck rather than converting it to another format.
- Styling lives in the `<style>` block in `index.html`, `css/custom.css`, and `dist/theme/aml.css`. Favor narrowly scoped changes.
- `README.md` contains the abstract, research themes, and team/paper list.
- There are pre-existing uncommitted changes, including `README.md`, `index.html`, and `figures/FPSA.png`. Preserve them. The user has now requested committing and pushing all recent presentation changes. Check Git for the authoritative commit/push state.
- A preview server was started on `http://127.0.0.1:8874/`, serving `talkteam`. It may need restarting in a later session. Use the actual working directory when serving.

## User's presentation goals and style

Title: **From Brain Causality to Browser AI: Machine Learning & Neuroimaging at TReNDS**.

A visual, high-level, 30-minute tour showcasing the strength of Sergey Plis's team at TReNDS in Atlanta. Cover problem motivation/setup and selected results. Keep derivations and algorithm details limited to what helps the intuition. The full talk spans brain causality, architected interpretability (ArchInterp), decentralized ML/neuroFLAME, browser neuroimaging AI/Brainchop, and time permitting introspection and fixed-point computation.

Figure legibility is a priority: the user explicitly objects to small, illegible figures surrounded by unused slide space. Fill available space before accepting small figure labels. On GRACE-C, the results row now uses unequal columns matched to the portrait-shaped solver comparison and landscape SCC figure. The SCC figure is larger and both figure headings align at the top. This change is scoped under `#grace-c .grace-results` and preserves both source SVGs.

Follow the user's existing slide style closely: warm cream background, condensed uppercase headings, muted blue-gray body text, restrained teal/green highlights, large research figures, team portraits next to the relevant papers, small paper citations, and existing corner logos. Avoid slogans, cliches, generic promotional copy, and unnecessary redesigns.

The user gives concrete visual instructions through pasted screenshots with handwritten numbers. Interpret the numbers together with the user's explanation: they may specify slide order or fragment order within a slide. The marks are instructions for arrangement/reveals, not artwork to reproduce. Follow the order supplied by the user. Ask a focused question only if a consequential ambiguity remains after reading the screenshots and accompanying text.

Preserve accurate labels, measurements, and citations. Prefer source figures and native vector artwork when available. Transparent figure backgrounds are strongly preferred when they integrate the figure into the cream slide. Visually center the actual content group, accounting for whitespace inside assets.

## Completed: causal learning section

Implemented the user's annotated screenshot order in the existing Reveal.js deck. The labels below are the user's narrative numbers, not Reveal's numeric slide hashes. Stable slide IDs are available for previews.

Primary source:

- `/Users/splis/Documents/talks/atlanta/causaltalk/index.html`
- `/Users/splis/Documents/talks/atlanta/causaltalk/figures/`
- Source repository: `https://github.com/neuroneural/causaltalk`

The current destination section is the second horizontal Reveal stack in `talkteam/index.html`, between the comments `COLUMN 2: THEME 1` and `COLUMN 3: THEME 2`. Locate it by text, because line numbers change.

Current visible order, after the Brain Causality section title:

1. Causal ≠ Measurement Timescale (`#/causal-timescales`)
2. Representation (`#/causal-representation`)
3. Undersampling Effect (`#/undersampling-effect`)
4. Compressed Graph (`#/compressed-graph`)
5. Simple Loops (`#/simple-loops`)
6. Search Tree (`#/causal-search-tree`)
8. Search pruning/runtime results (`#/causal-search-runtime`)
9. Answer Set Programming (`#/answer-set-programming`)
10. MSL/SAT results (`#/asp-results`)
11. GRACE-C: approximately 100 Variables (`#/grace-c`)
12. Deliberate Undersampling (`#/deliberate-undersampling`)

The two existing RnR slides follow this sequence (`#/rnr-pipeline`, `#/rnr-recovery`). The equivalence-class/theorem slide is retained in the source as `id="undersampling-equivalence-backup" data-visibility="hidden"`, excluded from normal presentation navigation. The user explicitly selected this treatment when asked about the missing screenshot 7.

Imported the original `simple_loops.png`, `edge_merging_tree.png`, `runtime_demo.png`, `clingo.png`, and `ASP.png` from `causaltalk/figures/`. The DBN and compressed graph figures were already present and matched the source exactly. All new paths are repository-relative.

Deliberate Undersampling now has two cumulative fragments: the equivalence-class illustration above (`data-fragment-index="0"`), then the numerical heatmap below (`data-fragment-index="1"`). The original `du_gain.png` remains untouched. A CSS viewport clips its redundant paper caption while retaining the formula, axes, labels and colour bars. Kseniya's first-author credit, Sajad's portrait and the full paper citation remain. New layout styles are scoped to causal slides. Citation positioning was corrected on the effect, GRACE-C and RnR slides so their existing citations remain visible.

Browser inspection covered the requested slides and both deliberate-undersampling reveals. Original figures were preserved, assets resolved, and `git diff --check` passed. A byte comparison confirmed that all slides and scripts after the causal section, including FPSA, and all earlier slide markup and prior styles were unchanged. The user subsequently requested that all recent changes be committed and pushed.

Existing assets include `neuron.png`, `brainnet.png`, `fmri.png`, `undersamplingDBN.png`, `changes_on_undersampling_ICLR.svg`, `eq_class_G4_ICLR.svg`, `RASLvsRASL.svg`, `100nodeSCC.svg`, `rnr.png`, `rnr_value_add.svg`, `salience.png`, `venn_diagrams.svg`, and `du_gain.png` in `talkteam/figures/`.

Highlight **Sajad Abavisani** (Mohammadsajad Abavisani) and these papers, preserving correct author credit:

- Solovyeva, K., Danks, D., Abavisani, M., & Plis, S. (2023). *Causal learning through deliberate undersampling*. CLeaR 2023, PMLR 213:518–530. First author Kseniya Solovyeva. `https://proceedings.mlr.press/v213/solovyeva23a.html`
- Abavisani, M., Danks, D., & Plis, S. M. (2023). *GRACE-C: Generalized rate agnostic causal estimation via constraints*. ICLR 2023.
- Abavisani, M., Solovyeva, K., Danks, D., Calhoun, V. D., & Plis, S. (2026). *RnR: a meta-solver for causal discovery in undersampled time series data*. NeurIPS 2026 poster, as supplied by the user. `https://openreview.net/forum?id=f1Ye3BzygN`

Portraits already used: `figures/Sajad.jpeg`, `figures/Xenia.jpeg` (Kseniya Solovyeva), and `figures/DavidDanks.jpeg`. Preserve the association between people and papers. Existing slide assertions are not a substitute for checking source material when changing a technical claim.

Copy any newly used assets into `talkteam` and use repository-relative paths, so the destination deck remains portable. Preserve any needed animation or interaction from source slides. Do not modify unrelated sections just to accommodate the causal section.

## Latest refinement: larger undersampling illustration and published MeanMLP comparison

- Deliberate Undersampling retains two cumulative fragments. The first gives the upper illustration almost the full central slide width. On the second reveal it reduces to a 280px-high overview above the heatmap, still substantially larger than the earlier 190px version. Rewinding restores the enlarged first reveal. The heatmap keeps its previous width, axes, labels and colour bars. Its formula is retained in speaker notes, and the formula and redundant paper caption are clipped from the display to make room.
- The MeanMLP slide (`#/arch-slide`) is titled **A Simple Baseline for fMRI Classification**. It displays the original published comparison at full central width, with Pavel's portrait and the NeuroImage citation preserved. The previous aggregate 13-architecture chart, its reconstructed D3 renderer, and its summary claims were removed.
- The comparison comes from the user-supplied `/Users/splis/Documents/proposals/DoD/PRE-EMPT/figures/general_comparison_fin.svgz`. The portable deck asset is `figures/general_comparison_fin.svg`. It is the decompressed source with only its six white background fills changed to `none`. Preserve the vector artwork and transparent background.
- Both MeanMLP and the two undersampling reveals were visually inspected in a browser. Keep prioritizing large, readable research figures over unused slide space.

## Completed in this chat: fixed-point self-attention slide

Slide: `id="fixed-point-self-attention"`, class `self-slide`, reachable at `#/fixed-point-self-attention` (formerly numeric `#/5/4`).

The user approved the following direction:

- Three cumulative fragments, in order: mechanism diagram, benchmark tables together, bottom result together. Implemented with `data-fragment-index="0"`, `"1"`, and `"2"`.
- A new bottom result uses the supplied paper's Figure 4c: accuracy gain versus test-time iteration budget for 29M, 110M, and 340M models, with a short interpretation of saturation around 8–16 steps.
- **Use FPSA (fixed-point self-attention) in slide labels, not +SELF.** The rows are now `ViT-B/16 + FPSA` and `BERT-Base + FPSA`. The figure uses FPSA-LH for the learned-halting variant.
- Benchmark values were reconciled with the attached paper. The erroneous COCO mAP column was removed. Speaker notes document the source locations and naming differences in the manuscript.
- A small compute note clarifies that fixed parameter count does not mean unchanged computation.
- The bottom plot now uses **`figures/FPSA_compute_scaling.svg`**, extracted from the PDF's native vector artwork with the white background paths excluded. Curves and labels were preserved. No generated reconstruction of the data was used.
- The previous PNG, `figures/FPSA_compute_scaling.png`, remains but is no longer referenced by the slide.
- The bottom row has `margin-left: 100px` to center its visible content better. Styling changes are scoped under `.self-slide`.
- The citation footer on this slide was positioned so it remains visible.
- The three reveal steps were verified in a browser, and the final transparent plot/positioning was visually checked. `git diff --check` passed.

Supplied paper, if still available: `/private/tmp/29071_Closing_the_Loop_with_Fi.pdf`. Temporary preview: `/private/tmp/FPSA-slide-preview-centered.png`. Temporary files may not persist, so the working deck and repository SVG are the authoritative result.

## Other original source decks and people

These are context for the overall presentation, not a request to edit them in the next task:

- Brainchop: local `talkbrainchop`, `https://github.com/neuroneural/talkbrainchop`; highlight Armina Fani.
- Interpretability: local `talkinterp`, `https://github.com/neuroneural/talkinterp`; Usman Mahmood (defended, Senior Scientist II at Sail Biomedicines in Boston) and Pavel Popov (PhD student). Usman's NeuroImage/ICASSP papers, Pavel's MeanMLP NeuroImage and accepted IEEE TMI paper.
- Federated/neuroFLAME: local `decentralized_OHBM`, `https://github.com/neuroneural/decentralized_OHBM`; Riyasat Ohib (now Google DeepMind), SSFL (TMLR 2026) and the 2024 Frontiers in Neuroinformatics paper with Bishal Thapaliya.
- Fixed-point/introspection: Mrinal Mathur, *MIND over Body* (ICLR 2025 Oral) and *Closing the Loop with Fixed-Point Self-Attention* (NeurIPS 2026 poster, user-supplied status). Course source: `https://neuroneural.net/fixedpointcourse/lecture4.html`.
- Team photos also exist under `/Users/splis/Documents/talks/atlanta/newreveal/figures/`.
- Acknowledge NIH, NSF, and AMD Inc. Support collaboration and student recruitment goals without promotional slogans.

## Working approach for the next agent

Read this file and relevant source slides, then follow any further user screenshots and narration. The numbered rearrangement described above is already implemented. Make the authorized changes directly in the existing deck. Preserve all unrelated work. Preview changed slides in a browser, check the fragment sequence where relevant, verify figures/citations/text fit, and provide a concise result with a usable preview. Do not claim that local changes are on GitHub unless they have actually been pushed. This handoff does not authorize creating a new chat or messaging other chats.
