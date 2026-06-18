# 📊 Derivable Judgement: Inferential Statistics Analysis

> A comprehensive statistical analysis project demonstrating hypothesis testing, confidence intervals, and various statistical tests on healthcare data.

---

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Description](#-dataset-description)
- [Hypotheses](#-hypotheses)
- [Statistical Methods](#-statistical-methods)
- [Results Summary](#-results-summary)
- [Key Findings](#-key-findings)
- [Video Resources](#-video-resources)
- [Study Materials](#-study-materials)
- [Installation & Usage](#-installation--usage)

---

## 🎯 Project Overview

**Derivable Judgement** is an inferential statistics project that applies advanced statistical techniques to analyze healthcare data. The project demonstrates how to derive meaningful conclusions from sample data and make informed judgments about population parameters.

### Objectives:
✅ Calculate confidence intervals for key variables  
✅ Perform hypothesis testing using t-tests  
✅ Test independence using chi-square tests  
✅ Compare multiple groups using ANOVA  
✅ Analyze relationships through correlation and covariance  

---

## 📁 Dataset Description

| Attribute | Type | Description |
|-----------|------|-------------|
| **record_id** | UUID | Unique identifier for each patient |
| **age_group** | Categorical | Age brackets (18-25, 26-35, 36-45, 46-60, 60+) |
| **age** | Numerical | Actual age in years |
| **weight** | Numerical | Weight in kilograms |
| **gender** | Categorical | Male, Female, Other |
| **region** | Categorical | Geographic regions (North, South, East, West) |
| **smoking_status** | Categorical | Smoker, Non-Smoker, Former Smoker |
| **exercise_frequency** | Categorical | Daily, Weekly, Rarely, Never |
| **bmi** | Numerical | Body Mass Index |
| **blood_pressure** | Numerical | Systolic blood pressure (mmHg) |
| **diabetes** | Boolean | Presence of diabetes (True/False) |
| **hypertension** | Boolean | Presence of hypertension (True/False) |
| **cholesterol_level** | Numerical | Cholesterol in mg/dL |
| **glucose_level** | Numerical | Fasting glucose in mg/dL |
| **visit_date** | Date | Date of medical visit |

**📊 Dataset Size:** 200 patient records

---

## 🔬 Hypotheses

### **Hypothesis 1: Smoking Status & Diabetes Prevalence**

| Component | Statement |
|-----------|-----------|
| **H₀** | Smoking status has **no effect** on diabetes prevalence |
| **H₁** | Smoking status **affects** diabetes prevalence |
| **Test Used** | Chi-Square Test of Independence |
| **Significance Level** | α = 0.05 |

### **Hypothesis 2: BMI Difference Between Genders**

| Component | Statement |
|-----------|-----------|
| **H₀** | No significant difference in BMI between genders |
| **H₁** | Significant difference in BMI between genders |
| **Test Used** | Independent t-Test |
| **Significance Level** | α = 0.05 |

---

## 📐 Statistical Methods

### **1️⃣ Confidence Intervals (95%)**

**Formula:**
```
CI = x̄ ± t(α/2, n-1) × SE

where:
  x̄ = Sample Mean
  t(α/2, n-1) = t-critical value
  SE = Standard Error = s/√n
  s = Sample Standard Deviation
  n = Sample Size
```

| Variable | Mean | 95% CI Lower | 95% CI Upper |
|----------|------|-------------|------------|
| **Age (years)** | 49.04 | 46.47 | 51.60 |
| **Weight (kg)** | 78.00 | 75.23 | 80.76 |

---

### **2️⃣ Independent t-Test (BMI by Gender)**

**Formula:**
```
t = (x̄₁ - x̄₂) / √(s₁²/n₁ + s₂²/n₂)

Degrees of Freedom (df) = n₁ + n₂ - 2
```

**Results:**

| Metric | Value |
|--------|-------|
| **t-Statistic** | -1.152 |
| **p-value** | 0.252 |
| **Critical Value (α=0.05)** | ±1.972 |
| **Decision** | ✅ **Accept H₀** |
| **Interpretation** | No significant difference in BMI between genders |

---

### **3️⃣ Chi-Square Test (Smoking Status × Diabetes)**

**Formula:**
```
χ² = Σ [(Observed - Expected)² / Expected]

Degrees of Freedom (df) = (rows - 1) × (columns - 1)

Critical Value: χ²(α, df)
```

**Results:**

| Metric | Value |
|--------|-------|
| **Chi-Square Statistic** | 0.029 |
| **p-value** | 0.986 |
| **Critical Value (α=0.05, df=2)** | 5.991 |
| **Decision** | ✅ **Accept H₀** |
| **Interpretation** | Smoking status is **independent** of diabetes prevalence |

---

### **4️⃣ ANOVA Test (BMI across Age Groups)**

**Formula:**
```
F = MSB / MSW

where:
  MSB (Mean Squares Between) = SSB / (k - 1)
  MSW (Mean Squares Within) = SSW / (n - k)
  
  SSB = Σ nᵢ(x̄ᵢ - x̄grand)²
  SSW = Σ Σ (xᵢⱼ - x̄ᵢ)²
```

**Group Statistics:**

| Age Group | Sample Size | Mean BMI | Std Dev |
|-----------|------------|----------|---------|
| **18-25** | 22 | 27.52 | 4.8 |
| **26-35** | 38 | 27.90 | 5.2 |
| **36-45** | 38 | 25.03 | 5.1 |
| **46-60** | 39 | 30.01 | 4.9 |
| **60+** | 63 | 27.49 | 5.3 |
| **TOTAL** | 200 | 27.59 | 5.2 |

**ANOVA Results:**

| Source | Sum of Squares | df | Mean Square | F-Statistic | p-value |
|--------|----------------|----|----|------------|---------|
| **Between Groups** | 480.55 | 4 | 120.14 | 1.124 | 0.354 |
| **Within Groups** | 6200.25 | 195 | 31.79 | - | - |
| **Total** | 6680.80 | 199 | - | - | - |

**Decision:** ✅ **Accept H₀** - No significant difference in BMI across age groups

---

### **5️⃣ Covariance & Correlation (Age × BMI)**

**Formula:**
```
Covariance: Cov(X,Y) = Σ(xᵢ - x̄)(yᵢ - ȳ) / (n-1)

Correlation: r = Cov(X,Y) / (σₓ × σᵧ)

Pearson's r range: [-1, 1]
```

| Metric | Value | Interpretation |
|--------|-------|-----------------|
| **Covariance** | 5.782 | Weak positive relationship |
| **Correlation (r)** | 0.054 | **Very weak** positive correlation |
| **R² (Coefficient of Determination)** | 0.0029 | Age explains only 0.29% of BMI variation |

**Interpretation:** 🔗 Age and BMI are **virtually independent** with negligible linear relationship

---

## 📈 Results Summary

| Test | Hypothesis | Result | p-value | Decision |
|------|-----------|--------|---------|----------|
| **Confidence Intervals** | Population Parameters | CI Calculated | - | ✅ |
| **t-Test** | BMI by Gender | Not Significant | 0.252 | Accept H₀ |
| **Chi-Square** | Smoking × Diabetes | Not Significant | 0.986 | Accept H₀ |
| **ANOVA** | BMI by Age Group | Not Significant | 0.354 | Accept H₀ |
| **Correlation** | Age × BMI | Negligible (r=0.054) | - | ✅ |

---

## 💡 Key Findings

### 🎯 Main Conclusions:

1. **Gender & BMI:** 👥
   - No statistically significant difference in BMI between males and females
   - Both groups show similar BMI distributions

2. **Smoking & Diabetes:** 🚬
   - Smoking status is **independent** of diabetes prevalence in this dataset
   - Diabetes occurs across all smoking categories at similar rates

3. **Age & BMI:** 📅
   - Age groups show different mean BMIs, but differences are **not statistically significant**
   - BMI variation within age groups is larger than variation between them

4. **Age & BMI Relationship:** 📊
   - Extremely weak correlation (r = 0.054)
   - Age is **not a good predictor** of BMI
   - Less than 1% of BMI variation is explained by age

---

## 🎥 Video Resources

Explore these resources to understand the statistical concepts used in this project:

### Video Link 
[![Click Here For Video](https://drive.google.com/file/d/1puypV9I74IvJIYWn9Z8zhXz7vLD1YLkn/view?usp=sharing)


---

## 📚 Study Materials

### Multiple Choice Questions & Answers

Prepare for your exams with our comprehensive Q&A document covering all topics from this project!

[![Download MCQ Document](https://img.shields.io/badge/Download-MCQ%20Questions%20%26%20Answers-green?style=for-the-badge&logo=googledrive&logoColor=white)](./Derivable_Judgement_MCQ_Answers.docx)

**Document Includes:**
- ✅ 50+ Multiple Choice Questions
- ✅ Detailed Answers with Explanations
- ✅ Topics: Hypothesis Testing, Confidence Intervals, t-Tests, Chi-Square, ANOVA
- ✅ Difficulty Levels: Basic to Advanced
- ✅ Perfect for exam preparation

---

## 🚀 Installation & Usage

### Prerequisites
```bash
Python 3.7+
pandas
numpy
scipy
```

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/kotadiyadarshil18-code/Mathematics-Advanced-Statistics.git
cd Mathematics-Advanced-Statistics
```

2. **Install dependencies:**
```bash
pip install pandas numpy scipy matplotlib
```

3. **Navigate to the project:**
```bash
cd "Derivable Judgement"
```

### Running the Notebook

```bash
jupyter notebook "Derivable Judgement.ipynb"
```

Or open directly in your preferred Jupyter environment (VS Code, Google Colab, etc.)

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Python 3.14** | Programming language |
| **Jupyter Notebook** | Interactive analysis environment |
| **Pandas** | Data manipulation & analysis |
| **NumPy** | Numerical computing |
| **SciPy** | Statistical functions & distributions |
| **Matplotlib** | Data visualization |

---

## 📊 Project Structure

```
Derivable Judgement/
├── Derivable Judgement.ipynb              # Main analysis notebook
├── health_dataset_200_records.csv         # Dataset
├── Derivable_Judgement_MCQ_Answers.docx   # Study material (MCQs)
└── README.md                              # Documentation
```

---

## 📝 Formula Reference Sheet

### Common Statistical Formulas

**Standard Error:**
```
SE = s / √n
```

**Confidence Interval:**
```
CI = x̄ ± z* × SE  (for large samples)
CI = x̄ ± t* × SE  (for small samples)
```

**t-Test Statistic:**
```
t = (x̄₁ - x̄₂) / √(s₁²/n₁ + s₂²/n₂)
```

**Chi-Square Statistic:**
```
χ² = Σ [(O - E)² / E]
```

**F-Statistic (ANOVA):**
```
F = Variance Between Groups / Variance Within Groups
```

**Pearson Correlation:**
```
r = Cov(X,Y) / (σₓ × σᵧ)
```

---

## 👨‍💻 Author

**Darshil Kotadiya**  
📧 Email: kotadiyadarshil18@example.com  
🐙 GitHub: [@kotadiyadarshil18-code](https://github.com/kotadiyadarshil18-code)



</div>
