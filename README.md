Repository Overview
This repository contains a collection of Bayesian analysis projects, covering topics such as:

Prior and posterior predictive distributions

Linear regression with prior/posterior analysis

Model comparison and assessment

Hierarchical modeling

Each project demonstrates practical implementations using R, Stan, and Bayesian libraries (rstan, bayesplot, loo), with a focus on interpretability, model evaluation, and real-world applications.

Projects Summary
1. Prior and Posterior Analysis
    File: Bayesian-Analysis - Prior-and-Posterior.qmd
    Description:
    
    Estimates exam pass rates for two teaching methods using Beta-Binomial models.
    
    Tests hypotheses (e.g., Is pass rate > 60%?) via credible intervals.
    
    Computes posterior predictive distributions and compares Method A vs. Method B.
    
    Key Result:
    
    Method B has a 97.7% probability of outperforming Method A.
    
    Techniques:
    
    Monte Carlo sampling for predictions.
    
    Stan for joint parameter estimation.

2. Bayesian Linear Regression
    File: Linear-Regression - Bayesian-Analysis.qmd
    Description:
    
    Analyzes the relationship between household income and food expenditure using Bayesian linear regression.
    
    Compares prior vs. posterior predictions and evaluates model fit using credible intervals.
    
    Key insights:
    
    Prior uncertainty was high, but posterior estimates became precise after incorporating data.
    
    Tested predictive performance for specific income values (e.g., 50€, 72€).
    
    Techniques:
    
    Stan for MCMC sampling.
    
    Visualization of posterior predictive intervals.

3. Model Comparison and Assessment
    File: Bayesian-Analysis - Model-Comparison-and-Assesment.qmd
    Description:
    
    Compares three models to predict wine alcohol content:
    
    Color intensity-only model (best fit).
    
    Magnesium-only model (weakest fit).
    
    Interaction model (minimal improvement).
    
    Uses LOO-CV and WAIC for model selection.
    
    Tests a Gamma-distributed alternative (comparable performance).
    
    Techniques:
    
    Posterior predictive checks (ppc_dens_overlay).
    
    Log-likelihood evaluation (loo).

4. Hierarchical Modeling
    File: Bayesian-Analysis - Hierarchical-Model.qmd
    Description:
    
    Models referendum voting data at three levels: national, regional, and constituency.
    
    Compares:
    
    Pooled model (underfits).
    
    Two-level hierarchical model (better fit).
    
    Three-level hierarchical model (best fit, validated by LOO-CV).
    
    Demonstrates partial pooling to handle group-level variability.
    
    Techniques:
    
    Stan for hierarchical structures.
    
    Posterior predictive checks (ppc_ribbon).

Technical Stack
- Languages: R, Stan.

- Libraries: rstan, bayesplot, loo, ggplot2.

Methods:

- MCMC sampling (NUTS).

- Posterior predictive checks.

- Cross-validation (LOO, WAIC).
