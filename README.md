{\rtf1\ansi\ansicpg1252\cocoartf2865
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Macro-Conditioned Diffusion Models for Financial Time Series\
\
This project explores conditional diffusion models for complex, nonstationary time series, with a focus on financial markets as a primary application. The model operates in the wavelet (time\'96frequency) domain and is conditioned on macroeconomic and regime-level variables, enabling realistic generation of multiscale dynamics and controlled counterfactual scenarios.\
\
Rather than optimizing for point prediction, the framework emphasizes generative fidelity: reproducing heavy-tailed distributions, volatility clustering, and regime-dependent behavior that characterize real-world time series. This approach is broadly applicable to domains where multiscale temporal structure and conditional dynamics are central concerns.\
\
Main concepts:\
- Continuous Wavelet Transform (CWT) for multiscale time\'96frequency representation\
- Conditional diffusion (DDPM) models for structured time series generation\
- Explicit macro-level and regime-based conditioning for controlled sampling\
- Evaluation grounded in domain-specific statistical properties rather than forecasting accuracy\
}