<div align="center">

# 📘 Mathematics Advanced Statistics

### 🚀 A Complete Mathematics & Statistics Analysis Project Using Python

<img src="https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python">
<img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter">
<img src="https://img.shields.io/badge/Pandas-Data%20Analysis-purple?style=for-the-badge&logo=pandas">
<img src="https://img.shields.io/badge/NumPy-Mathematics-blue?style=for-the-badge&logo=numpy">
<img src="https://img.shields.io/badge/Matplotlib-Visualization-success?style=for-the-badge">
<img src="https://img.shields.io/badge/Statistics-Advanced-red?style=for-the-badge">

---

A comprehensive project demonstrating **Mathematics**, **Statistics**, **Linear Algebra**, **Vectors**, **Matrices**, and **Data Analysis** using Python and Jupyter Notebook.

⭐ If you found this project useful, don't forget to Star this Repository!

</div>

---

# 📖 Project Overview

This repository presents an advanced implementation of mathematical and statistical concepts using Python.

The project demonstrates how mathematical theories can be applied to real-world datasets by performing calculations, statistical analysis, vector operations, matrix operations, and data visualization.

The notebook has been designed in a beginner-friendly manner where each concept is implemented using Python with proper explanations.

---

# 🎯 Objectives

The primary objectives of this project are:

- Learn Mathematical Computing using Python
- Understand Statistical Concepts
- Work with Real Dataset
- Perform Data Analysis
- Learn Vector Operations
- Learn Matrix Operations
- Apply Linear Algebra
- Perform Mathematical Calculations
- Improve Python Programming Skills
- Visualize Data Effectively

---

# ✨ Features

✔ Student Performance Dataset

✔ Data Loading

✔ Data Cleaning

✔ Exploratory Data Analysis

✔ Vector Fundamentals

✔ Matrix Fundamentals

✔ Linear Algebra Operations

✔ L1 Norm

✔ L2 Norm

✔ Dot Product

✔ Cross Product

✔ Angle Between Vectors

✔ Statistical Calculations

✔ Mathematical Visualization

✔ Beginner Friendly Code

✔ Well Structured Notebook

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|----------|
| Python | Programming Language |
| Jupyter Notebook | Development Environment |
| Pandas | Data Processing |
| NumPy | Mathematical Operations |
| Matplotlib | Data Visualization |
| CSV Dataset | Student Performance Analysis |

---

# 📂 Dataset Information

Dataset Name

> Student_Performance.csv

Dataset contains student academic information which is used for performing mathematical operations and statistical analysis.

Example attributes include:

- Student Scores
- Academic Performance
- Numerical Features
- Statistical Variables

The dataset is primarily used to demonstrate mathematical concepts instead of building machine learning models.

---

# 📊 Mathematical Concepts Covered

The project includes implementation of the following concepts:

## Linear Algebra

- Scalars
- Vectors
- Matrices
- Vector Magnitude
- Unit Vector
- Dot Product
- Cross Product
- Angle Between Vectors

## Statistics

- Mean
- Median
- Mode
- Variance
- Standard Deviation
- Range
- Data Distribution

## Mathematical Operations

- L1 Norm
- L2 Norm
- Euclidean Distance
- Matrix Calculations
- Vector Calculations
- Mathematical Interpretation

---

# 📈 Project Workflow

```text
Start
   │
   ▼
Import Libraries
   │
   ▼
Load Dataset
   │
   ▼
Understand Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Mathematical Operations
   │
   ▼
Statistical Analysis
   │
   ▼
Vector Operations
   │
   ▼
Matrix Operations
   │
   ▼
Visualization
   │
   ▼
Results
   │
   ▼
End
```

---

# 📁 Project Structure

```
Mathematics-Advanced-Statistics/

│── Calculative Foundation.ipynb
│── Student_Performance.csv
│── README.md
│── requirements.txt
│── LICENSE
│── .gitignore
```

---

# 🎥 Project Demonstration Video

