---
layout: page
title: "Forecasting mortality with SVD factor decomposition"
eyebrow: "time series · svd"
permalink: /projects/svd-mortality/
---

*A Lee-Carter-style mortality forecast built with SVD factor decomposition
and an ARIMA-modeled time index, applied to CDC WONDER mortality data.*

[View the code on GitHub](https://github.com/signal-within-noise/svd-opioid-mortality)

## Overview

<!-- Method first, dataset second -- e.g. "This project decomposes an
age-by-year log-mortality surface into latent factors via SVD, forecasts
the dominant time-varying factor with ARIMA, and reconstructs a one-step-
ahead mortality forecast. Applied here to U.S. opioid mortality data as a
test case." -->

## Method

<!-- Short technical walkthrough: log-linked rates, SVD decomposition,
normalization of b_x/k_t, ARIMA(0,1,0) random-walk-with-drift forecast. -->

## Results

![Observed vs. predicted 2019 mortality by age group](/assets/images/observed_vs_predicted.png)

<!-- One or two sentences of interpretation under each chart. -->

![Aggregate mortality trend, 2010-2019](/assets/images/agg_mort.png)

![SVD reconstruction by principal component](/assets/images/svd_reconst_mort.png)

## Validation

<!-- MAE/RMSE numbers from main.py go here. -->
