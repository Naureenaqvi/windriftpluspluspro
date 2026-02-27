# WinDrift++ Pro: An accurate and efficient detector for concept drift detection

**The code and datasets for this work will be available once the final paper is published.**

---

## 📄 Abstract

Modern machine learning systems deployed on data streams must operate reliably under continual change. In real-world settings, distributional shifts rarely affect a single statistical property in isolation; instead, changes often occur simultaneously across mean, variance, shape, and tail behaviour. These complex shifts can destabilise learning, leading to delayed responses, unnecessary retraining, or degraded predictive performance. Many existing drift detectors struggle in such scenarios due to rigid statistical assumptions or uniformly weighted decision mechanisms.

WinDrift++ Pro is an adaptive, cost-aware framework designed to regulate learning behaviour under non-stationary data streams. Building on earlier WinDrift variants, the framework learns which statistical signals are most informative for a given context rather than treating all drift evidence equally. It combines historical distributional patterns, extracted via wavelet-based features, with a lightweight cost-sensitive ensemble to dynamically weight multiple complementary distance measures. This enables the system to emphasise impactful changes while suppressing spurious or low-risk fluctuations.

The framework is designed with practical streaming constraints in mind, supporting stable adaptation, low computational overhead, and asymmetric error costs. Across a diverse collection of synthetic and real-world data streams, WinDrift++ Pro demonstrates improved learning stability, faster recovery from change, and reduced unnecessary adaptations when compared with existing drift detection approaches.

This repository will host the reference implementation and experimental assets associated with the WinDrift++ Pro framework.

Upon acceptance of this manuscript, the implementation and datasets will be released at this page: https://github.com/naureenaqvi/windriftpluspluspro

---

## 💻 Code

Code and datasets will be made available upon acceptance of the manuscript.
