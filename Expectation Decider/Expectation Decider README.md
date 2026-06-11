# 📊 Expectation Decider - Advanced Statistics & Probability Analysis

A comprehensive Jupyter notebook analyzing student exam performance through probability theory, statistical distributions, and Bayesian inference. This project applies real-world data to fundamental concepts in probability and statistics.

---

## 🎯 Project Overview

**Expectation Decider** is an educational resource that demonstrates key probability and statistics concepts using a real student dataset. It analyzes factors affecting exam success through:

- 🎲 **Probability Theory** - Basic concepts and applications
- 📈 **Probability Distributions** - Binomial distributions and random variables
- 🔗 **Conditional Probability** - Bayes' theorem and event relationships
- 📋 **Contingency Tables** - Joint and marginal probabilities
- 🎓 **Real-world Application** - Student exam performance analysis

---

<div align="center">
  <img width="280" height="280" alt="Popcorn GIF" src="https://github.com/user-attachments/assets/9ac5ad45-4830-4b30-b338-00a6fda5755f" />
</div>

---

## 📚 Table of Contents

1. [Key Concepts](#-key-concepts)
2. [Dataset Overview](#-dataset-overview)
3. [Analysis Sections](#-analysis-sections)
4. [Mathematical Formulas](#-mathematical-formulas)
5. [Key Findings](#-key-findings)
6. [Installation & Usage](#-installation--usage)
7. [Results Summary](#-results-summary)

---

## 🎓 Key Concepts

### 📌 1. Probability Basics

| Concept | Definition | Example |
|---------|-----------|---------|
| **Probability** | Measure of likelihood of an event occurring | P(Student Passes) = 0.605 |
| **Event** | A specific outcome or group of outcomes | Student getting a Pass grade |
| **Sample Space** | All possible outcomes | {Pass, Fail} |
| **Favorable Outcomes** | Outcomes we're interested in | 121 students who passed |

**Formula:**
$$P(E) = \frac{\text{Number of Favorable Outcomes}}{\text{Total Number of Outcomes}}$$

---

### 📊 2. Types of Probability

| Type | Definition | Formula | Example |
|------|-----------|---------|---------|
| **Empirical Probability** | Based on actual observed data | $P(E) = \frac{\text{Favorable Outcomes}}{\text{Total Outcomes}}$ | P(Pass) = 121/200 = 0.605 |
| **Theoretical Probability** | Based on mathematical theory | $P(E) = \frac{\text{Favorable Outcomes}}{\text{Total Outcomes}}$ | P(Heads) = 1/2 = 0.5 |

---

### 🔗 3. Event Relationships

| Relationship | Definition | Condition | Example |
|--------------|-----------|-----------|---------|
| **Independent Events** | Occurrence of one doesn't affect the other | $P(A \cap B) = P(A) \cdot P(B)$ | No correlation |
| **Dependent Events** | Occurrence of one affects the other | $P(A \cap B) \neq P(A) \cdot P(B)$ | Group Discussion & Pass |
| **Mutually Exclusive** | Events cannot occur together | $P(A \cap B) = 0$ | Pass and Fail |

---

### 🎲 4. Random Variables & Distributions

**Definition:** A random variable assigns numerical values to outcomes of a random experiment.

**Example:** Let X = number of students passing out of 3 randomly selected students
- X can take values: {0, 1, 2, 3}

#### Binomial Distribution (n=3 trials)

| X (Passes) | P(X) | Interpretation |
|-----------|------|-----------------|
| 0 | 0.0616 | All 3 fail |
| 1 | 0.2832 | Exactly 1 passes |
| 2 | 0.4337 | Exactly 2 pass |
| 3 | 0.2214 | All 3 pass |

**Mean Formula:**
$$\mu = n \cdot p = 3 \times 0.605 = 1.815$$

**Variance Formula:**
$$\sigma^2 = n \cdot p \cdot (1-p) = 3 \times 0.605 \times 0.395 = 0.717$$

**Binomial PMF:**
$$P(X = k) = \binom{n}{k} \cdot p^k \cdot (1-p)^{n-k}$$

---

### 📋 5. Contingency Table Analysis

#### Group Discussion vs Final Exam Pass

| | Pass ✅ | Fail ❌ | Total |
|---------|---------|---------|-------|
| **Group Discussion: Yes** | 75 | 43 | 118 |
| **Group Discussion: No** | 46 | 36 | 82 |
| **Total** | 121 | 79 | 200 |

**Key Probabilities:**
- $P(\text{Pass}) = \frac{121}{200} = 0.605$
- $P(\text{Yes}) = \frac{118}{200} = 0.59$
- $P(\text{Pass AND Yes}) = \frac{75}{200} = 0.375$

---

### 🧮 6. Conditional Probability

**Formula:**
$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

**Interpretation:** Probability of event A occurring given that event B has already occurred.

**Example - Pass given Group Discussion:**
$$P(\text{Pass} | \text{GD='Yes'}) = \frac{75}{118} = 0.636$$

This means: **63.6% of students who participated in group discussions passed the exam.**

---

### 🎯 7. Bayes' Theorem

**Formula:**
$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$

**Application Example:**
- P(High Attendance | Pass) = 0.70
- P(High Attendance | Fail) = 0.40  
- P(High Attendance) = 0.60

**Finding:** P(Pass | High Attendance) = 0.778

**Interpretation:** Students with high attendance have a **77.8% chance of passing** the exam.

---

## 📊 Dataset Overview

### Dataset Characteristics

| Attribute | Details |
|-----------|---------|
| **Total Records** | 200 students |
| **Time Period** | Single academic semester |
| **Data Source** | Student performance records |

### Features Analyzed

| Feature | Type | Range | Description |
|---------|------|-------|-------------|
| **study_hours** | Numeric | 6-18 hours/week | Weekly study time |
| **attendance** | Numeric | 55-78% | Class attendance percentage |
| **group_discussion** | Categorical | Yes/No | Participation in group study |
| **previous_test_score** | Numeric | 42-100 | Prior exam performance |
| **final_exam_pass** | Categorical | Pass/Fail | Target variable |

---

## 📈 Analysis Sections

### Section 1️⃣: Understanding the Basics

Calculate basic probabilities from the dataset:

```
✅ Probability of Student Studying >10 hrs/week: 0.54 (54%)
✅ Probability of Student Attendance >80%: 0.435 (43.5%)
✅ Probability of Student Passing Exam: 0.605 (60.5%)
```

---

### Section 2️⃣: Types of Events

**Empirical vs Theoretical Probabilities:**

| Type | Value | Method |
|------|-------|--------|
| Empirical P(Pass) | 0.605 | From actual data |
| Theoretical P(Heads) | 0.500 | Mathematical formula |

---

### Section 3️⃣: Random Variables & Probability Distributions

**Binomial Distribution Results (n=3, p=0.605):**

```
Mean (μ) = 1.815 students expected to pass
Variance (σ²) = 0.717
Standard Deviation (σ) = 0.847
```

---

### Section 4️⃣: Venn Diagram Probability

Visual representation of:
- **Set A:** Students studying >10 hours/week (n=108)
- **Set B:** Students with >80% attendance (n=87)
- **Overlap (A ∩ B):** Students meeting both conditions

---

### Section 5️⃣: Contingency Table & Joint Probability

Analyzes relationship between:
- **Group Discussion Participation** (Yes/No)
- **Exam Results** (Pass/Fail)

**Key Finding:** Students who participated in group discussions showed higher pass rates.

---

### Section 6️⃣: Conditional Probability & Event Relationships

**Test for Independence:**

```
P(Yes) = 0.59
P(Pass) = 0.605
P(Yes AND Pass) = 0.375

Expected if Independent: 0.59 × 0.605 = 0.357
Actual: 0.375
Result: ⚠️ DEPENDENT EVENTS
```

**Interpretation:** Group discussion participation and exam success are **dependent events**.

---

### Section 7️⃣: Bayes' Theorem Application

**Updated Probability Using New Information:**

```
Without knowing attendance:
  P(Pass) = 0.605 (60.5%)

Knowing student has high attendance:
  P(Pass | High Attendance) = 0.778 (77.8%)
```

---

## 📐 Mathematical Formulas

### Core Probability Formulas

#### 1. Basic Probability
$$P(E) = \frac{\text{Favorable Outcomes}}{\text{Total Outcomes}}$$

#### 2. Conditional Probability
$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

#### 3. Multiplication Rule (Dependent Events)
$$P(A \cap B) = P(A|B) \cdot P(B)$$

#### 4. Multiplication Rule (Independent Events)
$$P(A \cap B) = P(A) \cdot P(B)$$

#### 5. Addition Rule
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

#### 6. Bayes' Theorem
$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$

#### 7. Binomial Distribution
$$P(X = k) = \binom{n}{k} \cdot p^k \cdot (1-p)^{n-k}$$

#### 8. Mean of Binomial Distribution
$$\mu = n \cdot p$$

#### 9. Variance of Binomial Distribution
$$\sigma^2 = n \cdot p \cdot (1-p)$$

#### 10. Standard Deviation
$$\sigma = \sqrt{n \cdot p \cdot (1-p)}$$

---

## 🔍 Key Findings

### 🏆 Factors Affecting Exam Success

| Factor | Impact | Priority |
|--------|--------|----------|
| **High Attendance (>80%)** | +17.3% pass rate | 🥇 **Critical** |
| **Group Discussion** | +3.1% pass rate | 🥈 **High** |
| **Study Hours >10/week** | Positive correlation | 🥉 **Moderate** |
| **Prior Test Score** | Positive correlation | **Moderate** |

### 📊 Success Probability by Factors

| Condition | Pass Rate | Insight |
|-----------|-----------|---------|
| No Group Discussion | 56.1% | Lower success rate |
| With Group Discussion | 63.6% | **+7.5% improvement** |
| Low Attendance | ~50% | Critical risk factor |
| High Attendance | 77.8% | **Strongest predictor** |

### 💡 Key Insights

✅ **Insight 1:** Group discussion participation and exam success are **dependent events**  
✅ **Insight 2:** High attendance is the **strongest predictor** of exam success  
✅ **Insight 3:** Collaborative learning significantly impacts outcomes  
✅ **Insight 4:** Prior performance correlates with exam results  

---

## 🚀 Installation & Usage

### Prerequisites

```bash
Python 3.7+
Jupyter Notebook
```

### Required Libraries

```bash
pip install numpy pandas matplotlib seaborn scipy matplotlib-venn
```

### Running the Notebook

```bash
# Navigate to the project directory
cd "Expectation Decider"

# Start Jupyter
jupyter notebook

# Open: Expectation Decider.ipynb
```

### Data File

Ensure `Expectation Decider Data.csv` is in the same directory as the notebook.

---

## 📋 Results Summary

### 📊 Statistical Summary

| Metric | Value |
|--------|-------|
| Total Students | 200 |
| Pass Rate | 60.5% |
| Students with High Attendance | 43.5% |
| Students with High Study Hours | 54.0% |
| Group Discussion Participants | 59.0% |

### 🎯 Conditional Probabilities

| Condition | Probability |
|-----------|-------------|
| P(Pass \| Group Discussion) | 0.636 |
| P(Pass \| High Attendance) | 0.778 |
| P(High Attendance \| Pass) | 0.702 |

### 📈 Distribution Statistics (Binomial: n=3, p=0.605)

| Statistic | Value |
|-----------|-------|
| Mean | 1.815 |
| Variance | 0.717 |
| Std Dev | 0.847 |
| Most Likely Outcome | 2 passes (43.4%) |

---

## 🎬 Learn More

Watch this comprehensive video tutorial to understand probability concepts and their real-world applications:

[![Watch Probability Theory Complete Guide](https://img.shields.io/badge/📹-Watch%20Probability%20Concepts-FF0000?style=for-the-badge)](https://www.youtube.com/results?search_query=probability+theory)

---

## 📝 Learning Outcomes

After completing this project, you will understand:

✔️ Fundamental probability concepts and calculations  
✔️ Difference between empirical and theoretical probability  
✔️ Conditional probability and Bayes' theorem  
✔️ Probability distributions (especially binomial)  
✔️ Event relationships (independence, dependence, mutual exclusivity)  
✔️ Real-world application of probability theory  
✔️ How to analyze contingency tables  
✔️ Statistical inference from data  

---

## 🔗 Related Topics

- Probability Theory
- Advanced Statistics
- Binomial Distribution
- Bayesian Inference
- Conditional Probability
- Educational Data Analysis

---

## 👤 Author

**Your Name** | Mathematics & Advanced Statistics Enthusiast

📧 Email: [Your Email]  
🔗 GitHub: [@kotadiyadarshil18-code](https://github.com/kotadiyadarshil18-code)

---

## 📄 License

This project is open source and available under the MIT License.

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- 📝 Add more examples
- 🐛 Report issues
- 💡 Suggest improvements
- 📚 Add additional analysis

---

## ⭐ If This Helped You

Please consider giving this repository a star! ⭐ It motivates continued development of educational content.

---

**Last Updated:** 2026-06-11  
**Status:** ✅ Complete and Ready for Use

---

> 📌 **Note:** This notebook is designed for educational purposes. It demonstrates key concepts in probability and statistics through practical application and real-world data analysis.
