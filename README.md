# From Brain Causality to Browser AI: Machine Learning & Neuroimaging at TReNDS

**Presenter:** Sergey Plis (TReNDS Center, Atlanta — Georgia State University, Georgia Tech, Emory University)

## Abstract

In this talk, I will give a visual, high-level tour of the research happening in my team at the TReNDS Center in Atlanta, where we tackle fundamental machine learning challenges inspired by, and directly applied to, neuroimaging.

A central theme of our work is understanding brain function through **Causal Learning** and **AI Interpretability**. On the causal side, we develop theory and algorithms to bridge the mismatch between fast neural causal timescales and slow measurement timescales (a critical bottleneck in fMRI and beyond). For interpretability, we pioneer **ArchInterp** (architected interpretability): constructing deep learning models that are interpretable to researchers by design rather than relying on post-hoc explanations.

Because neuroimaging data is sensitive and siloed, yet modern AI is data-hungry, we also build algorithms and infrastructure for **decentralized machine learning**, including our open platform [neuroflame.org](http://neuroflame.org/). These same privacy constraints inspired [Brainchop](https://neuroneural.net/brainchop-test/), where we design parameter-efficient, state-of-the-art 3D neuroimaging models that run entirely client-side in the web browser. Finally, time permitting, I will touch on our foundational work improving the parameter efficiency of modern AI architectures via **introspection and fixed-point computation**.

Whether you are interested in ML theory, privacy-preserving systems, or neuroimaging applications, I’d love to connect about potential collaborations and opportunities for students to join the team. This work is generously supported by the **NIH**, **NSF**, and **AMD Inc.**

---

## Highlighted Team Members & Papers

1. **Brain Causality** — **Sajad Abavisani** & **Kseniya Solovyeva** (with David Danks & Vince Calhoun)
   - Solovyeva, K., Danks, D., Abavisani, M., & Plis, S. (2023). *Causal learning through deliberate undersampling*. **CLeaR 2023**, PMLR 213:518–530.
   - Abavisani, M., Danks, D., & Plis, S. M. (2023). *GRACE-C: Generalized rate agnostic causal estimation via constraints*. **ICLR 2023**.
   - Abavisani, M., Solovyeva, K., Danks, D., Calhoun, V. D., & Plis, S. (2026). [*RnR: a meta-solver for causal discovery in undersampled time series data*](https://openreview.net/forum?id=f1Ye3BzygN). **NeurIPS 2026**.

2. **ArchInterp (Architected Interpretability)** — **Dr. Usman Mahmood** (Defended; Senior Scientist II at Sail Biomedicines, Boston, MA) & **Pavel Popov** (PhD Student)
   - Mahmood, U., Fu, Z., Ghosh, S., Calhoun, V., & Plis, S. (2022). *Through the looking glass: Deep interpretable dynamic directed connectivity in resting fMRI*. **NeuroImage**, 264:119737.
   - Mahmood, U., Fu, Z., Calhoun, V., & Plis, S. (2023). *Glacier: glass-box transformer for interpretable dynamic neuroimaging*. **IEEE ICASSP 2023**, pp. 1–5.
   - Popov, P., Mahmood, U., Fu, Z., Yang, C., Calhoun, V., & Plis, S. (2024). *A simple but tough-to-beat baseline for fMRI time-series classification*. **NeuroImage**, 303:120909.
   - Popov, P. et al. (2026). *DECIFRA: Deep Interpretability with Causal Functional Graphs in Neuroimaging*. **IEEE Transactions on Medical Imaging (TMI)**, 2026 (In Press).

3. **Decentralized ML & NeuroFLAME** — **Dr. Riyasat Ohib** (Defended; now at Google DeepMind) & **Bishal Thapaliya**
   - Thapaliya, B., Ohib, R., Geenjaar, E., Liu, J., Calhoun, V., & Plis, S. M. (2024). *Efficient federated learning for distributed neuroimaging data*. **Frontiers in Neuroinformatics**, 18, p.1430987.
   - Ohib, R., Thapaliya, B., Dziugaite, G. K., Liu, J., Calhoun, V. D., & Plis, S. (2026). [*SSFL: Discovering Sparse Unified Subnetworks at Initialization for Efficient Federated Learning*](https://arxiv.org/abs/2405.09037). **Transactions on Machine Learning Research (TMLR)**, Jan 2026.

4. **Brainchop (Client-Side Browser 3D Neuroimaging AI)** — **Armina Fani**, **Dr. Alex Fedorov**, & **Mike Doan**
   - Plis, S. M., Masoud, M., Hu, F., Hanayik, T., Ghosh, S. S., Drake, C., Newman-Norlund, R., & Rorden, C. (2024). *Brainchop: Providing an edge ecosystem for deployment of neuroimaging artificial intelligence models*. **Aperture Neuro**, 4:10-52294.
   - Fani, A. et al. *MindGrab: Robust Skull Stripping of Any Modality on Any Device*.

5. **Introspective & Fixed-Point Computation** — **Mrinal Mathur** (with Barak A. Pearlmutter)
   - Mathur, M., Pearlmutter, B. A., & Plis, S. M. (2025). [*MIND over Body: Adaptive Thinking using Dynamic Computation*](https://openreview.net/forum?id=EjJGND0m1x). **ICLR 2025 Oral (Top 1.8%)**.
   - Mathur, M., Pearlmutter, B. A., & Plis, S. (2026). [*Closing the Loop with Fixed-Point Self-Attention*](https://openreview.net/forum?id=IH0NcTKzaZ). **NeurIPS 2026**.
