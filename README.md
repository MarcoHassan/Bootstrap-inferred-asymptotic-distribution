# R-bootstrapping-inferred-asymptotic-distribution
Bootstrapped inferred asymptotic distribution for instrumental variables regressions

Author: Marco Hassan

This work was completed as a final assignment for the Econometrics II Master level course at the University of St. Gallen.

Literature: 
Daron, A., Simon, J., & James, R. A. (2001, 12). The Colonial Origins of Comparative Development: An Empirical Investigation. The American Economic Review, 91, pp. 1369-1401. Retrieved from http://www.jstor.org/stable/2677930?origin=JSTOR-pdf

Nelson, C.R., Startz, R., 1990. Some further results on the exact small sample properties of the instrumental variable estimator. Econometrica 58, 967–976.

Stock, J.H., Wright, J.H., Yogo, M., 2002. A survey of weak instruments and weak identification in generalized method of moments. Journal of Business & Economics Statistics 20, 518–529.


# Idea

This study studies the famous paper "The Colonial Origins of Comparative Development: An Empirical Investigation" of Acemoglu, Johnson and Robinson.

Albeit the paper has been criticized on the more foundamental theoretical level critizing the validity of the dataset and the instrumental variable used this study addressed more formally the validity of relying on theoretical asymptotic distribution for Hypothesis tesiting in the case of a restricted dataset of around 80 observations in the case of the IV regression.

This test is important, especially given Nelson and Startz (1990), which found the asymptotic distribution of the IV estimator to be a very poor approximation to the finite sample distribution in the presence of weak instruments with the consequence that the t-test and Wald-test poorly perform for hypothesis testing.

To check these issues in Acemoglu et all. (2001), we continue by stressing the asymptotic results reported in section 2 by further analyzing the bootstrap results.
We make use of the resampling cases bootstrap which only assumes i.i.d. data observations. This involves taking the sample dataset as the population set, doing a sampling with replacement of the sample and inferring the parameter distribution of the resampled dataset. Under the assumption that the population parameters report an analogous distribution as the resampled one it is then possible to have a non-parametric estimation for the distribution, for the bias of asymptotic estimators and for the confidence intervals under Ho.

It turns out that if the normality assumption of the simple OLS estimators is satisfied as by the general theoretical framework accepting Null-hypothesis on the IV regression based on asymptotic distribution such as the Wald test seems an unjustified and dangerous approach.

# Well behaved bootstrapped distribution of OLS
![image](https://user-images.githubusercontent.com/42472072/52466805-2eacc080-2b8c-11e9-8dbd-591b048acb5a.png)

# Bootstrapped distribution of IV estimator

For botha a two step least square estimation as well as a generalized method of moments estimation the underlying asymptotic distribution is not justified.

![image](https://user-images.githubusercontent.com/42472072/52466921-7e8b8780-2b8c-11e9-93d9-9248d46205fe.png)

# Single observation influence applying the Jackknife in GMM estimator
![image](https://user-images.githubusercontent.com/42472072/52446757-9127a180-2b37-11e9-93d3-6681a44581b2.png)
