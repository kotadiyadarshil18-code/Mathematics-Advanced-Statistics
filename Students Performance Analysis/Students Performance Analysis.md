<div align="center">

# 📊 Mathematics & Advanced Statistics – Part B

### 🚀 A Complete Statistical Analysis & Linear Algebra Project Using Python

<img src="https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python">
<img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter">
<img src="https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas">
<img src="https://img.shields.io/badge/NumPy-Mathematics-blue?style=for-the-badge&logo=numpy">
<img src="https://img.shields.io/badge/Matplotlib-Visualization-success?style=for-the-badge">
<img src="https://img.shields.io/badge/Statistics-Advanced-red?style=for-the-badge">

---

A comprehensive project demonstrating **Descriptive Statistics**, **Probability**, **Distribution Analysis**, **Data Visualization**, and **Linear Algebra** using Python and Jupyter Notebook.

⭐ **If you found this project useful, don't forget to Star this Repository!**

</div>

---

# 📑 Table of Contents

- 📖 Project Overview
- 🎯 Objectives
- ✨ Features
- 🛠 Technologies Used
- 📂 Dataset Information
- 📊 Project Workflow
- 📁 Project Structure
- 🔗 Previous Project (Part A)
- 🎥 Project Demonstration Video
- 📚 Code Explanation
- 📈 Results
- 🎓 Learning Outcomes
- 🚀 Future Improvements
- 📦 Requirements
- 👨‍💻 Author
- 📄 License

---

# 📖 Project Overview

This repository presents **Part B** of the *Mathematics & Advanced Statistics* project. It focuses on applying statistical methods, probability concepts, distribution analysis, and linear algebra techniques to a real-world student performance dataset.

The project demonstrates how mathematical and statistical theories can be applied using Python to analyze academic performance, identify patterns, and visualize insights. Every concept is implemented with Python code, mathematical formulas, detailed explanations, and interpretations, making the notebook suitable for both academic learning and portfolio presentation.

---

# 🎯 Objectives

The primary objectives of this project are:

- Perform descriptive statistical analysis.
- Calculate measures of central tendency.
- Calculate measures of dispersion.
- Apply probability and conditional probability concepts.
- Visualize data distributions.
- Analyze skewness and kurtosis.
- Generate Q-Q plots for normality analysis.
- Perform vector operations using Linear Algebra.
- Strengthen Python programming and data analysis skills.

---

# ✨ Features

✔ Measures of Central Tendency

✔ Measures of Dispersion

✔ Probability Analysis

✔ Conditional Probability

✔ Contingency Table

✔ Histogram

✔ Normal Distribution Curve

✔ Skewness

✔ Kurtosis

✔ Q-Q Plot

✔ Vector Representation

✔ Dot Product

✔ L1 Norm

✔ L2 Norm

✔ Angle Between Vectors

✔ Well Documented Code

✔ Mathematical Formula for Every Concept

✔ Beginner Friendly Explanations

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| Jupyter Notebook | Development Environment |
| Pandas | Data Processing |
| NumPy | Mathematical Operations |
| Matplotlib | Data Visualization |
| SciPy | Statistical Functions |
| Seaborn | Advanced Visualization |
| Statsmodels | Q-Q Plot Analysis |

---

# 📂 Dataset Information

**Dataset Name**

> Student_Performance.csv

The dataset contains academic information of students and includes variables such as:

- Mathematics Score
- Science Score
- English Score
- Study Hours
- Attendance
- Pass/Fail Status

The dataset is used to demonstrate descriptive statistics, probability calculations, visualization techniques, and linear algebra operations on real-world educational data.

---

# 📊 Project Workflow

```text
Start
   │
   ▼
Import Required Libraries
   │
   ▼
Load Dataset
   │
   ▼
Data Understanding
   │
   ▼
Measures of Central Tendency
   │
   ▼
Measures of Dispersion
   │
   ▼
Probability Analysis
   │
   ▼
Distribution Analysis
   │
   ▼
Linear Algebra Operations
   │
   ▼
Visualization
   │
   ▼
Results & Interpretation
   │
   ▼
End
```

