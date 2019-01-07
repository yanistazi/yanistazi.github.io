---
title: "Research"
permalink: /research/
author_profile: true
---

## Observational Health Data Sciences and Informatics (OHDSI)
[OHDSI](https://www.ohdsi.org/) is a public-private collaborative between the pharmaceutical industry, academia, and government. We have been building a network of standardized healthcare databases and open-source analytic tools to enable large-scale analytics of observational data. Our goals include improving our understandings of healthcare systems, generating reliable clinical evidences on drug safety, and developing precision treatment effect models.

<!-- For instance, a randomized control trial of a drug is typically conducted on a very specific subpopulation of a limited sample size, leaving many unknowns about the potential side effects as well as efficacies in other subpopulations. Our network of large-scale healthcare databases provide us opportunities to investigate these insufficiently-studied effects of drugs. -->

As a member of the OHDSI inference and prediction group, my role is to develop statistical methods and computational techniques to extract useful insights from complex large-scale observational data.

## Scalable Bayesian sparse regression: generalized linear models and survival analysis in "large n & large p" regime
Sparse regression is one of the most widely used methods in modern statistical learning as data sets continue to grow in size and complexity. Bayesian sparse regression is a noteworthy alternative to the conventional frequentist or penalty based approaches. For example, Bayesian approach provides a coherent framework to account for and exploit many characteristics commonly found in observational healthcare data: heterogeneity across databases, prior information from the existing literatures, etc.

Posterior inference under Bayesian sparse regression models, however, remains computationally infeasible for many large-scale data sets. For example in a modern observational study based on healthcare databases, the number of observations typically ranges in the order of **n = 10<sup>5</sup> ∼ 10<sup>6</sup>** and that of the predictors in the order of **p = 10<sup>4</sup> ∼ 10<sup>5</sup>**. Such data sets are beyond typical scales where (fully) Bayesian analysis have previously been applied. Moreover, many of the existing computational techniques are rather limited in scope (to the Gaussian likelihood model, for example).

Our *conjugate gradient (CG) accelerated sampler* [(Nishimura and Suchard, 2018)](https://arxiv.org/abs/1810.12437) is the first computational technique of its kind to address “large n & large p” Bayesian sparse regression for binomial outcomes. In a study comparing risks of intracranial hemorrhage from two alternative blood anti-coagulants (n = 72,489 with p = 22,175), our algorithm delivers **11-fold speed-up** in posterior computation, cutting the computational time from **77.4 to 7.04 hours**. We are currently developing techniques to deal with more general outcomes including survival time &mdash; the most common outcome type in healthcare data.
