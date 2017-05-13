# About

MBE is a script that implements the mode-based estimate (MBE) for Mendelian randomization. This is proposed to obtain a single causal effect estimate from multiple genetic instruments.

# Usage

```MBE(BetaXG, BetaYG, seBetaXG, seBetaYG, phi=c(1,0.5,0.25), n_boot=1e4, alpha=0.05)```

Where:

- BetaXG: vector of instrument-exposure regression coefficients
- BetaYG: vector of instrument-outcome regression coefficients
- seBetaXG: vector of instrument-exposure standard errors (SEs)
- seBetaYG: vector of instrument-outcome SEs
- phi: tunning parameter (e.g., 1=default bandwidth; 0.5=half of the default bandwidth)
- n_boot: number of bootstrap iterations
- alpha: alpha level of the confidence intervals (e.g., alpha=0.05 corresponds to 1-0.05=95% confidence intervals)

# Citation 

Hartwig FP, Davey Smith G and Bowden J. Robust inference in summary data Mendelian randomisation via the zero modal pleiotropy assumption. bioRxiv 2017 https://doi.org/10.1101/126102