---

# 📁 Project Structure

```text
Mathematics-Advanced-Statistics-Part-B/

│── Statistics Foundation.ipynb
│── Student_Performance.csv
│── README.md
│── requirements.txt
│── LICENSE
│── .gitignore
```

---

# 🔗 Previous Project (Part A)

This project is a continuation of **Part A**.

📂 **GitHub Repository (Part A)**

👉 https://docs.google.com/document/d/1jWQw_ODoGXYQS7oq4cchb9jAz5xwBHjeyT3s7LapYcE/edit?usp=sharing

Part A focuses on mathematical foundations and introductory statistical concepts, while Part B extends those concepts into probability, visualization, and advanced linear algebra applications.

---

# 🎥 Project Demonstration Video

Watch the complete explanation of **Part B** here.

📺 **Project Video**

👉 https://drive.google.com/file/d/1SfTIwlRLbuq-pSZqQPZB_3Ku4K8ceJvC/view?usp=sharing

The video includes:

- Project Overview
- Dataset Explanation
- Code Walkthrough
- Statistical Analysis
- Probability Concepts
- Linear Algebra Operations
- Visualizations
- Final Results

  # 📚 Code Explanation

---

# 📌 Step 1: Measures of Central Tendency & Dispersion

Measures of Central Tendency and Dispersion are fundamental statistical techniques used to summarize and understand the characteristics of a dataset. In this project, these measures are applied to the **Mathematics Scores** of students to analyze their academic performance.

---

# Question 1: Calculate Mean

## 💻 Code

```python
mean_math = df["Math_score"].mean()

print("Mean:", mean_math)
```

## 📝 Explanation

- Calculated the **Mean** of the Mathematics scores.
- The mean represents the average score obtained by all students.
- It is one of the most widely used measures of central tendency.
- The mean provides a single value that summarizes the overall performance of the dataset.

## 📐 Mathematical Formula

$$
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}
$$

### Where

- $\bar{x}$ = Mean
- $x_i$ = Individual observation
- $n$ = Total number of observations

## 📊 Interpretation

The mean represents the average Mathematics score of all students. A higher mean indicates better overall academic performance.

---

# Question 2: Calculate Median

## 💻 Code

```python
median_math = df["Math_score"].median()

print("Median:", median_math)
```

## 📝 Explanation

- Calculated the **Median** of Mathematics scores.
- The median is the middle value after arranging all observations in ascending order.
- Unlike the mean, it is not affected by extreme values (outliers).

## 📐 Mathematical Formula

For Odd Number of Observations

$$
Median=x_{\frac{n+1}{2}}
$$

For Even Number of Observations

$$
Median=\frac{x_{\frac n2}+x_{\frac n2+1}}{2}
$$

## 📊 Interpretation

The median divides the dataset into two equal halves. It is a better measure of central tendency when the dataset contains outliers.

---

# Question 3: Calculate Mode

## 💻 Code

```python
mode_math = df["Math_score"].mode()[0]

print("Mode:", mode_math)
```

## 📝 Explanation

- Calculated the **Mode** of Mathematics scores.
- The mode is the value that occurs most frequently in the dataset.
- A dataset may contain one mode, multiple modes, or no mode.

## 📐 Mathematical Formula

$$
Mode = Most\ Frequent\ Observation
$$

## 📊 Interpretation

The mode identifies the score obtained by the highest number of students.

---

# Question 4: Calculate Range

## 💻 Code

```python
range_math = df["Math_score"].max() - df["Math_score"].min()

print("Range:", range_math)
```

## 📝 Explanation

- Calculated the **Range** of Mathematics scores.
- The range measures the spread of the dataset.
- It is the difference between the highest and lowest score.

## 📐 Mathematical Formula

$$
Range = Maximum - Minimum
$$

## 📊 Interpretation

A larger range indicates greater variation in students' Mathematics scores.

---

# Question 5: Calculate Variance

## 💻 Code

```python
variance_math = df["Math_score"].var()

print("Variance:", variance_math)
```

## 📝 Explanation

