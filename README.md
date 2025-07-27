# 📊 Marketing Mix Modeling: Estimating ROI Across Media Channels

This project builds a **marketing mix model (MMM)** to evaluate the effectiveness and ROI of four media channels—**TV, Digital, Print, and Social**—in driving product sales. The goal is to simulate and analyze how spending on each channel influences sales, and estimate the cost of increasing sales by 1% through each medium.

---

## 🔍 Objective

Using simulated data, this notebook demonstrates:

- How media spend influences sales outcomes.
- How log-transformations help capture **diminishing returns**.
- How to estimate the **cost per 1% sales lift** across channels.
- Which media type offers the most efficient ROI.

---

## 🧠 Methods

- **Data Simulation:** Synthetic data generated to reflect realistic ranges of media spend and their effect on sales.
- **Log-Linear OLS Regression:** Models the marginal impact of spend while capturing diminishing returns.
- **Robust Standard Errors (HC1):** Corrects for heteroskedasticity.
- **Multicollinearity Checks:** VIF scores calculated to ensure stable estimates.

---

## 📉 Key Insights

- **Model Fit:** Raw sales modeled with logged spend showed strong fit (R² = 0.994).
- **ROI Estimation:** A custom exponential function calculates how much spend is required to generate a 1% increase in sales.
- **Unexpected Result:** Despite lower overall spend, Print showed the most cost-effective ROI per 1% sales gain—highlighting the value of smaller, targeted channels.

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

## Stack

- Python (Pandas, NumPy, Matplotlib, Statsmodels)
- Jupyter Notebook

---

## File

- `MixedMarketing.ipynb` – The full notebook with code, model, and commentary.

---

## Next Steps

- Extend to include*interaction terms (e.g., cross-channel synergies).
- Adjust seasonality and incorporate lag effects to better reflect real-world dynamics.
- Test against real data (e.g., advertising datasets, panel surveys).

---

## 📬 Contact

Questions or feedback? Feel free to connect via [LinkedIn](https://www.linkedin.com/ulrickmitton) or open an issue.

