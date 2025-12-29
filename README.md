# Macro-Conditioned Diffusion Models for Financial Time Series

This project explores conditional diffusion models for complex, nonstationary time series, with a focus on financial markets as a primary application. The core contribution is a diffusion-based generative framework operating in the wavelet (time–frequency) domain and explicitly conditioned on macroeconomic and regime-level variables.

Instead of optimizing for point prediction, this work emphasizes generative realism: reproducing the statistical and temporal properties that characterize real financial data, including heavy tails, volatility clustering, and regime-dependent dynamics.

# Motivation

Financial return series exhibit a small number of persistent stylized facts that are notoriously difficult to reproduce jointly:
- Heavy-tailed marginal distributions
- Volatility clustering across multiple horizons
- Strong dependence on macroeconomic regimes

Classical econometric models capture subsets of these properties but rely on restrictive parametric assumptions. Modern deep generative models often struggle with training instability, tail behavior, or multiscale temporal structure.

This project investigates whether combining **multiscale wavelet representations** with **conditional diffusion models** can yield a stable, interpretable, and controllable generative framework for time series simulation.

# Core Ideas

Key concepts implemented in this project:

- Continuous Wavelet Transform (CWT) to represent time series in the time–frequency domain
- Conditional Denoising Diffusion Probabilistic Models (DDPMs) operating on wavelet coefficients
- Explicit macroeconomic and regime conditioning injected into the reverse diffusion process
- Evaluation grounded in empirically established stylized facts rather than forecasting accuracy

# What this project does

- Reproduces heavy-tailed return distributions and extreme quantiles
- Captures volatility clustering via persistent autocorrelation in squared returns
- Exhibits regime-dependent behavior under counterfactual conditioning with identical latent noise
- Generates multiscale volatility dynamics that differ across expansionary and crisis regimes

Scope and non-claims:

- This project does not aim to forecast future returns or volatility
- No claims of causal inference are made
- Tail index estimation and extreme value theory are outside the scope
- Conditioning variables are not interpreted as structural causal drivers

# Structure:
notebooks/
  Data preprocessing, wavelet transforms, model training, and evaluation

paper/
  Full academic write-up describing methodology, theory, and results

visuals/
  Figures and diagnostic plots used for analysis and presentation

# Potential applications include:
- Scenario generation and stress testing
- Regime-aware simulation of time series
- Synthetic data generation under macroeconomic conditions
- Research on multiscale generative modeling

