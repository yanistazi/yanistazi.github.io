---
permalink: /software/
title: "Software & Code"
excerpt: "Software & Code"
author_profile: true
---

## Software
- [bayesbridge v0.2](https://github.com/OHDSI/bayes-bridge)&nbsp; (with [documentation](https://bayes-bridge.readthedocs.io/en/latest/))
  <br> Python package for Bayesian sparse regression based on the Bayesian bridge priors. The package implements the standard (Polya-Gamma augmented) Gibbs sampler as well as the CG-accelerated sampler of [Nishimura & Suchard (2022)](https://doi.org/10.1080/01621459.2022.2057859).

- [CausalSurvival](https://github.com/nishimura-zeger-lab/CausalSurvival) <br>
  R package implementing state-of-the-art doubly robust methods for estimating counterfactual survival curves, including augmented inverse probability weighting and targeted maximum likelihood estimation. More traditional procedures such as inverse probability weighting and stratified Cox model are also included.

## Code
- [Hoseshoe scale sampler](https://github.com/aki-nishimura/horseshoe-scale-sampler) <br>
  Efficient rejection sampler for updating the local scale parameter in Gibbs sampling posterior distributions under (regularized) horseshoe models. Details and theoretical analysis can be found in the appendix of [Nishimura and Suchard (2022)](https://doi.org/10.1214/22-BA1308).

- [Discontinuous Hamiltonian Monte Carlo](https://github.com/aki-nishimura/discontinuous-hmc)
  <br> Python module implementing discontinuous Hamiltonian Monte Carlo of [Nishimura et. al. (2022)](https://doi.org/10.1093/biomet/asz083). Other codes used in the paper are also provided, including the modules to efficiently compute the log-likelihoods and their gradients of the Jolly-Seber and PAC Bayesian inference.

- [Probabilistic importance weighted matrix factorization](https://github.com/aki-nishimura/probabilistic-matrix-factorization)
  <br> Python module for the Bayesian heteroscedastic matrix factorization model as described in [Yang et. al. (2017)](https://www.researchgate.net/publication/320883956_Bayesian_Heteroscedastic_Matrix_Factorization_for_Conversion_Rate_Prediction).

- [(Recycled) No-U-Turn sampler](https://github.com/aki-nishimura/NUTS-matlab)
  <br> Matlab functions for the No-U-Turn sampler of [Hoffman & Gelman (2014)](http://www.jmlr.org/papers/volume15/hoffman14a/hoffman14a.pdf) as well as its improvement via the recycling algorithm of [Nishimura & Dunson (2016)](https://arxiv.org/abs/1511.06925).
