# 📊 Spread Locator

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blue?style=for-the-badge&logo=numpy)
![SciPy](https://img.shields.io/badge/SciPy-Statistics-green?style=for-the-badge&logo=scipy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal?style=for-the-badge)
![License](https://img.shields.io/badge/License-Educational-success?style=for-the-badge)

---

# 📖 Project Overview

**Spread Locator** is a statistical data analysis project developed using **Python**, **Jupyter Notebook**, and **Statistical Distribution Models**. The project focuses on understanding how transaction data is distributed by applying different probability distributions and statistical techniques.

The project combines **theoretical concepts** with **practical implementation** to analyze real-world data. Various probability distributions, statistical transformations, visualization techniques, and hypothesis-testing methods are used to identify data patterns, detect outliers, evaluate normality, and understand transaction behavior.

This project demonstrates how statistical analysis can support data-driven decision-making by selecting appropriate probability distributions and interpreting the characteristics of a dataset through graphical and mathematical approaches.

---

# 🎯 Objectives

The main objectives of this project are:

- 📊 Understand statistical distributions and their real-world applications.
- 📈 Analyze transaction data using probability distribution models.
- 🔍 Identify data patterns and trends through visualization.
- 📉 Test whether the dataset follows a normal distribution.
- 📐 Apply statistical transformations to improve data quality.
- 📊 Compare multiple probability distributions.
- 💻 Perform statistical analysis using Python.
- 📚 Learn practical implementation of statistical concepts.
- 🚀 Improve data interpretation and analytical skills.
- 📑 Present results using professional visualizations.

---

# ✨ Project Features

- ✅ Statistical Distribution Analysis
- ✅ Bernoulli Distribution
- ✅ Binomial Distribution
- ✅ Poisson Distribution
- ✅ Log-Normal Distribution
- ✅ Power Law Distribution
- ✅ Q-Q Plot Analysis
- ✅ Box-Cox Transformation
- ✅ Z-Score Analysis
- ✅ PDF & CDF Visualization
- ✅ Python Implementation
- ✅ Data Visualization
- ✅ Statistical Interpretation

---





---

# 📚 Part A – Theoretical Foundation


➡️ **[_Click here for Spread Locator.pdf](https://drive.google.com/file/d/10X3IZSVHkEsJDXeVtlGL4KBrxsyzVjTU/view?usp=sharing)**

---
# 📊 Part B – Data Analysis & Testing Tasks

## 📖 Overview

Part B focuses on the practical implementation of the statistical concepts introduced in Part A. Using Python, Jupyter Notebook, and the provided dataset, this section demonstrates how different probability distributions and statistical techniques can be applied to analyze real-world transaction data.

The notebook performs data loading, preprocessing, visualization, statistical testing, and distribution fitting. Each task includes Python implementation, graphical outputs, and result interpretation to help understand the behavior of the dataset.

---

# 🎯 Objectives of Part B

- 📂 Import and explore the dataset.
- 🧹 Perform data preprocessing and cleaning.
- 📊 Analyze the distribution of transaction data.
- 📈 Visualize data using statistical plots.
- 📉 Apply different probability distributions.
- 📐 Test data normality using Q-Q Plot.
- 🔄 Transform skewed data using Box-Cox Transformation.
- 📏 Calculate Z-Scores for transaction values.
- 📊 Plot PDF and CDF graphs.
- 📋 Compare distributions and interpret results.

---

# 📁 Dataset Information

**Dataset Name**

```text
spread_locator_dataset.xlsx
```

The dataset contains transaction-related information that is used throughout this project to perform statistical analysis and probability distribution modeling. It serves as the foundation for all experiments carried out in Part B.

---

# 📋 Dataset Columns

| Column Name | Description |
|--------------|-------------|
| Date | Date of the transaction |
| Transaction_ID | Unique transaction identifier |
| Customer_ID | Unique customer identifier |
| Transaction_Amount | Amount of each transaction |
| Payment_Method | Payment method used |
| Transaction_Status | Status of the transaction |
| Merchant_Category | Merchant category |
| Location | Transaction location |
| Time | Time of transaction |

> **Note:** Replace this table with the exact column names from your `spread_locator_dataset.xlsx` if they are different.

---

# 🛠️ Libraries Used

The following Python libraries are used throughout this project:

```python
import pandas as pd
import numpy as np

import matplotlib.pyplot as plt
import seaborn as sns

from scipy import stats
from scipy.stats import (
    bernoulli,
    binom,
    poisson,
    norm,
    lognorm,
    powerlaw,
    boxcox,
    zscore
)

import statsmodels.api as sm
```

---

# ⚙️ Purpose of Each Library

| Library | Purpose |
|----------|---------|
| **Pandas** | Data loading, cleaning, and manipulation |
| **NumPy** | Numerical calculations and array operations |
| **Matplotlib** | Creating charts and visualizations |
| **Seaborn** | Statistical data visualization |
| **SciPy** | Probability distributions and statistical tests |
| **Statsmodels** | Q-Q Plot and advanced statistical analysis |

---



---

# 📚 Practical Tasks

The following statistical tasks are performed in this notebook:

✅ Task 1 – Fit the data to Bernoulli and Binomial Distributions

✅ Task 2 – Fit the data to Poisson Distribution

✅ Task 3 – Model transaction amounts using Log-Normal and Power Law Distributions

✅ Task 4 – Generate and interpret a Q-Q Plot

✅ Task 5 – Apply Box-Cox Transformation

✅ Task 6 – Calculate Z-Scores and probability of transactions exceeding ₹5000

✅ Task 7 – Plot and interpret PDF and CDF

✅ Task 8 – Conclude which distribution best fits the dataset

---

# 1️⃣ Task 1 – Fit the Data to Bernoulli and Binomial Distributions

## 📖 Explanation

The objective of this task is to fit the dataset to **Bernoulli** and **Binomial** distributions. The Bernoulli distribution is used when an experiment has only two possible outcomes, such as **Success (1)** or **Failure (0)**. The Binomial distribution extends this concept by calculating the probability of obtaining a specific number of successes over a fixed number of independent trials. This analysis helps evaluate whether the transaction data follows these probability models and provides insight into transaction behavior. :contentReference[oaicite:0]{index=0}

---

## 🎯 Objective

- Fit the data to Bernoulli Distribution.
- Fit the data to Binomial Distribution.
- Visualize the probability distributions.
- Interpret the statistical results.

---

## 📐 Formula

### Bernoulli Distribution

$$
P(X=1)=p
$$

$$
P(X=0)=1-p
$$

Mean:

$$
\mu=p
$$

Variance:

$$
\sigma^2=p(1-p)
$$

### Binomial Distribution

$$
P(X=k)=\binom{n}{k}p^k(1-p)^{n-k}
$$

Mean:

$$
\mu=np
$$

Variance:

$$
\sigma^2=np(1-p)
$$

---

## 💻 Python Code

```python
# Bernoulli

#Success = 1, fail = 0

df["transaction_occurrence"] = df["transaction_status"].map({
    "Success" : 1,
    "Fail": 0
})

sns.countplot(x=df["transaction_occurrence"])
plt.title("Bernoulli Distribution - Transaction Occurrence")
plt.xlabel("Transaction (0= Fail, 1=success)")
plt.ylabel("Count")
plt.show()

## Binomial Distribution

sns.histplot(df["transaction_count"], bins=10)

plt.title("Binomal Distribution Weekly Transaction Counts")
plt.xlabel("NUmber of transactions per week ")
plt.ylabel("Frequency")

plt.show()
```

---

## 📸 Output

**Bernoulli Distribution**
>  <img width="715" height="568" alt="Screenshot 2026-07-01 114609" src="https://github.com/user-attachments/assets/f3ae1d46-17ac-40f8-950a-c53a79fdfeb4" />

**Binomial Distribution**
>  <img width="707" height="570" alt="Screenshot 2026-07-01 114713" src="https://github.com/user-attachments/assets/3d0a53dd-20c4-4175-9091-b7be3877f850" />


---

## 📊 Interpretation

- The Bernoulli Distribution models whether a transaction is successful or unsuccessful.
- The Binomial Distribution models the probability of obtaining a specific number of successful transactions over multiple trials.
- The resulting plots help determine how well the transaction data follows these distributions.
- If the observed probabilities closely match the theoretical distribution, the model is considered a good fit for the dataset.

---

## ✅ Conclusion

The Bernoulli and Binomial distributions provide a simple yet effective way to model binary events and repeated trials. They help understand transaction occurrence patterns and estimate the probability of successful outcomes in the dataset.

---

# 2️⃣ Task 2 – Fit the Data to Poisson Distribution

## 📖 Explanation

The Poisson Distribution is used to model the number of times an event occurs within a fixed interval of time or space. In this project, it is used to analyze the frequency of transactions occurring within a specific period. This distribution is suitable when events occur independently and the average rate of occurrence remains constant.

By fitting the dataset to a Poisson Distribution, we can determine whether the observed transaction counts follow the expected probability pattern. This helps in understanding transaction frequency and predicting future occurrences.

---

## 🎯 Objective

- Understand the Poisson Distribution.
- Calculate the average transaction rate (λ).
- Fit the dataset to the Poisson model.
- Compare observed and expected frequencies.
- Visualize the distribution using Python.

---

## 📌 Real-World Example

Suppose a customer service center receives **5 calls per hour** on average.

Using the Poisson Distribution, we can calculate the probability of receiving:

- 📞 0 Calls
- 📞 2 Calls
- 📞 5 Calls
- 📞 10 Calls

within the next hour.

---

## 📐 Formula

### Probability Mass Function

$$
P(X=k)=\frac{e^{-\lambda}\lambda^k}{k!}
$$

Where,

- **λ** = Average number of events
- **k** = Number of occurrences
- **e** = Euler's constant

### Mean

$$
\mu=\lambda
$$

### Variance

$$
\sigma^2=\lambda
$$

---

## 💻 Python Code

```python
daily_transaction = df.groupby("transaction_date").size()

lam = daily_transaction.mean()
print("Lambda:",lam)

x = np.arange(0,daily_transaction.max()+3)

pmf = poisson.pmf(x,lam)

plt.figure(figsize=(7,4))
plt.bar(x,pmf,color='blue')
plt.title("Poisson Distribution")
plt.xlabel("Transaction Per Day")
plt.ylabel("Probability")
plt.show()
```

---

## 📸 Output Screenshot

**Poisson Distribution**
 > <img width="777" height="492" alt="Screenshot 2026-07-01 114723" src="https://github.com/user-attachments/assets/3b24d962-04b2-490f-8640-7a9bfc798408" />

> 

Example:

![Poisson Distribution](images/task2_poisson.png)

---

## 📊 Interpretation

- The graph illustrates the probability of observing different transaction counts.
- The highest probability occurs near the average transaction rate.
- As the number of events moves away from the mean, the probability decreases.
- The Poisson Distribution is effective for modeling count-based transaction data.

---

## 📌 Applications

- 📞 Call Center Analysis
- 🚗 Traffic Monitoring
- 🌐 Website Visitors
- 🏥 Hospital Patient Arrivals
- 💳 Banking Transactions
- 🛒 Customer Purchases

---

## ✅ Conclusion

The Poisson Distribution successfully models the occurrence of transaction events over a fixed interval. It provides valuable insights into transaction frequency and helps estimate the likelihood of future transaction counts based on historical data.

---
---

# 3️⃣ Task 3 – Model Transaction Amounts using Log-Normal and Power Law Distributions

## 📖 Explanation

In this task, the transaction amounts are analyzed using **Log-Normal** and **Power Law** distributions. Financial transaction values are generally **positive** and often **right-skewed**, making them unsuitable for a normal distribution.

The **Log-Normal Distribution** assumes that the logarithm of the transaction amounts follows a normal distribution. It is widely used for modelling stock prices, income, transaction values, and biological measurements.

The **Power Law Distribution** is used when the dataset contains many small values and only a few extremely large values. It helps identify heavy-tailed behaviour where rare but very large transactions occur more frequently than expected.

By comparing both distributions, we can determine which model better represents the transaction data.

---

# 🎯 Objective

- Analyze transaction amounts.
- Fit Log-Normal Distribution.
- Fit Power Law Distribution.
- Compare both distributions.
- Identify the best-fitting model.

---

# 🌍 Real-World Applications

### 📈 Log-Normal Distribution

- Stock Prices
- Annual Income
- Property Prices
- Insurance Claims
- Financial Transactions

### ⚡ Power Law Distribution

- Earthquake Magnitudes
- City Population
- Website Traffic
- Social Media Followers
- Wealth Distribution

---

# 📐 Mathematical Formula

## Log-Normal Distribution

If

$$
Y=\ln(X)
$$

is normally distributed,

then

$$
X
$$

follows a Log-Normal Distribution.

Probability Density Function

$$
f(x)=\frac{1}{x\sigma\sqrt{2\pi}}
e^{-\frac{(\ln x-\mu)^2}{2\sigma^2}}
$$

---

## Power Law Distribution

$$
P(X=x)=Cx^{-\alpha}
$$

Where

- **C** = Constant
- **α** = Power Law Exponent

---

# 💻 Python Code

```
amt = df['transaction_amount']

shape , loc, scale = lognorm.fit(amt,floc=0)

print("Shap:", shape)
print("Scale:",scale)

plt.figure(figsize=(8,5))

sns.histplot(amt, bins = 30, stat='density', color='skyblue')

x=np.linspace(amt.min(),amt.max(), 300)

pdf= lognorm.pdf(x, shape, loc, scale)

plt.plot(x, pdf, 'r', linewidth=2)
plt.title("Log-Normal Fit")
plt.show()

## Power Law Distribution
shape, loc, scale= powerlaw.fit(amt)
print("shape:",shape)

pdf= powerlaw.pdf(x, shape, loc, scale)
plt.figure(figsize=(8,5))

sns.histplot(amt, bins=30, stat="density", color='green')

plt.plot(x, pdf, 'red', linewidth = 2 )

plt.title("Power Law Fit")
plt.show()
```

---

# 📸 Output Screenshot

### 📈 Log-Normal Distribution

> <img width="910" height="587" alt="Screenshot 2026-07-01 114732" src="https://github.com/user-attachments/assets/082ddfce-6e05-4f3b-a1dc-45d3660ce3c6" />





---

### ⚡ Power Law Distribution

> <img width="901" height="587" alt="Screenshot 2026-07-01 115743" src="https://github.com/user-attachments/assets/07e0e85f-c97a-4bc9-a4e1-99ac07feeb90" />



---

# 📊 Interpretation

### 📈 Log-Normal Distribution

- The graph shows that transaction amounts are positively skewed.
- Most transactions have lower values.
- Very high-value transactions occur less frequently.
- The distribution is suitable for modelling positive financial data.

---

### ⚡ Power Law Distribution

- The graph contains a heavy tail.
- Small transaction values occur very frequently.
- Large transaction values are rare but still possible.
- The distribution highlights extreme financial transactions.

---

# 📌 Comparison

| Log-Normal | Power Law |
|------------|-----------|
| Positive values only | Heavy-tailed distribution |
| Right-skewed | Extreme values occur frequently |
| Suitable for financial data | Suitable for rare large events |
| Smooth decline | Long-tail behaviour |

---

# ✅ Conclusion

The comparison of Log-Normal and Power Law distributions provides valuable insights into transaction amount behaviour. If the dataset is moderately right-skewed, the Log-Normal Distribution generally provides a better fit. If the dataset contains many extreme values, the Power Law Distribution may better capture the underlying pattern. Selecting the appropriate model improves the accuracy of statistical analysis and future predictions.

---

---

# 4️⃣ Task 4 – Generate and Interpret a Q-Q Plot

## 📖 Explanation

The **Quantile-Quantile (Q-Q) Plot** is a graphical technique used to determine whether the dataset follows a normal distribution. It compares the quantiles of the observed data with the quantiles of a theoretical normal distribution.

If the plotted points lie close to the reference line, the dataset is considered approximately normally distributed. Significant deviations from the line indicate skewness, outliers, or that the data does not follow a normal distribution.

In this project, the Q-Q Plot is used to evaluate whether the transaction amounts satisfy the normality assumption before applying statistical models.

---

# 🎯 Objective

- Check whether the dataset follows a normal distribution.
- Detect skewness and outliers.
- Compare sample quantiles with theoretical quantiles.
- Interpret the normality of transaction data.

---

# 🌍 Real-World Applications

- Machine Learning
- Financial Analysis
- Medical Research
- Quality Control
- Statistical Modeling

---

# 💻 Python Code

```python
plt.figure(figsize=(8,5))

stats.probplot(amt, dist="norm", plot=plt)
plt.title("Q-Q Plot")

plt.show()

# Sharpiro-Wilk test

stats, pvalue = stats.shapiro(amt)
print("Shapiro-Wilk Test Statistics:", stats)
print("p-value:", pvalue)

if pvalue > 0.05:
    print("Data appear Normally Distributed")
else:
    print("Data is Not Normally Distributed")
```

---

# 📸 Output Screenshot

> <img width="898" height="592" alt="Screenshot 2026-07-01 115853" src="https://github.com/user-attachments/assets/099eb933-2783-448b-91e1-a5aa3afd2836" />


---

# 📊 Interpretation

### ✅ If Points Follow the Straight Line

- Data is approximately normally distributed.
- Statistical tests based on normality can be applied.
- No significant skewness is present.

### ❌ If Points Deviate from the Line

- Data is not normally distributed.
- The dataset may contain outliers.
- The distribution may be positively or negatively skewed.
- Data transformation (such as Box-Cox) may be required.

---

# 📌 Advantages

- Easy to understand.
- Detects normality visually.
- Identifies skewness.
- Helps detect outliers.
- Useful before regression and hypothesis testing.

---

# ✅ Conclusion

The Q-Q Plot provides a simple and effective visual method for checking whether transaction amounts follow a normal distribution. Based on the position of the plotted points, we can determine whether the data is suitable for parametric statistical analysis or if transformation techniques should be applied.

---

---

# 5️⃣ Task 5 – Apply Box-Cox Transformation

## 📖 Explanation

The **Box-Cox Transformation** is a statistical technique used to transform non-normal data into a distribution that is closer to normal. Many statistical models assume that the data is normally distributed and has constant variance. If the dataset is highly skewed, the Box-Cox transformation helps stabilize the variance and reduce skewness.

In this project, the Box-Cox transformation is applied to the transaction amounts to improve the distribution of the data before performing further statistical analysis.

---

# 🎯 Objective

- Reduce skewness in the dataset.
- Stabilize the variance.
- Improve data normality.
- Prepare the data for statistical analysis.
- Improve model performance.

---

# 🌍 Real-World Applications

- Financial Data Analysis
- Machine Learning
- Regression Analysis
- Medical Research
- Banking Analytics

---

# 📐 Formula

The Box-Cox Transformation is defined as:

For λ ≠ 0

$$
Y=\frac{X^\lambda-1}{\lambda}
$$

For λ = 0

$$
Y=\ln(X)
$$

Where:

- **X** = Original data
- **Y** = Transformed data
- **λ (Lambda)** = Transformation parameter

---

# 💻 Python Code

```python
positive = amt + 1

transformed, lamda = boxcox(positive)
print("Optimal Lambda =", lamda)

plt.figure(figsize=(12,5))
plt.subplot(1,2,1)
plt.hist(amt, bins=30, color='skyblue')
plt.title("Original Data")

plt.subplot(1,2,2)
plt.hist(transformed, bins=30, color='green')
plt.title("After Box-Cox Transformation")

plt.show()
```

---

# 📸 Output Screenshot

> <img width="1222" height="563" alt="Screenshot 2026-07-01 120106" src="https://github.com/user-attachments/assets/3067c6a8-bb99-4832-91fc-c16e3330a71e" />





---

# 📊 Interpretation

- Before transformation, the transaction data may be highly right-skewed.
- After applying the Box-Cox transformation, the distribution becomes more symmetric.
- The variance is stabilized across the dataset.
- Statistical models that assume normality can perform more effectively on the transformed data.

---

# 📌 Advantages

- Reduces skewness.
- Improves normality.
- Stabilizes variance.
- Enhances statistical model performance.
- Produces more reliable analytical results.

---

# ✅ Conclusion

The Box-Cox Transformation improves the quality of the dataset by reducing skewness and making the data closer to a normal distribution. This transformation allows statistical tests and predictive models to produce more accurate and reliable results.

---

---

# 6️⃣ Task 6 – Calculate Z-Scores and Compute the Probability of Transactions Exceeding ₹5000

## 📖 Explanation

In this task, the **Z-Score** is calculated to determine how far each transaction amount is from the dataset's mean in terms of standard deviations. Z-Scores help identify unusual observations (outliers) and compare different transaction values on a common scale.

After calculating the Z-Score, the probability of a transaction amount exceeding **₹5000** is computed using the Normal Distribution. This helps estimate how likely high-value transactions are within the dataset.

---

# 🎯 Objective

- Calculate the Z-Score for transaction amounts.
- Identify outliers in the dataset.
- Standardize the transaction values.
- Calculate the probability of transactions exceeding ₹5000.
- Interpret the statistical significance of the results.

---

# 🌍 Real-World Applications

- 💳 Fraud Detection
- 🏦 Banking & Finance
- 📊 Risk Analysis
- 📈 Business Intelligence
- 🤖 Machine Learning

---

# 📐 Formula

### Z-Score Formula

$$
Z=\frac{X-\mu}{\sigma}
$$

Where:

- **X** = Transaction Amount
- **μ** = Mean Transaction Amount
- **σ** = Standard Deviation

---

### Probability

$$
P(X>5000)=1-\Phi(Z)
$$

Where:

- **Φ(Z)** = Cumulative Distribution Function (CDF)

---

# 💻 Python Code

```python
# Calculate Z-Score

df["Z_score"] = zscore(amt)

print(df[["transaction_amount","Z_score"]].head())

# Probability of transaction amount > ₹5000

mean = amt.mean()
std = amt.std()

prob = 1-norm.cdf(5000, loc=mean, scale=std)

print("Probability of transaction Amount > ₹5000:", prob)
```

---

# 📸 Output Screenshot

> <img width="632" height="178" alt="Screenshot 2026-07-01 120244" src="https://github.com/user-attachments/assets/5b2361d2-36fc-4c88-b27e-f9c13c6de38d" />




---

# 📊 Interpretation

- A **positive Z-Score** indicates the transaction amount is above the mean.
- A **negative Z-Score** indicates the transaction amount is below the mean.
- Large positive or negative Z-Scores may represent outliers.
- The calculated probability shows how likely a transaction amount greater than ₹5000 is under the fitted normal distribution.

---

# 📌 Advantages

- Standardizes different values.
- Detects outliers efficiently.
- Supports probability calculations.
- Improves statistical interpretation.
- Useful for anomaly detection.

---

# ✅ Conclusion

The Z-Score analysis standardizes transaction amounts and helps identify unusually high or low transactions. By calculating the probability of transactions exceeding ₹5000, the analysis provides valuable insights into the occurrence of high-value transactions and supports risk assessment and decision-making.

---

---

# 7️⃣ Task 7 – Plot and Interpret the Probability Density Function (PDF) and Cumulative Distribution Function (CDF)

## 📖 Explanation

In this task, the **Probability Density Function (PDF)** and **Cumulative Distribution Function (CDF)** are plotted to understand the probability distribution of transaction amounts.

The **Probability Density Function (PDF)** describes how the probability of transaction amounts is distributed across different values. It helps identify where the data is concentrated and which transaction values are most likely to occur.

The **Cumulative Distribution Function (CDF)** represents the cumulative probability that a transaction amount is less than or equal to a specific value. It is useful for calculating probabilities, percentiles, and understanding the cumulative behavior of the dataset.

By visualizing both PDF and CDF, we gain a complete understanding of the distribution and probability characteristics of the transaction data.

---

# 🎯 Objective

- Plot the Probability Density Function (PDF).
- Plot the Cumulative Distribution Function (CDF).
- Understand the probability distribution of transaction amounts.
- Compare density and cumulative probability.
- Interpret transaction probabilities.

---

# 🌍 Real-World Applications

- 📊 Financial Risk Analysis
- 💳 Banking & Payment Systems
- 📈 Investment Analysis
- 📦 Inventory Management
- 🤖 Machine Learning
- 📉 Statistical Forecasting

---

# 📐 Mathematical Formula

## Probability Density Function (PDF)

$$
f(x)=\frac{1}{\sigma\sqrt{2\pi}}
e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

Where:

- **μ** = Mean
- **σ** = Standard Deviation

---

## Cumulative Distribution Function (CDF)

$$
F(x)=P(X\le x)
$$

For a normal distribution,

$$
F(x)=\int_{-\infty}^{x}f(t)\,dt
$$

---

# 💻 Python Code

```python
x = np.linspace(amt.min(), amt.max(), 500)
# PDF 

pdf = norm.pdf(x, mean, std)

plt.figure(figsize=(8,5))
plt.plot(x, pdf, color = "blue")
plt.title("Probability Density Funcation (PDF)")
plt.xlabel("Transaction Amount")
plt.ylabel("Density")
plt.grid(True)
plt.show()

## CDF

cdf = norm.cdf(x,mean,std)

plt.figure(figsize=(8,5))
plt.plot(x, cdf, color = "green")
plt.title("cumulative Distribution Function (CDF)")
plt.xlabel("Transaction Amount")
plt.ylabel("cumulative")
plt.grid(True)
plt.show()
```

---

# 📸 Output Screenshot

### 📈 Probability Density Function

><img width="922" height="587" alt="image" src="https://github.com/user-attachments/assets/e505ba0a-4489-41d9-aa80-cee6d554e17f" />



---

### 📊 Cumulative Distribution Function

> <img width="862" height="590" alt="image" src="https://github.com/user-attachments/assets/8f8cf7ad-b69a-4ed5-abfd-c0165b49b387" />



---

# 📊 Interpretation

### PDF

- Shows where transaction amounts are most concentrated.
- The highest point of the curve represents the most probable transaction values.
- The total area under the curve equals **1**, representing the total probability.

### CDF

- Shows the cumulative probability up to a given transaction amount.
- Starts at **0** and gradually increases to **1**.
- Helps estimate the probability that a transaction amount is less than or equal to a specific value.

---

# 📌 Difference Between PDF and CDF

| PDF | CDF |
|-----|-----|
| Shows probability density | Shows cumulative probability |
| Describes the shape of the distribution | Describes accumulated probability |
| Area under the curve equals probability | Values range from 0 to 1 |
| Used to understand likelihood | Used to calculate cumulative probabilities |

---

# ✅ Conclusion

The PDF and CDF provide complementary views of the transaction data. While the PDF highlights the likelihood of different transaction values, the CDF shows the cumulative probability of observing values up to a specified amount. Together, they help in understanding the distribution and support better statistical decision-making.

---

---

# 8️⃣ Task 8 – Conclude Which Distribution Best Fits the Dataset

## 📖 Explanation

After applying multiple statistical distributions and analysis techniques, the final step is to determine which probability distribution best represents the transaction dataset. This conclusion is based on the graphical analysis, statistical interpretation, and the overall behavior of the data observed throughout the previous tasks.

Different distributions are suitable for different types of data. By comparing Bernoulli, Binomial, Poisson, Log-Normal, and Power Law distributions along with the Q-Q Plot, Box-Cox Transformation, Z-Score Analysis, PDF, and CDF, we can identify the most appropriate statistical model for the dataset.

---

# 🎯 Objective

- Compare all fitted probability distributions.
- Evaluate the distribution that best represents the dataset.
- Summarize the statistical analysis.
- Interpret the final findings.
- Recommend the most suitable probability distribution.

---

# 📊 Comparison of Distributions

| Distribution | Best Used For | Suitable for this Project |
|--------------|---------------|---------------------------|
| Bernoulli | Binary outcomes | ✔ Yes |
| Binomial | Fixed number of trials | ✔ Yes |
| Poisson | Event counts over time | ✔ Yes |
| Log-Normal | Positive, right-skewed values | ✔ Yes |
| Power Law | Heavy-tailed data | ✔ Depends on the data |
| Normal Distribution | Symmetric continuous data | ✔ If Q-Q Plot indicates normality |

---



---

# 📸 Output Screenshot

><img width="1620" height="97" alt="image" src="https://github.com/user-attachments/assets/dd220c8b-8952-4c0b-9c85-77bf4bb890f8" />




---

# 📊 Interpretation

- Compare the fitted distributions based on the generated plots and statistical measures.
- Explain which distribution most closely follows the transaction data.
- Mention whether the Q-Q Plot supports normality.
- Describe the effect of the Box-Cox Transformation.
- Summarize the findings from the Z-Score, PDF, and CDF analyses.

---

# 📝 Final Conclusion

Based on the analysis performed in this project, the selected probability distribution provides the best representation of the transaction dataset. The visualizations, statistical calculations, and probability models help explain the characteristics of the data and support informed decision-making.

The project demonstrates how different statistical distributions can be applied to real-world datasets to understand data behavior, identify patterns, detect outliers, and improve analytical accuracy.

---

# 🎥 Project Demonstration

Watch the project demonstration video here:

📺 **Video**

👉 ## 🎥 Project Video

[▶️ Watch the Video](https://drive.google.com/file/d/1SfTIwlRLbuq-pSZqQPZB_3Ku4K8ceJvC/view?usp=sharing)

# 👨‍💻 Author

**Darshil**

- 🎓 Statistical Distribution Analysis Project
- 🐍 Python | Jupyter Notebook | Data Analysis
- 📊 GitHub Portfolio Project

If you found this project helpful, don't forget to ⭐ star the repository!
