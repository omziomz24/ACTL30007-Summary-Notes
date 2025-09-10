# ACTL30007: Actuarial Modelling III - Comprehensive Summary Notes

This repository contains my comprehensive summary notes for the subject **ACTL30007: Actuarial Modelling III**, completed at the University of Melbourne. These notes are designed to provide a structured and detailed breakdown of all key topics covered in the course, with a focus on both theoretical concepts and practical applications using the R programming language.

The notes were compiled to be a single, all-encompassing resource for revision and reference. They are formatted in LaTeX for clear presentation of mathematical and statistical notation.

## Subject Breakdown

The course, Actuarial Modelling III, provides an in-depth look at advanced stochastic modelling techniques essential for general insurance, extreme events, and time series analysis. The curriculum is designed to extend beyond introductory concepts, focusing on the distributional and dependency structures of risks.

Here's a rough breakdown of the key topics covered in the notes:

### 1. Introduction to General Insurance Modelling
* **Framework:** Introduces the fundamental **Collective Risk Model**, where total loss $S$ is the sum of random claim sizes $X_i$ over a random number of claims $N$.
* **Key Components:** Discusses the importance of modeling both **claim frequency** (the distribution of $N$) and **claim severity** (the distribution of $X_i$).
* **Moments:** Provides the formulas for the expected value and variance of the aggregate loss $S$ based on the moments of $N$ and $X$.
* **Generating Functions:** Explains the relationship between the moment generating function (MGF) of $S$ and the probability generating function (PGF) of $N$.

### 2. Collective Risk Modelling Theory
* **Individual vs. Collective Models:** Compares the two primary approaches to modeling total claims.
* **Convolutions:** Details how to compute the distribution of a sum of random variables using convolutions for both discrete and continuous cases.
* **Panjer's Recursion:** A key algorithm for computing the aggregate loss distribution for discrete claim sizes when the claim frequency follows a member of the $(a, b, 0)$ or $(a, b, 1)$ class of distributions (e.g., Poisson, Binomial, Negative Binomial).

### 3. Individual Claim Size Modelling
* **Data Preparation:** Covers essential steps like handling **left-truncation** (due to deductibles) and **right-censoring** (due to policy limits).
* **Descriptive Analysis:** Explains how to use tools like the **Cullen and Frey graph**, **Loss Index function**, and **Mean-Excess plot** to understand a dataset's distributional characteristics, particularly its tail behavior.
* **Parametric Distributions:** Summarizes the properties of common severity distributions, including Gamma, Inverse Gaussian, Weibull, Lognormal, and Pareto.
* **Parameter Estimation:** Details the two main methods for fitting distributions: **Moment Matching** and **Maximum Likelihood Estimation (MLE)**.
* **Model Selection:** Outlines various methods for comparing models, from graphical tools (Q-Q, P-P plots) to hypothesis tests and information criteria (AIC, BIC).

### 4. Copulas
* **Dependence Measures:** Compares traditional measures like **Pearson's correlation** with rank-based measures like **Kendall's tau** and **Spearman's rho**.
* **Sklar's Theorem:** Introduces the central concept of copulas, which separate the joint distribution of a random vector into its marginals and a function that captures the dependence structure.
* **Copula Families:** Explores different types of copulas, including the **Independence**, **Comonotonicity**, and **Countermonotonicity** copulas, as well as **Archimedean** copulas like the **Clayton**, **Frank**, and **Gumbel** families.
* **Tail Dependence:** Defines and quantifies the concepts of upper and lower tail dependence, which are crucial for modeling correlated extreme events.

### 5. Extreme Value Theory (EVT)
* **Tail Analysis:** Discusses methods for measuring and modeling the tails of distributions, which are critical for actuarial applications involving catastrophic losses.
* **Block Maxima (GEV):** Explains the **Generalized Extreme Value (GEV)** distribution as the limiting distribution of normalized block maxima.
* **Threshold Exceedances (GPD):** Introduces the **Generalized Pareto Distribution (GPD)** as the limiting distribution of excesses over a high threshold.
* **Estimation:** Covers the practical challenges and methods for fitting GEV and GPD distributions to data, including the selection of block size or threshold.

### 6. Time Series Fundamentals
* **Core Concepts:** Defines time series, **white noise**, and the properties of auto-covariance and auto-correlation functions (ACF).
* **Stationarity:** Distinguishes between strict and weak stationarity, and explains how to test for and handle non-stationarity using **detrending** and **differencing**.
* **Exploratory Analysis:** Uses tools like scatter plots and various smoothing techniques (Moving Average, Lowess, Splines) to visualize time-series data and identify patterns.

### 7. Time Series Models
* **ARIMA Models:** Provides a comprehensive overview of **Autoregressive (AR)**, **Moving Average (MA)**, and **ARMA** models, including their stationarity, invertibility, and ACF/PACF properties.
* **Seasonal ARIMA (SARIMA):** Extends ARIMA models to handle seasonal components in the data, explaining the role of seasonal differencing and seasonal AR/MA polynomials.
* **Multivariate Models:** Introduces **Vector Autoregressive (VAR)** models for analyzing and forecasting multiple time series simultaneously.
* **ARCH Models:** Describes **Autoregressive Conditional Heteroscedasticity (ARCH)** models, which are used to capture volatility clustering in financial time series.

## Appendix: R Code & Formulas

The notes are heavily annotated with R code examples for each model, demonstrating how to fit models, interpret outputs, and generate diagnostic plots. An appendix provides a quick reference guide to essential R functions and a summary of key proofs and derivations covered in the course.

This repository serves as a valuable resource for anyone studying or revising for ACTL30007, or for anyone seeking a concise yet comprehensive guide to advanced actuarial modelling concepts.
