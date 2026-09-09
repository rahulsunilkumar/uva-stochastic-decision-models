# Roots Natural Kitchen Queueing Analysis

A data-driven analysis of the in-person ordering process at Roots Natural Kitchen using queueing theory and discrete-event simulation.

## Project Structure

```
.
├── Analysis/                            
│   ├── Roots Analysis Notebook.ipynb
│   ├── Roots Final Data.xlsx
├── Paper/                               
│   ├── Roots Paper.pdf
│   ├── Figures/                         
│   │   ├── comparison.png
│   │   ├── distribution-fits.png
│   │   ├── impact.png
│   │   ├── sensitivity.png
│   │   └── utilization.png
├── Presentation/                        
│   ├── Roots Presentation.pptx
├── README.md
├── requirements.txt
```

## Overview

This project models the service process as a three-stage tandem queue:
1. Order Taking  
2. Assembly  
3. Cashier / Payment  

Using real timestamp data, the system is analyzed both analytically and through simulation to identify bottlenecks and evaluate improvements.

## Methods

- M/M/1 and tandem queue modeling  
- Steady-state performance analysis  
- Discrete-event simulation  
- Empirical validation with real data 

## Key Results

- Order taking is the primary bottleneck  
- Utilization at Stage 1 is ~0.78  
- Analytical model predicts ~7.49 min average system time  
- Simulation predicts ~7.45 min  
- Adding a second order-taker reduces time to ~3.60 min (~52% improvement)  
 

## How to Run

Install dependencies:
```bash
pip install -r requirements.txt
```

Run the main notebook in `Analysis/` to reproduce results.
