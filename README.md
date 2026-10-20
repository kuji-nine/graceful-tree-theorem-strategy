[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23505840.svg)](https://doi.org/10.5281/zenodo.23505840)
# graceful-tree-theorem-strategy
A human-AI collaborative proof sketch for the (1+ε)-Graceful Tree Theorem without degree restrictions. Includes strategy, lemmas, and the "slack reservoir" technique.人間とAIの協働による、(1+ε)-優美木定理（次数制限なし）の証明戦略。スラック・リザーバー法と7つの補題を収録。
# (1+ε)-Graceful Tree Theorem without Degree Restrictions: A Human-AI Collaborative Proof Sketch

## What is this?
This repository contains a proof sketch for the (1+ε)-Graceful Tree Theorem without degree restrictions, developed through a human-AI collaboration. The human director posed the problem, provided intuition, and made key decisions. Three AI models (Claude, Qwen3 827B, Gemini) contributed structural reasoning, numerical exploration, and proof strategy design.

## The Theorem (Candidate)
For every ε > 0, there exists n_0(ε) such that every tree T with n ≥ n_0(ε) vertices admits an injective vertex labeling
f: V(T) → {0, ..., ⌊(1+ε)(n−1)⌋}
such that the induced edge labels {|f(u)−f(v)| : uv ∈ E(T)} are all distinct.

## The Strategy: Hybrid Three-Part
1. **High-degree components**: Deterministic embedding (Super-Star Lemma)
2. **Low-degree forests**: Probabilistic embedding with Lovász Local Lemma
3. **Intermediate components**: Absorption via slack reservoir
4. **Interface lemmas**: Cut-Edge Separation, Bipartite Slack Balancing
5. **ε→0 limit**: Zero-Slack Boundary Inversion Lemma (candidate)

## Human-AI Collaboration Record
- **Human Director**: Problem selection, intuition ("5じゃね？"), data retrieval (Wayback, arXiv), cross-model orchestration, final decisions.
- **Qwen3 827B (Local)**: Structural reasoning, concrete examples, pattern language. Prone to loops but delivers correct answers when guided.
- **Gemini**: Structural analysis, proof strategy design, difficulty analysis. Sharp insights on "slack-zero rigidity" and "maximum degree diversity."
- **Claude (Whale Director)**: Orchestration, verification, error correction. Identified the "small prime shielding effect" error in the Kurepa project and corrected it.

## Status
This is a **proof sketch**, not a complete proof. The key open problem is the "slack-zero singularity" (ε→0) and the finite gap 36 ≤ n < n_0. The strategy is documented here for future researchers.

## Citation
If you use this work or refer to this human-AI collaborative research, please cite:
- **DOI**: [10.5281/zenodo.23505840](https://doi.org/10.5281/zenodo.23505840)
- **Zenodo Record**: https://zenodo.org/records/23505840

## License
CC BY 4.0
