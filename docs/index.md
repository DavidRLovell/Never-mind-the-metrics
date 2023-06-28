---
layout: default
---

# Never mind the metrics---Visualising binary confusion matrix performance metric distributions to put performance in perspective
## by David Lovell, Dimity Miller, Jaiden Capra and Andrew Bradley
### Source code and interactive visualisations at  
[davidrlovell.github.io/Never-mind-the-metrics](https://davidrlovell.github.io/Never-mind-the-metrics/)

**Paper to appear**: in ICML23  
**Preprint**: [https://arxiv.org/abs/2206.02157](https://arxiv.org/abs/2206.02157)

**TL;DR:** Uncertainty in classifier performance metrics can easily eclipse differences in classifier performance; rather than searching for the "best" performance metric, we should put more effort into gathering representative data.

**Abstract:** There are strong incentives to build classification systems that demonstrate outstanding predictive performance on various datasets and benchmarks. We believe these incentives risk a narrow focus on models and on the performance metrics used to evaluate and compare them---resulting in a growing body of literature to evaluate and compare _metrics_. This paper strives for a more balanced perspective on classifier performance metrics by highlighting their distributions under different models of uncertainty and showing how this uncertainty can easily eclipse differences in the empirical performance of classifiers. We begin by emphasising the fundamentally discrete nature of empirical confusion matrices and show how binary matrices can be meaningfully represented in a three dimensional compositional lattice, whose cross-sections form the basis of the space of receiver operating characteristic (ROC) curves. We develop equations, animations and interactive visualisations of the contours of performance metrics within (and beyond) this ROC space, showing how some are affected by class imbalance. We provide interactive visualisations that show the discrete posterior predictive probability mass functions of true and false positive rates in ROC space, and how these relate to uncertainty in performance metrics such as Balanced Accuracy (BA) and the Matthews Correlation Coefficient (MCC). Our hope is that these insights and visualisations will raise greater awareness of the substantial uncertainty in performance metric estimates that can arise when classifiers are evaluated on empirical datasets and benchmarks, and that classification model performance claims should be tempered by this understanding.

**Keywords:** Confusion matrix, performance metric, class imbalance, beta-binomial distribution, ROC  

## Links to figures and interactive visualisations

* **All possible ROC and Precision-Recall reference points**   [http://bit.ly/see-ROC-reference-points](http://bit.ly/see-ROC-reference-points) shows all possible points in ROC and Precision-Recall spaces corresponding to confusion matrices of a given size, coloured by Balanced Accuracy. 
* **Confusion matrix performance metric contours**  
[http://bit.ly/see-confusion-metrics](http://bit.ly/see-confusion-metrics) enables us to interactively visualise a range of confusion matrix performance metrics by plotting their contours, coloured from red (low) to white (middle) to blue (high). 
* **Uncertainty in confusion matrices and their performance metrics**  
[http://bit.ly/see-confusion-uncertainty](http://bit.ly/see-confusion-uncertainty) enables interactive exploration of the posterior predictive pmfs of confusion matrices and three performance metrics (MCC, BA, F1) under binomial and beta-binomial models of uncertainty. 
* **Interactive confusion simplex**  
[http://bit.ly/see-confusion-simplex](http://bit.ly/see-confusion-simplex) shows an interactive visualisation of the 3D projection of binary confusion matrices of size 100. Each point corresponds to a unique confusion matrix and is coloured by the value of that matrix's Matthews Correlation Coefficient.
* **Animated performance metric contours**  
These animated plots show how the contours of various performance metrics change with class balance, i.e., as the number of negative examples and positive examples vary in confusion matrices of fixed size. We have created animations of
  * Accuracy:                             [https://bit.ly/see-animated-accuracy](https://bit.ly/see-animated-accuracy)
  * Balanced Accuracy:                    [https://bit.ly/see-animated-BA](https://bit.ly/see-animated-BA)
  * F1 Score:                             [https://bit.ly/see-animated-F1](https://bit.ly/see-animated-F1)
  * Matthews Correlation Coefficient:     [https://bit.ly/see-animated-MCC](https://bit.ly/see-animated-MCC)
* [All figures in the manuscript](https://davidrlovell.github.io/Never-mind-the-metrics/AllFigures.html):  
This document provides the RMarkdown behind the figures and interactive visualisations in our paper for anyone who wants to see how they were created or who wishes to extend them.
  * Source code (Rmarkdown) is available from Github at   [https://github.com/DavidRLovell/Never-mind-the-metrics](https://github.com/DavidRLovell/Never-mind-the-metrics)