- Calculated the **Variance** of Mathematics scores.
- Variance measures how far the observations are spread from the mean.
- A larger variance indicates greater variability among student scores.

## 📐 Mathematical Formula

For Sample Variance

$$
s^2=\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}
$$

### Where

- $s^2$ = Sample Variance
- $x_i$ = Individual Observation
- $\bar{x}$ = Mean
- $n$ = Number of Observations

## 📊 Interpretation

Higher variance means the Mathematics scores are more dispersed, whereas lower variance indicates that the scores are clustered closer to the mean.

---

# Question 6: Calculate Standard Deviation

## 💻 Code

```python
std_math = df["Math_score"].std()

print("Standard Deviation:", std_math)
```

## 📝 Explanation

- Calculated the **Standard Deviation** of Mathematics scores.
- Standard deviation is the square root of variance.
- It measures the average distance of observations from the mean.
- It is one of the most important measures of dispersion in statistics.

## 📐 Mathematical Formula

$$
s=\sqrt{\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}}
$$

### Where

- $s$ = Standard Deviation
- $x_i$ = Individual Observation
- $\bar{x}$ = Mean
- $n$ = Number of Observations

## 📊 Interpretation

A smaller standard deviation indicates that the Mathematics scores are close to the average score, while a larger standard deviation indicates greater variability among students.

---

# 📈 Summary of Step 1

The following statistical measures were successfully calculated:

- ✔ Mean
- ✔ Median
- ✔ Mode
- ✔ Range
- ✔ Variance
- ✔ Standard Deviation

These measures provide a comprehensive understanding of the central tendency and variability of students' Mathematics scores, forming the foundation for further statistical analysis in the project.

---
# 📚 Step 2: Probability Basics

Probability is a branch of mathematics that measures the likelihood of an event occurring. In this section, probability concepts are applied to analyze the student performance dataset.

---

# Question 1: Probability of Passing

## 💻 Code

```python
print("========== Probability of Passing ==============")
prob_pass = (df["pass_fail"] == 1).mean()
print(f"Probability of Passing: {prob_pass}")
```

---

## 📝 Explanation

- Selected all students whose **Pass/Fail status is equal to 1 (Pass)**.
- Counted the total number of students who passed.
- Divided this value by the total number of students in the dataset.
- The result represents the probability that a randomly selected student has passed.

---

## 📐 Mathematical Formula

$$
P(A)=\frac{n(A)}{n(S)}
$$

Where,

- $P(A)$ = Probability of Event A
- $n(A)$ = Number of Favorable Outcomes
- $n(S)$ = Total Number of Outcomes

---

## 📊 Interpretation

The calculated probability indicates the likelihood that a randomly selected student from the dataset has successfully passed.

A higher probability value indicates that a greater proportion of students have passed.

---

# Question 2: Contingency Table

## 💻 Code

```python
print("========== Contingency Table ==============")
df["Hours_Studied_GT5"] = df["Hours_studied"] > 5 
cont_table = pd.crosstab(df["pass_fail"],
                         df["Hours_Studied_GT5"])
print(cont_table)
```

---

## 📝 Explanation

- Created a contingency table using the **Attendance** and **Pass/Fail** columns.
- The table summarizes the frequency distribution of two categorical variables.
- It helps identify relationships between attendance and examination performance.

---

## 📐 Mathematical Formula

For two categorical variables,

$$
C_{ij}=Frequency(X_i,Y_j)
$$

Where,

- $X$ = Attendance Category
- $Y$ = Pass/Fail Category

---

## 📊 Interpretation

The contingency table helps determine whether students with better attendance have a higher probability of passing.

It provides an easy comparison between attendance levels and academic outcomes.

---

# Question 3: Conditional Probability

## 💻 Code

```python
print("========== Conditional Probability ==============")
Student = df[df["Hours_studied"]> 5]
passed = Student[Student["pass_fail"] == 1]
conditional_prob = len(passed)/len(Student)
print(f"P(pass | Hours_studied > 5)= {conditional_prob}")
```

---

## 📝 Explanation

