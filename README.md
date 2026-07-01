# Spread Locator — Advanced Statistics 📊🔬

[![Notebook](https://img.shields.io/badge/Notebook-Jupyter-orange)](./Spread%20Locator/Spread%20Locator.ipynb) [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/kotadiyadarshil18-code/Mathematics-Advanced-Statistics/blob/main/Spread%20Locator/Spread%20Locator.ipynb) [![Watch Demo](https://img.shields.io/badge/Watch%20Demo-YouTube-red)](https://youtu.be/REPLACE_WITH_YOUR_VIDEO_URL)

> Analysis of transaction data using Bernoulli, Binomial, Poisson, Log-Normal, Power Law distributions, Box-Cox transform, Q-Q plots, Z-scores, PDF/CDF visualizations and decision making insights.

---

## Table of Contents
- [Overview](#overview)
- [Demo & Buttons](#demo--buttons)
- [How to run](#how-to-run)
- [Key Formulas & Emojis](#key-formulas--emojis)
- [Charts / Screenshots](#charts--screenshots)
- [How to save screenshots programmatically](#how-to-save-screenshots-programmatically)
- [Conclusions & Insights](#conclusions--insights)
- [License](#license)

---

## Overview
This project contains exploratory analysis of a transaction dataset:
- Transaction occurrence modeled via Bernoulli (Success/Fail) ✅❌
- Weekly transaction counts: Binomial-like analysis
- Daily transactions: Poisson process modeling (λ)
- Transaction amounts: Log-Normal vs Power-Law fits, Q-Q plot, Box-Cox transform
- Z-scores, PDF and CDF for transaction amount behavior and probability estimates

---

## Demo & Buttons
- Open notebook: [Open Spread Locator Notebook](./Spread%20Locator/Spread%20Locator.ipynb)  
- Run in Google Colab: [Open in Colab](https://colab.research.google.com/github/kotadiyadarshil18-code/Mathematics-Advanced-Statistics/blob/main/Spread%20Locator/Spread%20Locator.ipynb)  
- Demo video: [Watch the Demo 🎥](https://youtu.be/REPLACE_WITH_YOUR_VIDEO_URL)

(If you'd like a clickable "button" look, GitHub supports simple HTML. Example:)
<p align="left">
  <a href="https://github.com/kotadiyadarshil18-code/Mathematics-Advanced-Statistics/blob/main/Spread%20Locator/Spread%20Locator.ipynb">
    <img src="https://img.shields.io/badge/Open%20Notebook-View-blue" alt="Open Notebook" />
  </a>
  <a href="https://colab.research.google.com/github/kotadiyadarshil18-code/Mathematics-Advanced-Statistics/blob/main/Spread%20Locator/Spread%20Locator.ipynb">
    <img src="https://img.shields.io/badge/Open%20in%20Colab-Run-orange" alt="Open in Colab" />
  </a>
  <a href="https://youtu.be/REPLACE_WITH_YOUR_VIDEO_URL">
    <img src="https://img.shields.io/badge/Watch%20Demo-YouTube-red" alt="Watch Demo" />
  </a>
</p>

---

## How to run
1. Clone the repo:
   ```bash
   git clone https://github.com/kotadiyadarshil18-code/Mathematics-Advanced-Statistics.git
   cd Mathematics-Advanced-Statistics/Spread\ Locator
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   or at minimum:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy statsmodels openpyxl
   ```
3. Open the notebook:
   - Locally: `jupyter notebook "Spread Locator/Spread Locator.ipynb"`
   - Or click "Open in Colab" or "Open Notebook" above.

---

## Key Formulas & Emojis 🧮✨

- Bernoulli (p): Probability of success  
  🟢 Bernoulli: P(X=1) = p, P(X=0) = 1-p

- Binomial:  
  🔢 Binomial(k; n, p) = C(n,k) p^k (1-p)^(n-k)

- Poisson:  
  📈 Poisson(k; λ) = e^{-λ} λ^k / k!

- Log-Normal PDF (X > 0):  
  🧾 f(x; μ, σ) = (1/(x σ sqrt(2π))) exp(- (ln x - μ)^2 / (2 σ^2))

- Power-law (Pareto-like):  
  ⚡ f(x) ∝ x^{-α}

- Z-score:  
  🧮 z = (x - μ) / σ

- Box-Cox transform (λ):  
  🔁 x(λ) = { (x^λ - 1) / λ,  if λ ≠ 0;  ln(x), if λ = 0 }

Use these to interpret fits and parameters in the notebook.

---

## Charts / Screenshots 📷
Below are placeholders for the screenshots of the charts generated in the notebook. Save the chart images into this repo (recommended path: `Spread_Locator/screenshots/`) and update the filenames if different.

1. Bernoulli (Transaction Occurrence)
![Bernoulli Countplot](Spread_Locator/screenshots/bernoulli.png)

2. Binomial-like (Weekly Transaction Counts)
![Weekly Transactions Histogram](Spread_Locator/screenshots/binomial.png)

3. Poisson (Transactions Per Day)
![Poisson PMF](Spread_Locator/screenshots/poisson.png)

4. Log-Normal Fit (Transaction Amounts)
![LogNormal Fit](Spread_Locator/screenshots/lognormal.png)

5. Power-Law Fit (Transaction Amounts)
![PowerLaw Fit](Spread_Locator/screenshots/powerlaw.png)

6. Q-Q Plot (Test Normality)
![Q-Q Plot](Spread_Locator/screenshots/qqplot.png)

7. Box-Cox Transformation (Before / After)
![Box-Cox Before After](Spread_Locator/screenshots/boxcox.png)

8. PDF (Transaction Amount using Normal approx)
![PDF Plot](Spread_Locator/screenshots/pdf.png)

9. CDF (Transaction Amount)
![CDF Plot](Spread_Locator/screenshots/cdf.png)

10. (Optional) Z-score table / high-value detection
![Z-Scores](Spread_Locator/screenshots/zscores.png)

> Note: I recommend using a directory without spaces for screenshots (`Spread_Locator/screenshots/`) to avoid URL encoding issues. If you prefer the `Spread Locator/` folder, change the image paths accordingly and escape spaces when linking.

---

## How to save screenshots programmatically (copy-ready snippet)
Put this snippet into your notebook (after each plotting cell) to save the figures automatically into `Spread_Locator/screenshots/`:

```python
import os
os.makedirs("Spread_Locator/screenshots", exist_ok=True)

# After creating a figure (plt.figure() / sns.*)
# plt.plot(...); plt.title("...")  # your existing plotting code
plt.savefig("Spread_Locator/screenshots/bernoulli.png", bbox_inches='tight', dpi=150)
# repeat for each figure with a descriptive filename
```

Suggested filenames and where to add the save commands:
- `bernoulli.png` — after countplot
- `binomial.png` — after histplot(transaction_count)
- `poisson.png` — after Poisson bar plot
- `lognormal.png` — after lognormal fit overlay
- `powerlaw.png` — after powerlaw fit plot
- `qqplot.png` — after stats.probplot()
- `boxcox.png` — after Box-Cox plots
- `pdf.png` / `cdf.png` — after PDF and CDF plots
- `zscores.png` — screenshot of df.head() or a histogram of z-scores

---

## Conclusions & Insights ✅
- Log-Normal best fits transaction amounts (positive skew).  
- Poisson describes daily transaction counts (λ ≈ observed mean).  
- Bernoulli useful to model success/failure of individual transactions.  
- Box-Cox helps stabilize variance for further modeling.  
- Use Z-scores to flag high-value transactions for review (fraud detection).

---

## Next steps / How I can help
- I can add the demo video URL and upload the screenshots if you provide them (or paste the links here).
- I can run the notebook and generate the screenshots for you and commit them into the repo.

---

## License
MIT License — feel free to reuse and adapt this README.
