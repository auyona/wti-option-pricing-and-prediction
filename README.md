# WTI Option Pricing and Prediction

This repository contains my project on WTI crude oil futures that combines:

- Real-data analysis using historical WTI spot and futures prices  
- Ornstein–Uhlenbeck (OU) model for mean-reverting dynamics in commodities  
- European option pricing formulas applied to WTI futures under the OU process  
- LaTeX reports with full mathematical derivations and results  

---

## Project Structure

README.md # This file
/report/ # LaTeX reports + compiled PDFs
option_pricing.tex
price_prediction.tex
crude_oil_price_prediction.pdf
crude_oil_price_prediction_chart.png
/data/ # WTI crude oil datasets
wti_crude_oil_price.csv
wti_spot_price.csv


---

## Highlights

- Implemented OU mean-reverting process for WTI futures:
  \[
    dF_t = \theta(\mu - F_t)\,dt + \sigma dW_t
  \]
- Derived closed-form formulas for European call/put options under OU distribution  
- Calibrated model parameters \((\theta, \mu, \sigma)\) using real WTI data  
- Compared OU-based pricing vs. traditional Black–Scholes framework  
- Produced full LaTeX reports with equations, code, and graphs  

---

## Reports

- [`option_pricing.tex`](report/option_pricing.tex) – LaTeX source for option pricing write-up  
- [`price_prediction.tex`](report/price_prediction.tex) – LaTeX source for crude oil price prediction  
- [`crude_oil_price_prediction.pdf`](report/crude_oil_price_prediction.pdf) – Compiled PDF report  
- [`crude_oil_price_prediction_chart.png`](report/crude_oil_price_prediction_chart.png) – Chart used in report  

---

## Data

- [`wti_crude_oil_price.csv`](data/wti_crude_oil_price.csv) – Historical WTI crude oil futures  
- [`wti_spot_price.csv`](data/wti_spot_price.csv) – Historical WTI crude oil spot prices  

---

## How to Compile the LaTeX Reports

If you want to rebuild the PDFs from the LaTeX source:

```bash
cd report
pdflatex option_pricing.tex
pdflatex price_prediction.tex
