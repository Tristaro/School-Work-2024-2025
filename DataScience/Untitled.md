# DS1000 Midterm Cheat Sheet

---

## **Key Concepts & Definitions**

### **Data Types**

- **Categorical**: Data that represents groups or categories (e.g., eye color, gender, zip codes).
- **Quantitative**: Numerical data that represents amounts or measurements (e.g., height, weight, test scores).
- **Example**: A dataset with students' favorite colors (categorical) and their heights (quantitative).

### **Descriptive Statistics**

- **Mean**: Average value of a dataset.
- **Median**: Middle value when data is ordered.
- **Mode**: Most frequently occurring value.
- **Variance & Standard Deviation**: Measure how spread out the data is.
- **Example**: Given test scores `[70, 80, 85, 90, 95]`, the mean is 84, median is 85, and standard deviation shows how much scores deviate from the mean.

### **Distribution Shapes**

- **Symmetric**: Left and right sides mirror each other.
- **Skewed Left**: Tail on the left (e.g., exam scores where most students score high but a few score very low).
- **Skewed Right**: Tail on the right (e.g., income distribution where most people earn lower amounts but a few earn very high).
- **Example**: A histogram showing salaries where most employees earn $50,000 but a few executives earn $500,000 (right-skewed).

### **Boxplots & Five-Number Summary**

- **Five-Number Summary**: Minimum, Q1 (25th percentile), Median (50th percentile), Q3 (75th percentile), Maximum.
- **Boxplot**: A visual representation of the five-number summary.
- **Example**: A boxplot of student heights showing a median of 170 cm, with a few outliers above 190 cm.

### **Normal Distribution**

- Bell-shaped, symmetric curve where most values cluster around the mean.
- **68-95-99.7 Rule**: 68% of data falls within 1 standard deviation, 95% within 2, and 99.7% within 3.
- **Example**: IQ scores follow a normal distribution with mean 100 and standard deviation 15.

### **Z-score**

- Measures how many standard deviations a value is from the mean.
- **Formula**: `z = (x - μ) / σ`
- **Example**: If SAT scores have a mean of 500 and standard deviation of 100, a score of 650 has a z-score of `(650-500)/100 = 1.5`.

### **Correlation (r)**

- Measures strength & direction of a linear relationship between two variables (-1 to 1).
- **Example**: Height and weight have a strong positive correlation (~0.8), meaning taller people tend to weigh more.

### **Regression Equation**

- Describes the relationship between dependent (Y) and independent (X) variables.
- **Formula**: `y = a + bx`
- **Example**: Predicting weight (Y) based on height (X), where `y = 50 + 0.5x` means for every 1 cm increase in height, weight increases by 0.5 kg.

### **Residuals**

- Difference between actual and predicted values in regression.
- **Formula**: `e = y - ŷ`
- **Example**: If actual weight is 80 kg and predicted is 78 kg, residual is `80 - 78 = 2`.

### **Relative Risk (RR)**

- Compares risk between two groups.
- **Formula**: `RR = P(disease | exposed) / P(disease | unexposed)`
- **Example**: If 10% of smokers get lung cancer but only 2% of non-smokers do, RR = `10/2 = 5`.
- RR=1: No difference in risk between the two groups.
- RR>1: Higher risk in the exposed group (risk factor).
- RR<1: Lower risk in the exposed group (protective factor).

### **Odds Ratio (OR)**

- Compares odds of an event occurring in two groups.
- **Formula**: `OR = (p1 / (1 - p1)) / (p0 / (1 - p0))`
- **Example**: If 20% of exposed people develop a disease while 5% of non-exposed do, `OR = (0.2/0.8) / (0.05/0.95) = 4`.

### **Standard Normal Table**

- Used to find probabilities for standard normal (Z) scores.
- **Example**: If Z = 1.5, the table shows `P(Z < 1.5) ≈ 0.933`.

---

## **Important Formulas**

```
Mean (x̄) = Σxᵢ / n
Variance (s²) = Σ (xᵢ - x̄)² / (n-1)
Standard Deviation (s) = √s²
Correlation (r) = Σ (xᵢ - x̄)(yᵢ - ȳ) / ( (n-1) * sₓ * sᵧ )
Regression Slope (b) = r (sᵧ / sₓ)
Intercept (a) = ȳ - b x̄
```

---

## **Python Quick Reference**

```python
import numpy as np
import pandas as pd

# Descriptive Stats
np.mean(x), np.median(x), np.std(x, ddof=1)

# Normal Distribution Calculations
from scipy.stats import norm
norm.cdf(value, loc=mean, scale=std)

# Regression
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
```

---

## **Good luck!**