Watch the complete explanation of this project here:

📺 **Video Link:** (https://drive.google.com/file/d/1NxYnqzNCreRGhOSAaDtm7g9ISNANosnz/view?usp=sharing)

This video covers:

- Project Overview
- Dataset Explanation
- Mathematics Concepts
- Statistics Concepts
- Code Walkthrough
- Final Results

---

# 📚 Code Explanation

---

# Question 1: Import Libraries

## Code

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import statistics as stats
import math
from scipy import linalg
import scipy
import seaborn as sns
from sklearn.decomposition import PCA
from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
```

## Explanation

- Imported all the required Python libraries for the project.
- **Pandas** is used for loading and managing the dataset.
- **NumPy** performs vector, matrix and mathematical calculations.
- **Matplotlib** and **Seaborn** are used to create graphs and visualizations.
- **SciPy** provides advanced linear algebra functions.
- **PCA** and **LDA** are imported for dimensionality reduction techniques.

---

# Question 2: Import Dataset

## Code

```python
data = pd.read_csv("Student_Performance.csv")
data.head()
```

## Explanation

- Loaded the **Student_Performance.csv** dataset using Pandas.
- Stored the dataset in the variable **data**.
- Used the `head()` function to display the first five rows.
- Verified that the dataset was loaded correctly.
- This dataset is used for all mathematical and statistical operations.

---

# Question 3: Represent Each Student's Subject Scores as a Vector

## Code

```python
# Student 1 Score Vector
student_1 = data.loc[0, ['math_score', 'science_score', 'english_score']].to_numpy(dtype=float)

# Student 2 Score Vector
student_2 = data.loc[1, ['math_score', 'science_score', 'english_score']].to_numpy(dtype=float)

# Student 3 Score Vector
student_3 = data.loc[2, ['math_score', 'science_score', 'english_score']].to_numpy(dtype=float)

print("Student 1:", student_1)
print("Student 2:", student_2)
print("Student 3:", student_3)
```

## Explanation

- Selected the Math, Science and English scores of the first three students.
- Converted the selected scores into NumPy arrays using `to_numpy()`.
- Each NumPy array represents one student's marks as a mathematical vector.
- These vectors are used for vector operations such as L1 Norm, L2 Norm, Dot Product and Projection.
- Converting the dataset into vectors makes mathematical calculations easier and more efficient.

## Mathematical Representation

Let the score vector of a student be:

$$
\mathbf{v}=
\begin{bmatrix}
Math\\
Science\\
English
\end{bmatrix}
$$

For Student 1,

$$
\mathbf{v_1}=
\begin{bmatrix}
42.7\\
55.4\\
57.0
\end{bmatrix}
$$

For Student 2,

$$
\mathbf{v_2}=
\begin{bmatrix}
57.6\\
68.8\\
64.8
\end{bmatrix}
$$

For Student 3,

$$
\mathbf{v_3}=
\begin{bmatrix}
84.8\\
95.0\\
79.2
\end{bmatrix}
$$

## Output

```text
Student 1: [42.7 55.4 57.0]
Student 2: [57.6 68.8 64.8]
Student 3: [84.8 95.0 79.2]
```

---
## Question 4 : Calculate L1 Norm

### Explanation

- Calculated the L1 Norm (Manhattan Distance) of each student vector.
- L1 Norm is the sum of the absolute values of all vector elements.
- It measures the overall magnitude of a vector.
- Higher L1 Norm indicates higher combined subject scores.
- This metric is widely used in optimization and machine learning.

**Formula**

$$
L1 = |x_1| + |x_2| + |x_3|
$$

---

## Question 5 : Calculate L2 Norm

### Explanation

- Calculated the Euclidean length of each student's score vector.
- L2 Norm measures the straight-line distance from the origin.
- It represents the actual magnitude of the vector.
- Students with larger score values have larger L2 Norms.
- This norm is commonly used in Linear Algebra and Machine Learning.

**Formula**

$$
L2=\sqrt{x_1^2+x_2^2+x_3^2}
$$

---

## Question 6 : Dot Product

### Explanation

- Calculated the dot product between two student vectors.
- The dot product measures the similarity between vectors.
- A larger value indicates that the vectors point in a similar direction.
- It is also used to calculate the angle between vectors.
- This concept is important in recommendation systems and machine learning.

**Formula**

$$
A\cdot B=x_1y_1+x_2y_2+x_3y_3
$$

---

## Question 7 : Angle Between Two Vectors

### Explanation

- Calculated the cosine of the angle using the dot product.
- Converted the cosine value into an angle in degrees.
- A smaller angle indicates more similar performance.
- A larger angle indicates greater difference between students.
- This helps compare two vectors mathematically.

**Formula**

$$
\cos\theta=\frac{A\cdot B}{||A||\,||B||}
$$

---

## Question 8 : Projection of One Vector onto Another

### Explanation

- Projected one student's score vector onto another vector.
- Projection measures how much one vector lies in the direction of another.
- It is useful for feature analysis and dimensionality reduction.
- The projected vector preserves the direction of the reference vector.
- Projection is an important concept in Linear Algebra.

---

## Question 9 : Matrix Addition

### Explanation

- Converted student vectors into matrices.
- Added two matrices using NumPy.
- Matrix addition is performed by adding corresponding elements.
- Both matrices must have the same dimensions.
- The result is a new matrix containing the summed values.

---

## Question 10 : Matrix Multiplication

### Explanation

- Multiplied matrices using matrix multiplication rules.
- Each row is multiplied by each column.
- Matrix multiplication is different from element-wise multiplication.
- It is widely used in graphics, AI and scientific computing.
- The resulting matrix represents combined mathematical transformations.

---

---

# 📊 Results

The project successfully demonstrates the practical implementation of various mathematical and statistical concepts using Python.

### Key Results

- Successfully represented student scores as mathematical vectors.
- Computed L1 Norm and L2 Norm for measuring vector magnitude.
- Calculated the Dot Product to determine vector similarity.
- Measured the Angle Between Vectors using cosine similarity.
- Performed Vector Projection for directional analysis.
- Executed Matrix Addition, Matrix Multiplication, and Matrix Transpose.
- Calculated the Covariance Matrix for feature relationship analysis.
- Computed the Determinant and Inverse of matrices.
- Performed Eigenvalue and Eigenvector analysis.
- Applied LU Decomposition and Singular Value Decomposition (SVD).
- Implemented Principal Component Analysis (PCA).
- Implemented Linear Discriminant Analysis (LDA).
- Visualized mathematical concepts using 2D and 3D plots.

---

# 📚 Learning Outcomes

After completing this project, I gained practical knowledge of:

- Python Programming
- Data Analysis using Pandas
- Numerical Computing with NumPy
- Data Visualization using Matplotlib and Seaborn
- Linear Algebra Concepts
- Vector Mathematics
- Matrix Operations
- Eigenvalues and Eigenvectors
- PCA (Principal Component Analysis)
- LDA (Linear Discriminant Analysis)
- Scientific Computing using SciPy

---

# 🚀 Future Improvements

This project can be further enhanced by adding:

- Interactive Dashboard using Streamlit
- Power BI Dashboard Integration
- Machine Learning Models
- Student Performance Prediction
- Advanced Statistical Analysis
- Correlation Heatmaps
- Interactive Visualizations
- More Real-world Datasets

---


---

# 📦 Requirements

```text
numpy
pandas
matplotlib
seaborn
scipy
scikit-learn
jupyter
```

# 👨‍💻 Author ## Darshil Kotadiya

**Student | Python Developer | Data Analytics Enthusiast**

**GitHub:**  
https://github.com/kotadiyadarshil18-code

---

# 📄 License

This project is licensed under the **MIT License**.


<div align="center">

## ⭐ Thank You for Visiting This Repository ⭐



</div>
