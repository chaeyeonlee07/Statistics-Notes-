# Statistics-Notes-

## 👓 Classes Updated 
- Linear Modeling

  ◻️ Lecture 21: Shrinkage Method Rasso Regression
  
    🟦 Summary: We can lower MSE by inducing bias while lowering variances. Two methods are Lasso and Ridge. Ridge is two squared norms on each beta coefficients. Larger lambda leads to smaller $\beta$, smaller variance of $\beta$, and more biased $\beta$. There is always some value of lambda such that the MSE of ridge estimator is lower than that of OLS, although such parameter $\lambda$ is unknown.
    
  ◻️ Lecture 22: Shrinkage Method Rasso Regression + GLM
  
    🟦 Summary: Compared to Ridge regression which fails to zero out any of the $\beta$, Lasso regression zeros out betas. Similar to Ridge, there is no analytic solution or clear inference direction. If $\vec{y}$ is no longer continuous, then we cannot just use the model $\vec{y} \sim N(x\vec{\beta}, \sigma_\epsilon^2\mathbb{1}_n)$ because the variance is no longer constant and errors are dichotomous for two different values of $\vec{y}$. Therefore, we need a GLM framework which allows $\vec{y}$ to follow different distributions. The steps are largely: 1) specifying the conditional distributions of $\vec{y_i}$ and 2) finding link functions that transforms E[ $\vec{y_i}$ | $\vec{x_i}^T$ ] into the range $(-\infty,\infty)$.
