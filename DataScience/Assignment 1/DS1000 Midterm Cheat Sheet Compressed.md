/* Multi-Column Markdown Plugin for Obsidian */
.columns {
  column-count: 3;
  column-gap: 10px;
  font-size: 6pt;
}
```

```markdown
<div class="columns">

## **Key Concepts & Definitions**
### **Data Types**
- **Categorical**: Data representing groups/categories (e.g., eye color, zip codes).
- **Quantitative**: Numerical data (e.g., height, weight).
- **Example**: A dataset with students' favorite colors (categorical) and heights (quantitative).

### **Descriptive Statistics**
- **Mean**: Average value.
- **Median**: Middle value when ordered.
- **Mode**: Most frequent value.
- **Variance & Std Dev**: Spread of data.
- **Example**: Test scores `[70, 80, 85, 90, 95]`, mean = 84, median = 85.

### **Distribution Shapes**
- **Symmetric**: Left & right mirror.
- **Skewed Left**: Tail on left (e.g., test scores).
- **Skewed Right**: Tail on right (e.g., income distribution).
- **Example**: Salaries mostly $50k but a few at $500k (right-skewed).

### **Boxplots & Five-Number Summary**
- **Min, Q1, Median, Q3, Max**
- **Boxplot**: Visual representation.
- **Example**: Heights with median 170 cm, outliers at 190 cm.

### **Normal Distribution**
- Bell-shaped, symmetric.
- **68-95-99.7 Rule**
- **Example**: IQ scores (mean 100, std dev 15).

### **Z-score**
- Standard deviations from mean.
- `z = (x - μ) / σ`
- **Example**: SAT mean = 500, std dev = 100, score 650 → `z = 1.5`.

### **Correlation (r)**
- Strength/direction of linear relationship (-1 to 1).
- **Example**: Height & weight (~0.8 correlation).

### **Regression Equation**
- `y = a + bx`
- **Example**: Predict weight (Y) based on height (X): `y = 50 + 0.5x`.

### **Residuals**
- Difference: `e = y - ŷ`
- **Example**: Actual 80kg, predicted 78kg → residual = 2.

### **Relative Risk (RR)**
- `RR = P(disease | exposed) / P(disease | unexposed)`
- **Example**: Smokers (10%) vs non-smokers (2%) → `RR = 5` (5× higher risk).

### **Odds Ratio (OR)**
- `OR = (p1 / (1 - p1)) / (p0 / (1 - p0))`
- **Example**: Disease risk 20% (exposed) vs 5% (unexposed) → `OR = 4`.

### **Standard Normal Table**
- **Example**: `P(Z < 1.5) ≈ 0.933`

## **Important Formulas & Explanations**
### **Mean (x̄)**
- `x̄ = Σxᵢ / n`
- **Example**: `[5,10,15]` → mean = `10`.

### **Variance (s²)**
- `s² = Σ (xᵢ - x̄)² / (n-1)`
- **Example**: `[5,10,15]`, variance = `25`.

### **Standard Deviation (s)**
- `s = √s²`

### **Correlation (r)**
- `r = Σ (xᵢ - x̄)(yᵢ - ȳ) / ( (n-1) * sₓ * sᵧ )`

### **Regression Slope (b)**
- `b = r (sᵧ / sₓ)`
- **Example**: Height ↑1cm → Weight ↑0.5kg, `b = 0.5`.

### **Intercept (a)**
- `a = ȳ - b x̄`
- **Example**: `y = 50 + 0.5x`, when `x = 0`, `y = 50`.

## **Python Quick Reference**
```python
import numpy as np
import pandas as pd

# Descriptive Stats
np.mean(x), np.median(x), np.std(x, ddof=1)

# Normal Distribution
from scipy.stats import norm
norm.cdf(value, loc=mean, scale=std)

# Regression
from sklearn.linear_model import LinearRegression
model = LinearRegression()
model.fit(X, y)
```
</div>
