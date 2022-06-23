---
layout: default
---

# Never mind the metrics---Visualising confusion matrix performance metric distributions
## by David Lovell, Dimity Miller, Jaiden Capra and Andrew Bradley
### Source code and interactive visualisations

**Full paper**: https://arxiv.org/abs/2206.02157


**TL;DR:** Uncertainty in classifier performance metrics can easily eclipse differences in classifier performance; rather than searching for the "best" performance metric, we should put more effort into gathering representative data.

There are strong incentives to build classification systems that demonstrate outstanding predictive performance on various datasets and benchmarks. We believe these incentives risk a narrow focus on models and on the performance metrics used to evaluate and compare them---resulting in a growing body of literature to evaluate and compare metrics. This paper strives for a more balanced perspective on classifier performance metrics by highlighting their distributions under different models of uncertainty and showing how this uncertainty can easily eclipse differences in the empirical performance of classifiers. We begin by emphasising the fundamentally discrete nature of empirical confusion matrices and show how binary matrices can be meaningfully represented in a three dimensional compositional lattice, whose cross-sections form the basis of the space of receiver operating characteristic (ROC) curves. We develop equations, animations and interactive visualisations of the contours of performance metrics within (and beyond) this ROC space, showing how some are affected by class imbalance. We provide interactive visualisations that show the discrete posterior predictive probability mass functions of true and false positive rates in ROC space, and how these relate to uncertainty in performance metrics such as Balanced Accuracy (BA) and the Matthews Correlation Coefficient (MCC). Our hope is that these insights and visualisations will raise greater awareness of the substantial uncertainty in performance metric estimates that can arise when classifiers are evaluated on empirical datasets and benchmarks, and that classification model performance claims should be tempered by this understanding.

**Keywords:** Confusion matrix, performance metric, class imbalance, beta-binomial distribution, ROC  
