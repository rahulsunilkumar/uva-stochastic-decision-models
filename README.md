# SYS 3060, Stochastic Decision Models; Spring 2026

This repository contains my coursework for SYS 3060 at the University of Virginia. The four assignments cover probability, continuous- and discrete-time Markov chains, and absorbing processes. The larger part of the repository is our final team project: a queueing analysis of the lunchtime ordering process at Roots Natural Kitchen.

## Project debrief

We observed 147 arrivals across three lunch periods and modeled the line as a tandem network: customers move through order taking, bowl assembly, and payment in sequence. Using the collected timestamps, we estimated arrival and service rates, checked the exponential assumptions, analyzed the system as three M/M/1 queues, and validated the results with a discrete-event simulation.

Order taking emerged as the bottleneck, with an estimated utilization of 0.778. The analytic model predicted an average system time of 7.49 minutes, closely matching the simulation estimate of 7.45 minutes. Adding a second order-taker reduced the analytic estimate to 3.60 minutes—a 52% improvement—while simulation produced a more conservative estimate of 4.24 minutes.

The study is best read as a practical application of stochastic modeling rather than a perfect account of restaurant operations. Observations came from short, busy lunch windows; grouped arrivals were sometimes recorded together; and some timestamps required cleaning. Even with those limitations, the model consistently identified the first stage as the best target for additional staffing.

## Repository contents

- `A01/`–`A04/`: course assignments
- `Project/Analysis/`: cleaned data and the reproducible Jupyter notebook
- `Project/Paper/`: final paper and figures
- `Project/Presentation/`: project presentation

To reproduce the analysis, install `requirements.txt` and run `Analysis/Roots Analysis Notebook.ipynb`.