- Selected students who studied for more than **5 hours**.
- Counted the number of students who both studied more than five hours and passed.
- Divided this count by the total number of students who studied more than five hours.
- This calculates the probability of passing given that a student studied for more than five hours.

---

## 📐 Mathematical Formula

$$
P(A|B)=\frac{P(A\cap B)}{P(B)}
$$

Where,

- $A$ = Student Passed
- $B$ = Student Studied More Than 5 Hours

---

## 📊 Interpretation

Conditional probability measures the likelihood that a student passes **given** that the student has studied for more than five hours.

If the conditional probability is high, it suggests that studying for more than five hours is associated with better academic performance.

---

# 📌 Real-World Applications

Probability concepts are widely used in:

- Student Performance Analysis
- Machine Learning
- Medical Diagnosis
- Financial Risk Analysis
- Weather Forecasting
- Recommendation Systems
- Decision Making
- Artificial Intelligence

---

# 📈 Summary of Step 2

The following probability concepts were successfully implemented:

✔ Probability of Passing

✔ Contingency Table

✔ Conditional Probability

✔ Statistical Interpretation

✔ Real-world Probability Analysis

These concepts help quantify uncertainty and analyze relationships between study habits, attendance, and student performance.

---

# 📚 Step 3: Distribution & Visualization

Data visualization helps us understand the distribution, spread, and shape of the dataset. In this section, various graphical and statistical techniques are used to analyze the distribution of students' Mathematics scores.

---

# Question 1: Histogram

## 💻 Code

```python
plt.figure(figsize=(8,5))
plt.hist(df["Math_score"], bins=10, edgecolor="black")

plt.title("Distribution of Mathematics Scores")
plt.xlabel("Math Score")
plt.ylabel("Frequency")

plt.show()
```

---

## 📝 Explanation

- Created a Histogram to visualize the distribution of Mathematics scores.
- Each bar represents the number of students within a particular score interval.
- The histogram helps identify whether the data is normally distributed, positively skewed, or negatively skewed.

---

## 📐 Mathematical Formula

The histogram represents the empirical frequency distribution:

$$
Frequency_i = Number\ of\ observations\ in\ Class_i
$$

where,

- $Frequency_i$ = Number of observations in the i-th class interval.

---

## 📊 Interpretation

The histogram shows how Mathematics scores are distributed across different score ranges.

A symmetric histogram indicates an approximately normal distribution, while an asymmetric histogram suggests skewness.

---

# Question 2: Histogram with Normal Distribution Curve

## 💻 Code

```python
from scipy.stats import norm

plt.figure(figsize=(8,5))

sns.histplot(
    df["Math_score"],
    kde=False,
    stat="density",
    bins=10
)

x = np.linspace(
    df["Math_score"].min(),
    df["Math_score"].max(),
    100
)

plt.plot(
    x,
    norm.pdf(
        x,
        df["Math_score"].mean(),
        df["Math_score"].std()
    ),
    linewidth=2
)

plt.title("Histogram with Normal Distribution")
plt.show()
```

---

## 📝 Explanation

- Created a histogram of Mathematics scores.
- Plotted the theoretical Normal Distribution Curve using the dataset's mean and standard deviation.
- Compared the actual distribution with the ideal normal distribution.

---

## 📐 Mathematical Formula

Normal Distribution

$$
f(x)=\frac{1}{\sigma\sqrt{2\pi}}
e^{-\frac{(x-\mu)^2}{2\sigma^2}}
$$

Where,

- $\mu$ = Mean
- $\sigma$ = Standard Deviation

---

## 📊 Interpretation

If the histogram closely follows the normal curve, the data is approximately normally distributed.

Significant deviations from the curve indicate skewness or unusual data patterns.

---

# Question 3: Calculate Skewness

## 💻 Code

```python
skewness = df["Math_score"].skew()

print("Skewness:", skewness)
```

---

## 📝 Explanation

- Calculated the Skewness of Mathematics scores.
- Skewness measures the asymmetry of the data distribution.

---

## 📐 Mathematical Formula

$$
Skewness=
\frac{
\sum(x_i-\bar{x})^3
}
{
(n-1)s^3
}
$$

Where,

