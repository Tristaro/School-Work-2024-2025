**DS1000 Midterm Cheat Sheet**

---

### **Key Concepts & Definitions**

- **Data Types:**
    
    - **Categorical**: Data that represents groups or categories (e.g., eye color, gender, zip codes).
    - **Quantitative**: Numerical data that represents amounts or measurements (e.g., height, weight, test scores).
    - **Example**: A dataset with students' favorite colors (categorical) and their heights (quantitative).
- **Descriptive Statistics:**
    
    - **Mean**: Average value of a dataset.
    - **Median**: Middle value when data is ordered.
    - **Mode**: Most frequently occurring value.
    - **Variance & Standard Deviation**: Measure how spread out the data is.
    - **Example**: Given test scores [70, 80, 85, 90, 95], the mean is 84, median is 85, and standard deviation shows how much scores deviate from the mean.
- **Distribution Shapes:**
    
    - **Symmetric**: Left and right sides mirror each other.
    - **Skewed Left**: Tail on the left (e.g., exam scores where most students score high but a few score very low).
    - **Skewed Right**: Tail on the right (e.g., income distribution where most people earn lower amounts but a few earn very high).
    - **Example**: A histogram showing salaries where most employees earn $50,000 but a few executives earn $500,000 (right-skewed).
- **Boxplots & Five-Number Summary:**
    
    - **Five-Number Summary**: Minimum, Q1 (25th percentile), Median (50th percentile), Q3 (75th percentile), Maximum.
    - **Boxplot**: A visual representation of the five-number summary.
    - **Example**: A boxplot of student heights showing a median of 170 cm, with a few outliers above 190 cm.
- **Normal Distribution:**
    
    - Bell-shaped, symmetric curve where most values cluster around the mean.
    - **68-95-99.7 Rule**: 68% of data falls within 1 standard deviation, 95% within 2, and 99.7% within 3.
    - **Example**: IQ scores follow a normal distribution with mean 100 and standard deviation 15.
- **Z-score:**
    
    - Measures how many standard deviations a value is from the mean.
    - Formula: z=x−μσz = \frac{x - \mu}{\sigma}
    - **Example**: If SAT scores have a mean of 500 and standard deviation of 100, a score of 650 has a z-score of (650-500)/100 = 1.5.
- **Correlation (r):**
    
    - Measures strength & direction of a linear relationship between two variables (-1 to 1).
    - **Example**: Height and weight have a strong positive correlation (~0.8), meaning taller people tend to weigh more.
- **Regression Equation:**
    
    - Describes the relationship between dependent (Y) and independent (X) variables.
    - Formula: y=a+bxy = a + bx
    - **Example**: Predicting weight (Y) based on height (X), where y=50+0.5xy = 50 + 0.5x means for every 1 cm increase in height, weight increases by 0.5 kg.
- **Residuals:**
    
    - Difference between actual and predicted values in regression.
    - Formula: e=y−y^e = y - \hat{y}
    - **Example**: If actual weight is 80 kg and predicted is 78 kg, residual is 80 - 78 = 2.
- **Relative Risk (RR):**
    
    - Compares risk between two groups.
    - Formula: RR=p1p0RR = \frac{p_1}{p_0}
    - **Example**: If 10% of smokers get lung cancer but only 2% of non-smokers do, RR = 10/2 = 5.
- **Odds Ratio (OR):**
    
    - Compares odds of an event occurring in two groups.
    - Formula: OR=p1/(1−p1)p0/(1−p0)OR = \frac{p_1 / (1 - p_1)}{p_0 / (1 - p_0)}
    - **Example**: If 20% of exposed people develop a disease while 5% of non-exposed do, OR = (0.2/0.8) / (0.05/0.95) = 4.
- **Standard Normal Table:**
    
    - Used to find probabilities for standard normal (Z) scores.
    - **Example**: If Z = 1.5, the table shows P(Z < 1.5) ≈ 0.933.

---

### **Important Formulas**

- **Mean (********xˉ\bar{x}********)**: ∑xin\frac{\sum x_i}{n}
- **Variance (********s2s^2********)**: ∑(xi−xˉ)2n−1\frac{\sum (x_i - \bar{x})^2}{n-1}
- **Standard Deviation (********ss********)**: s2\sqrt{s^2}
- **Correlation (r)**: r=∑(xi−xˉ)(yi−yˉ)(n−1)sxsyr = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{(n-1)s_x s_y}
- **Regression Slope (b)**: b=rsysxb = r \frac{s_y}{s_x}
- **Intercept (a)**: a=yˉ−bxˉa = \bar{y} - b\bar{x}
- **Relative Risk (RR)**: P(disease∣exposed)P(disease∣unexposed)\frac{P(disease | exposed)}{P(disease | unexposed)}
- **Odds Ratio (OR)**: (a/c)(b/d)\frac{(a/c)}{(b/d)}

---

### **Midterm Review Questions & Answers**

1. First quartile falls in: **c. 71-80**
2. Standard deviation remains: **d. unchanged**
3. SAT scores probability: **b. 0.317**
4. Residual plot suggests: **a. Straight line is not a good fit**
5. Median estimate: **a. 15**
6. Python probability function: **b. 1 - norm.cdf(0.5, loc=1, scale=2)**
7. Boxplot provides: **d. All of the above**
8. Association explained by: **c. Lurking variables**
9. Mean age from boxplot: **c. Higher than controls**
10. Overweight threshold: **c. 34.15 oz**
11. Regression effectiveness: **b. Not effective**
12. Who ranked better?: **b. Equally well**
13. Removing outlier affects slope: **b. Decrease**
14. Regression intercept: **c. -8.5**
15. Proportion sleeping <6h: **b. 0.292**
16. > 4h study & <6h sleep: **c. 0.4**
    
17. Python for mean & plot: **d. Correct syntax**
18. Relative risk for smokers: **c. 2.6**
19. Odds ratio non-smokers: **a. 3.5**
20. Resistant measure: **d. Interquartile range**

---

### **Python Quick Reference**

- **Importing Libraries:** `import numpy as np, import pandas as pd`
- **Descriptive Stats:**
    
    ```python
    np.mean(x), np.median(x), np.std(x, ddof=1)
    ```
    
- **Normal Distribution Calculations:**
    
    ```python
    from scipy.stats import norm
    norm.cdf(value, loc=mean, scale=std)
    ```
    
- **Regression:**
    
    ```python
    from sklearn.linear_model import LinearRegression
    model = LinearRegression()
    model.fit(X, y)
    ```
    

---

**Good luck!**