# Macro-Conditioned Diffusion Models for Financial Time Series

This project explores conditional diffusion models for complex, nonstationary time series, with a focus on financial markets as a primary application. The model operates in the wavelet (time–frequency) domain and is conditioned on macroeconomic and regime-level variables, enabling realistic generation of multiscale dynamics and controlled counterfactual scenarios.

Rather than optimizing for point prediction, the framework emphasizes generative fidelity: reproducing heavy-tailed distributions, volatility clustering, and regime-dependent behavior that characterize real-world time series. This approach is broadly applicable to domains where multiscale temporal structure and conditional dynamics are central concerns.

Main concepts:
- Continuous Wavelet Transform (CWT) for multiscale time–frequency representation
- Conditional diffusion (DDPM) models for structured time series generation
- Explicit macro-level and regime-based conditioning for controlled sampling
- Evaluation grounded in domain-specific statistical properties rather than forecasting accuracy
