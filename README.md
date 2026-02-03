# Multi-Asset-Trend-Following-Strategy
ESILV Algotrading 2025-26 Capstone Project
Author: Paul Hochenauer

## Project Overview
This project implements and optimizes a cross-asset quantitative trading strategy based on Managed Futures (Commodity Trading Advisors - CTA) principles. The goal is to study a simple trend-following algorithm and refine it to improve risk-adjusted returns across various market regimes.

The strategy is tested on a dataset of daily closing prices for 47 assets spanning multiple asset classes.

## Key Features
Data Processing: Utilizes daily log-returns for mathematical compounding advantages and normal distribution modeling.

Time-Series Standardization: Implements forward-filling techniques to ensure a continuous time series, preventing "gaps" during weekends or holidays that could disrupt trend signals.

Signal Filtering: Uses statistical methods, such as the t-statistic, to weight signals and filter out market "noise," ensuring trades are only executed on statistically significant trends.

Robust Backtesting: Evaluation is conducted over a 15-year period (2010–2025), including an out-of-sample validation phase.

## Technical Stack
Language: Python

Libraries: * Pandas & NumPy: Data manipulation and numerical computation.

Matplotlib & Seaborn: Exploratory Data Analysis (EDA) and correlation heatmaps.

tqdm: Progress tracking for long backtesting loops.

## Performance Results
The optimized version of the strategy (CWRP) significantly outperformed the initial baseline:

Annualized Return: 18.78%.

Sharpe Ratio: 1.4162 (compared to a baseline of 0.0107).

Volatility: Reduced from 15.45% to 13.26%.

Stability: Demonstrated superior performance during the 2021–2022 market surges and effective management of 2024 plateaus.

## Repository Structure
capstone 2026-Hochenauer.ipynb: The main research and implementation notebook.

assets_data_student.csv: Historical daily closing prices for 47 assets.
