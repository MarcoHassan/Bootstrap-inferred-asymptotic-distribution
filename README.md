# R-bootstrapping-inferred-asymptotic-distribution
Bootstrapped inferred asymptotic distribution for instrumental variables regressions

Author: Marco Hassan

This work was completed as a final assignment for the Econometrics II Master level course at the University of St. Gallen.

# Idea

This study studies the famous paper "The Colonial Origins of Comparative Development: An Empirical Investigation" of Acemoglu, Johnson and Robinson.

Albeit the paper has been criticized on the more foundamental theoretical level critizing the validity of the dataset and the instrumental variable used this study addressed more formally the validity of relying on theoretical asymptotic distribution for Hypothesis tesiting in the case of a restricted dataset of around 80 observations in the case of the IV regression.

It turns out that if the normality assumption of the simple OLS estimators is satisfied as by the general theoretical framework accepting Null-hypothesis on the IV regression based on asymptotic distribution such as the Wald test seems an unjustified and dangerous approach.

This is confirmed in the analysis of the paper where the distribution of the estimator based on 50000 generated bootstrapped values seems far than normal and displaying fat tails suggesting a few number of observation driving the results and leading to misleading results relying on asymptotic theory.

# Bootstrapped distribution of IV estimator
![image](https://user-images.githubusercontent.com/42472072/52446663-545baa80-2b37-11e9-9eba-a15ed05ccd18.png)

# Single observation influenced applying the Jackknife estimation on each of the bootstrapped estimation
![image](https://user-images.githubusercontent.com/42472072/52446757-9127a180-2b37-11e9-93d3-6681a44581b2.png)
