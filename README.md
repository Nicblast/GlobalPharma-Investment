## Project BioFuture: R&D Acceleration & Acquisition Valuation

**Executive Overview**

This is astrategic evaluation of the acquisition of BioFuture ($1.2B valuation) and the financial viability of a $150M investment to accelerate Phase II clinical trials. This analysis bridges clinical performance, financial modeling, and regulatory risk.

## Methodology

**Data Processing:**

I cleaned the GlobalPharma Dataset.ods using pandas by mean-imputing missing patient counts. Performed exploratory data analysis (EDA) via df.info() and df.describe() to validate data integrity.

**Visualization:**

I then generated an histograms with matplotlib and seaborn to assess the distributions of patient counts, success scores, R&D spend, and compliance scores.

**Financial Modeling:**

Before automation I perfomed manual calculation. I calculated the drug's Current Expected Value using baseline success probabilities and drug market value.

**Optimization:**

I finally conducted a Break-Even Analysis to determine the exact Phase II success rate increase required to offset the $150M additional investment.


## Strategic Investment Analysis

**1. Terminal Success Probability ($P_S$)**
This would be the likelihood of the asset reaching the market given a potentially successful Phase II trial.
$$P_S = P_{III} \times P_A$$
* **Why:** This "Filter" takes into accounts for all risks remaining after the current stage.
* **Calculation:** $0.60 \times 0.90 = 0.54$

---

**2. Risk-Adjusted Success Value ($V_S$)**
This is nothing but the expected monetary value of the project at the moment the Phase II milestone is achieved.
$$V_S = P_S \times R$$
* **Why:** This "Success Value" represents the real prize we want. It is the revenue ($R$) adjusted for possible future failures.
* **Calculation:** $0.54 \times \$1,200M = \$648M$

---

**3. The Break-Even Hurdle ($\Delta P$)**
The specific increase in probability required to justify the investment cost ($I$).
$$\Delta P = \frac{I}{V_S}$$
* **Why:** This ratio calculates the Efficiency Requirment." It determines how much probability we must "buy" or guarantee ourselves to cover our $150M bill.
* **Calculation:** $\$150M / \$648M \approx 0.2315$

---

**4. Final Business Metric**
Converting the probability delta into standard percentage points.
$$\text{Required Increase} = \Delta P \times 100$$
* **Result:** $0.2315 \times 100 = 23.15$

<img width="1601" height="1054" alt="IMG_3536" src="https://github.com/user-attachments/assets/2525fff5-d48c-448d-9034-21c8e80633bb" />
