- $x_i$ = Observation
- $\bar{x}$ = Mean
- $s$ = Standard Deviation

---

## 📊 Interpretation

- **Skewness = 0** → Perfectly Symmetric Distribution

- **Skewness > 0** → Positively Skewed Distribution

- **Skewness < 0** → Negatively Skewed Distribution

The calculated skewness helps determine whether students' scores are evenly distributed or concentrated toward higher or lower values.

---

# Question 4: Calculate Kurtosis

## 💻 Code

```python
kurtosis = df["Math_score"].kurt()

print("Kurtosis:", kurtosis)
```

---

## 📝 Explanation

- Calculated the Kurtosis of Mathematics scores.
- Kurtosis measures the peakedness and tail heaviness of the distribution.

---

## 📐 Mathematical Formula

$$
Kurtosis=
\frac{
\sum(x_i-\bar{x})^4
}
{
(n-1)s^4
}
-3
$$

---

## 📊 Interpretation

- **Kurtosis = 0** → Normal Distribution

- **Kurtosis > 0** → Heavy Tails (Leptokurtic)

- **Kurtosis < 0** → Light Tails (Platykurtic)

This metric indicates whether the dataset contains more extreme values than a normal distribution.

---

# Question 5: Q-Q Plot

## 💻 Code

```python
from scipy import stats

stats.probplot(
    df["Math_score"],
    dist="norm",
    plot=plt
)

plt.title("Q-Q Plot")

plt.show()
```

---

## 📝 Explanation

- Generated a Quantile-Quantile (Q-Q) Plot.
- Compared the Mathematics score distribution with the theoretical normal distribution.
- Used to evaluate whether the dataset follows normality.

---

## 📐 Mathematical Concept

A Q-Q Plot compares:

$$
Observed\ Quantiles
\quad vs \quad
Theoretical\ Quantiles
$$

If

$$
Observed \approx Theoretical
$$

then

$$
Data \ follows \ Normal \ Distribution
$$

---

## 📊 Interpretation

If the plotted points lie close to the reference line, the data is approximately normally distributed.

Large deviations from the line indicate departures from normality.

---

# 🌍 Real-World Applications

Distribution analysis is widely used in:

- Machine Learning
- Data Science
- Financial Analysis
- Medical Research
- Business Intelligence
- Quality Control
- Artificial Intelligence
- Predictive Analytics

---

# 📈 Summary of Step 3

The following distribution analysis techniques were successfully implemented:

✔ Histogram

✔ Normal Distribution Curve

✔ Skewness

✔ Kurtosis

✔ Q-Q Plot

✔ Statistical Interpretation

✔ Distribution Analysis

These techniques provide a deeper understanding of the shape, spread, and normality of the student performance dataset.

---
# 📚 Step 4: Linear Algebra

Linear Algebra is one of the most important branches of mathematics used in Data Science, Machine Learning, Artificial Intelligence, Computer Vision, and Scientific Computing.

In this section, the students' Mathematics and Science scores are represented as vectors, and several vector operations are performed to analyze their mathematical relationship.

---

# Question 1: Represent Student Scores as Vectors

## 💻 Code

```python
math_vec = df["Math_score"].head().values
science_vec = df["Science_score"].head().values

print("Math Vector :", math_vec)
print("Science Vector :", science_vec)
```

---

## 📝 Explanation

- Selected the first five Mathematics scores.
- Selected the first five Science scores.
- Converted both columns into NumPy vectors.
- These vectors are used for Linear Algebra operations.

---

## 📐 Mathematical Representation

Let,

$$
\mathbf{A}=
\begin{bmatrix}
a_1\\
a_2\\
a_3\\
a_4\\
a_5
\end{bmatrix}
$$

and

$$
\mathbf{B}=
\begin{bmatrix}
b_1\\
b_2\\
b_3\\
b_4\\
b_5
\end{bmatrix}
$$

represent the Mathematics and Science score vectors.

---

## 📊 Interpretation

Each student's score is represented as a vector. This allows mathematical operations such as similarity measurement, vector length calculation, and angle computation.

---

