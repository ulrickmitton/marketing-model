# Estimating ROI Across Media Channels

This project builds a **marketing mix model (MMM)** to evaluate the effectiveness and ROI of four media channels—**TV, Digital, Print, and Social**—in driving product sales. The goal is to simulate and analyze how spending on each channel influences sales, and estimate the cost of increasing sales by 1% through each medium.

---

## Objective

Using simulated data, this notebook demonstrates:

- How media spend influences sales outcomes.
- How log-transformations help capture **diminishing returns**.
- How to estimate the **cost per 1% sales lift** across channels.
- Which media type offers the most efficient ROI.

---

## Methods

- **Data Simulation:** Synthetic data generated to reflect realistic ranges of media spend and their effect on sales.
- **OLS Regression:** Settled on a log-linear specification after an initial iteration.

---

## Findings

- Marketing relationships are often non-linaar; log transformation resulted in better fit.
- Important to be congnizant of saturation (i.e diminishing marginal effect) of additional ad spend

---

## Visualization Example

![ROI Bar Chart](#)

> A bar chart displays the estimated cost of a 1% increase in sales by media type, revealing which channel delivers the best marginal return.

---

## Equation Used

The cost to achieve a 1% lift in sales via channel \( i \) is:


Cost_i = bar{x}_i * ( e^(.01/beta_i) - 1 )


Where:
- bar{x}_i = average spend for channel \( i \)
- beta_i = estimated coefficient for logged media spend from the regression

---


---

## File

- `MixedMarketing.ipynb` – The full notebook with code, model, and commentary.

---

## Next Steps

- Extend to include*interaction terms (e.g., cross-channel synergies).
- Adjust seasonality and incorporate lag effects to better reflect real-world dynamics.
- Test against real data (e.g., advertising datasets, panel surveys).

---

## Stack

- Python (Pandas, NumPy, Matplotlib, Statsmodels)
- Jupyter Notebook

----

## Contact
LinkedIn: [LinkedIn](https://www.linkedin.com/ulrickmitton) 
email: mitton.ulrick@gmail.com

