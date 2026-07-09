# Academic Research

Key academic papers that form the foundation of GEO as a discipline.

---

## GEO: Generative Engine Optimization (KDD 2024)

**Paper:** arXiv:2311.09735
**Authors:** Pranjal Aggarwal et al., Princeton University
**Venue:** ACM SIGKDD Conference on Knowledge Discovery and Data Mining, 2024

### Key Findings

- GEO strategies can improve AI citation visibility by **up to 40%**
- Introduced **GEO-bench**, a large-scale benchmark for evaluating GEO techniques
- Most effective single strategy: citing external sources (+27–115%)
- Second most effective: adding statistics (+33–40%)
- Third: expert quotations (+30–41%)

### Methodology

The authors created a simulated generative engine environment and tested various content optimization strategies against a control group. Strategies were evaluated on citation frequency — how often optimized content appeared in AI-generated responses.

**Link:** https://arxiv.org/abs/2311.09735

---

## AutoGEO: Automatic GEO (ICLR 2026)

**Paper:** arXiv:2510.11438
**Authors:** Carnegie Mellon University
**Venue:** International Conference on Learning Representations, 2026

### Key Findings

- Extended the 47 citation strategies from KDD 2024
- Developed automated optimization pipeline
- Demonstrated that machine-learned GEO strategies outperform manual approaches
- Showed that strategy effectiveness varies by platform (ChatGPT vs. Perplexity vs. Gemini)

### Significance

AutoGEO represents the shift from manual GEO guidelines to automated, platform-aware optimization.

**Link:** https://arxiv.org/abs/2510.11438

---

## UC Berkeley EMNLP 2024: Negative Signal Detection

**Venue:** Conference on Empirical Methods in Natural Language Processing, 2024

### Key Findings

- Identified 8 categories of negative signals that reduce AI citation priority
- Demonstrated that AI models consistently deprioritize content with excessive CTAs, thin content, and missing author signals
- Showed that these signals are evaluated by the AI engine, not just search crawlers

### Practical Application

This research formed the basis of the 8-signal negative detection system used in GEO auditing tools.

---

## How to Use This Research

| Paper | Best Use |
|-------|----------|
| KDD 2024 (Princeton) | Apply the 47 citation strategies ranked by impact |
| ICLR 2026 (CMU) | Understand platform-specific optimization |
| EMNLP 2024 (Berkeley) | Audit your content for negative signals |