# Question 2: Dot Product

## 💻 Code

```python
dot_product = np.dot(math_vec, science_vec)

print("Dot Product :", dot_product)
```

---

## 📝 Explanation

- Calculated the Dot Product between the Mathematics and Science vectors.
- The Dot Product measures how similar two vectors are.
- It is widely used in Machine Learning and Recommendation Systems.

---

## 📐 Mathematical Formula

$$
A \cdot B
=
\sum_{i=1}^{n}
A_iB_i
$$

or

$$
A\cdot B
=
A_1B_1+A_2B_2+\cdots+A_nB_n
$$

---

## 📊 Interpretation

A larger Dot Product indicates that both vectors point in similar directions, suggesting similar patterns between Mathematics and Science scores.

---

# Question 3: L1 Norm

## 💻 Code

```python
l1_norm = np.linalg.norm(math_vec, ord=1)

print("L1 Norm :", l1_norm)
```

---

## 📝 Explanation

- Calculated the L1 Norm of the Mathematics score vector.
- L1 Norm is also known as the Manhattan Norm.
- It is the sum of the absolute values of all vector components.

---

## 📐 Mathematical Formula

$$
||A||_1
=
\sum_{i=1}^{n}|A_i|
$$

---

## 📊 Interpretation

The L1 Norm represents the total magnitude of the Mathematics score vector.

Higher values indicate a greater combined score.

---

# Question 4: L2 Norm

## 💻 Code

```python
l2_norm = np.linalg.norm(math_vec)

print("L2 Norm :", l2_norm)
```

---

## 📝 Explanation

- Calculated the Euclidean length of the Mathematics vector.
- L2 Norm measures the actual distance of the vector from the origin.
- It is the most commonly used vector norm.

---

## 📐 Mathematical Formula

$$
\|A\|_2 =
\sqrt{\sum_{i=1}^{n} A_i^2}
$$

---

## 📊 Interpretation

The L2 Norm measures the overall magnitude of the Mathematics score vector using Euclidean distance.

---

# Question 5: Angle Between Two Vectors

## 💻 Code

```python
cos_theta = dot_product / (
    np.linalg.norm(math_vec) *
    np.linalg.norm(science_vec)
)

angle = np.degrees(np.arccos(cos_theta))

print("Angle :", angle)
```

---

## 📝 Explanation

- Calculated the cosine of the angle using the Dot Product.
- Converted the cosine value into degrees.
- Measured the similarity between Mathematics and Science vectors.

---

## 📐 Mathematical Formula

First,

$$
\cos(\theta)=
\frac{A \cdot B}
{\|A\|_2 \times \|B\|_2}
$$
Then,

$$
\theta=
\cos^{-1}
\left(
\frac{A \cdot B}
{\|A\|_2 \times \|B\|_2}
\right)
$$
---

## 📊 Interpretation

- Small Angle → High Similarity
- Large Angle → Low Similarity

If the calculated angle is close to **0°**, the Mathematics and Science scores follow a similar pattern.

---

# 🌍 Real-World Applications

Linear Algebra is extensively used in:

- Machine Learning
- Artificial Intelligence
- Data Science
- Computer Vision
- Robotics
- Recommendation Systems
- Natural Language Processing
- Image Processing
- Deep Learning

---

# 📈 Summary of Step 4

Successfully implemented:

✔ Student Score Vectors

✔ Dot Product

✔ L1 Norm

✔ L2 Norm

✔ Angle Between Vectors

✔ Vector Mathematics

✔ Linear Algebra Concepts

✔ Mathematical Interpretation

The implementation demonstrates how vector operations can be applied to real-world student performance data for similarity analysis and mathematical computation.

---
---

# 📊 Results

The project successfully demonstrates the practical implementation of **Descriptive Statistics**, **Probability**, **Distribution Analysis**, and **Linear Algebra** using Python.

The statistical techniques were applied to the Student Performance dataset to analyze academic performance and identify meaningful insights.

## 📌 Key Results

