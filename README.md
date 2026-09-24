# Bermudan Swaptions (Hull–White) & NIG Pricing

**Assignment 6** · MATLAB · Financial Engineering course, Politecnico di Milano

Two structured-product case studies: an **equity certificate swap** priced under a calibrated Normal Inverse Gaussian model, and a **10y Bermudan payer swaption** priced on a Hull–White trinomial tree.

## What we did

- **NIG calibration** to the EURO STOXX 50 smile with Lewis/FFT pricing.
- **Certificate swaps** (2y and 3y with double trigger) priced by Monte Carlo; flat-vol Black misprices the upfront by 64 bp (2y) and 114 bp (3y) on EUR 100M.
- **Bermudan swaption** (10y, non-call 2, strike 5%) on a Hull–White trinomial tree (a = 0.11, σ = 0.008).
- Tree validated against the market ZCB curve and the **Jamshidian** decomposition; price lies within analytical no-arbitrage bounds.

## Repository structure

| Path | Content |
|---|---|
| `runAssignment6_Group5.m` | Main script |
| `bootstrap/` | Discount-curve bootstrap |
| `ex_1/` | Case study 1 — NIG calibration and certificate pricing |
| `ex_2/` | Case study 2 — Hull–White tree, Bermudan and Jamshidian pricing |
| `REPORT_Assignment6_Group5.pdf` | Report |

## How to run

Open the folder in MATLAB (R2023b or later) and run `runAssignment6_Group5.m`. It adds the sub-folders to the path and executes every exercise in order.

## Team

Gabriele Alippi, Elisa Colombo, Simone Colombo, Giacomo Costa

Part of the **Financial Engineering** course (Prof. R. Baviera) — M.Sc. in Mathematical Engineering, Quantitative Finance, Politecnico di Milano, A.Y. 2025/26.
