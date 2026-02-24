# WinDrift++ Pro: An accurate and efficient detector for concept drift detection

**The code and datasets for this work will be available once the final paper is published.**

---

## 📄 Abstract

Accurate handling of concept drift is essential for maintaining stable and reliable learning systems operating on evolving data streams. In practice, distributional changes often affect multiple statistical properties simultaneously, such as mean, variance, and higher-order moments, leading to degraded predictive performance and unstable adaptation. Many existing drift detectors, particularly single-test and uniformly weighted ensembles, lack robustness under such complex shifts and may trigger unnecessary or delayed model updates.

This article presents *WinDrift++ Pro*, an adaptive and cost-sensitive drift regulation framework for governing learning adaptation under non-stationarity. Extending *WinDrift* and *WinDrift++*, the proposed method introduces a context-aware weighting mechanism that learns which statistical tests provide the most reliable evidence of distributional change for a given data context. A knowledge base derived from wavelet-transformed historical features is combined with a cost-sensitive random forest to dynamically weight five complementary distance measures: Kolmogorov–Smirnov, Kuiper, Cramér–von Mises, Anderson–Darling, and Earth Mover's Distance. This design explicitly accounts for asymmetric error costs, enabling learning systems to prioritise impactful drift while suppressing destabilising false adaptations.

Experiments on 30 synthetic and real-world data streams demonstrate that WinDrift++ Pro consistently improves learning stability, achieving higher classification accuracy, faster recovery after drift, and fewer unnecessary adaptations than ten state-of-the-art methods. Upon acceptance of this manuscript, the implementation and datasets will be released at this page: https://github.com/naureenaqvi/windriftpluspluspro

---

## 💡 Impact Statement

Reliable operation of machine learning systems in real-world streaming environments depends critically on their ability to detect concept drift accurately, early, and efficiently. In domains such as intelligent infrastructure, finance, cyber-security, healthcare monitoring, and large-scale Internet of Things (IoT) deployments, delayed or incorrect drift detection can be as harmful as missed change, leading to unnecessary retraining, wasted computational resources, degraded predictive accuracy, and unstable decision-making.

As data streams increasingly underpin smart cities and connected systems, learning models must operate under strict constraints, including limited memory, bounded computation, continuous operation, and highly non-stationary data. Existing drift detectors often struggle in such settings due to slow response, excessive false alarms, or impractical computational overhead.

This work addresses these challenges by enabling fast, low-delay drift detection while maintaining computational and memory efficiency. *WinDrift++ Pro* improves the practical viability of stream learning by combining high drift detection accuracy with efficient resource usage and adaptability across diverse drift types. By leveraging prior learning patterns through a lightweight knowledge base, the framework responds quickly to impactful change while suppressing unnecessary adaptations, resulting in more stable learning behaviour and higher classification accuracy when combined with downstream classifiers.

This research supports scalable trustworthy stream-learning systems for long-running applications such as urban sensing, smart transportation, environmental monitoring, and real-time decision services. Efficient drift handling without additional resource burden, together with the open release of code and datasets, provides a practical foundation for advancing concept drift handling in next-generation smart city and IoT systems.

---

## 💻 Code

Code and datasets will be made available upon acceptance of the manuscript.