- Successfully calculated the **Mean, Median, and Mode** of Mathematics scores.
- Measured the spread of the dataset using **Range, Variance, and Standard Deviation**.
- Computed the **Probability of Passing** students.
- Created a **Contingency Table** to analyze the relationship between Attendance and Pass/Fail status.
- Calculated **Conditional Probability** for students studying more than five hours.
- Visualized the distribution of Mathematics scores using a **Histogram**.
- Compared the dataset with the **Normal Distribution Curve**.
- Measured the **Skewness** and **Kurtosis** of the dataset.
- Verified data normality using a **Q-Q Plot**.
- Represented student scores as mathematical vectors.
- Calculated the **Dot Product** between Mathematics and Science vectors.
- Computed **L1 Norm** and **L2 Norm** of score vectors.
- Determined the **Angle Between Vectors** to analyze similarity.

---

# 📊 Statistical Insights

The analysis revealed several important observations regarding student performance:

- The average Mathematics score represents the overall academic performance of the students.
- The median indicates the central score and is less affected by extreme values.
- Variance and Standard Deviation reveal the consistency of students' performance.
- Probability calculations provide insights into students' passing rates.
- Conditional Probability demonstrates the relationship between study hours and examination success.
- Distribution analysis helps determine whether the dataset follows a normal distribution.
- Linear Algebra techniques quantify the similarity between subject scores.

---

# 📈 Output Gallery

The project generates several statistical outputs and visualizations, including:

✔ Mean, Median & Mode

✔ Range, Variance & Standard Deviation

✔ Probability Calculations

✔ Contingency Table

✔ Conditional Probability

✔ Histogram

✔ Normal Distribution Curve

✔ Skewness

✔ Kurtosis

✔ Q-Q Plot

✔ Vector Representation

✔ Dot Product

✔ L1 Norm

✔ L2 Norm

✔ Angle Between Vectors

> 📸 **You can add screenshots of these outputs here for better visualization.**

Example:

```
images/

│── Mean_Output.png
│── Histogram.png
│── QQ_Plot.png
│── Probability_Output.png
│── Linear_Algebra_Output.png
```

---

# 🎓 Learning Outcomes

After completing this project, I gained practical knowledge of:

- Descriptive Statistics
- Measures of Central Tendency
- Measures of Dispersion
- Probability Theory
- Conditional Probability
- Distribution Analysis
- Data Visualization
- Linear Algebra
- Vector Mathematics
- Scientific Computing
- Python Programming
- NumPy
- Pandas
- Matplotlib
- SciPy
- Seaborn
- Statsmodels

---

# 🌍 Real-World Applications

The concepts implemented in this project are widely used in:

- Data Analytics
- Business Intelligence
- Artificial Intelligence
- Machine Learning
- Financial Analysis
- Medical Research
- Educational Analytics
- Risk Analysis
- Scientific Research
- Predictive Modeling

---

# 🚀 Future Improvements

This project can be further enhanced by adding:

- Interactive Dashboard using Streamlit
- Power BI Dashboard
- Student Performance Prediction using Machine Learning
- Correlation Heatmap
- Feature Engineering
- Statistical Hypothesis Testing
- Interactive Graphs using Plotly
- More Real-world Educational Datasets
- Model Evaluation Techniques
- Automated Report Generation

---

# 📦 Requirements

Install the required Python libraries before running the notebook.

```text
numpy
pandas
matplotlib
seaborn
scipy
statsmodels
scikit-learn
jupyter
```

or

```bash
pip install -r requirements.txt
```

---

# 📚 References

- Python Documentation
- NumPy Documentation
- Pandas Documentation
- Matplotlib Documentation
- SciPy Documentation
- Statsmodels Documentation
- Scikit-learn Documentation

---

# 👨‍💻 Author

## Darshil Kotadiya

**Aspiring Data Analyst | Python Developer | SQL | Power BI | Excel | Mathematics & Advanced Statistics**



---



---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use this repository for educational and learning purposes.

---

<div align="center">

# 🙏 Thank You for Visiting This Repository

### ⭐ If you enjoyed this project, please consider giving it a Star ⭐

## Happy Learning! 🚀

Made with ❤️ by **Darshil Kotadiya**

</div>
