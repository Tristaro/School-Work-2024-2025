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
- **Example**: Suppose we are studying lung cancer risk in smokers and non-smokers. The data is:

| Group           | People with Lung Cancer | Total People | Probability (PPP) |
| --------------- | ----------------------- | ------------ | ----------------- |
| **Smokers**     | 10                      | 100          | 10/100=0.10       |
| **Non-Smokers** | 2                       | 100          | 2/100=0.02        |
Now, calculate the **Relative Risk**:
RR = (0.10/0.02) = 5
This means that smokers are **5 times more likely** to develop lung cancer compared to non-smokers.
- RR=1: No difference in risk between the two groups.
- RR>1: Higher risk in the exposed group (risk factor).
- RR<1: Lower risk in the exposed group (protective factor).
### **Odds Ratio (OR)**
- Compares odds of an event occurring in two groups.
- **Formula**: `OR = (p1 / (1 - p1)) / (p0 / (1 - p0))`
-  Where:
	- p<sub>1</sub>​ = Probability of the event in the exposed group.
	- p<sub>0​</sub> = Probability of the event in the unexposed group.
	- 1−p<sub>1</sub>​ and 1−p<sub>0</sub>​ are the probabilities of the event _not_ occurring in the respective groups.
- **Example**: If 20% of exposed people develop a disease while 5% of non-exposed do, `OR = (0.2/0.8) / (0.05/0.95) = 4`.
### **Standard Normal Table**
- Used to find probabilities for standard normal (Z) scores.
- **Example**: If Z = 1.5, the table shows `P(Z < 1.5) ≈ 0.933`.
## **Important Formulas & Explanations**
### **Mean (x̄)**
- **Formula**: `x̄ = Σxᵢ / n`
- **Explanation**: The sum of all observations divided by the number of observations.
- **Example**: For the numbers `[5, 10, 15]`, mean = `(5+10+15)/3 = 10`.
### **Variance (s²)**
- **Formula**: `s² = Σ (xᵢ - x̄)² / (n-1)`
- **Explanation**: Measures the spread of the data from the mean.
- **Example**: If x̄ = 10 and data points are `[5, 10, 15]`, variance = `((5-10)² + (10-10)² + (15-10)²) / (3-1) = 25`.
### **Standard Deviation (s)**
- **Formula**: `s = √s²`
- **Explanation**: The square root of variance; gives the average deviation from the mean.
### **Correlation (r)**
- **Formula**: `r = Σ (xᵢ - x̄)(yᵢ - ȳ) / ( (n-1) * sₓ * sᵧ )`
- **Explanation**: Measures the strength and direction of a linear relationship between two variables.
- **Example**: If taller people tend to weigh more, `r` is positive.
### **Regression Slope (b)**
- **Formula**: `b = r (sᵧ / sₓ)`
- **Explanation**: Represents the change in `y` for a one-unit increase in `x`.
- **Example**: If height increases by 1 cm, weight increases by 0.5 kg, `b = 0.5`.
### **Intercept (a)**
- **Formula**: `a = ȳ - b x̄`
- **Explanation**: The predicted value of `y` when `x = 0`.
- **Example**: If the regression equation is `weight = 50 + 0.5(height)`, then when `height = 0`, predicted `weight = 50`.
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
### **Practice Multiple Choice Questions for DS1000 Midterm**

#### **1. In a class of 100 students, the grades on an accounting test are summarized in the following frequency table:**

|Grade Range|Frequency|
|---|---|
|91–100|11|
|81–90|31|
|71–80|42|
|61–70|16|
The first quartile would fall into what grade range?
- a. 91-100
- b. 81-90
- **c. 71-80** ✅
- d. 61-70
#### **2. If 5 points were added to each student's exam score, the standard deviation of the new scores would:**
- a. Be increased by 5
- b. Be increased by 25
- c. Be decreased by 5
- **d. Remain unchanged** ✅
#### **3. The proportion of students scoring between 460 and 550 on the SAT math test is closest to:**
- a. 0.309
- **b. 0.317** ✅
- c. 0.626
- d. 0.681
#### **4. A plot of residuals suggests that:**
- **a. A straight line is not a good summary for the data** ✅
- b. The correlation must be zero
- c. The correlation must be positive
- d. Outliers must be present
#### **5. From the histogram, the median property damage caused by tornadoes is approximately:**
- **a. 15** ✅
- b. 25
- c. 30
- d. 40
#### **6. To find the probability that a normally distributed variable (mean = 1, standard deviation = 2) is greater than 0.5, which Python code should be used?**
- a. `norm.cdf(0.5, loc=1, scale=2)`
- **b. `1 - norm.cdf(0.5, loc=1, scale=2)`** ✅
- c. `norm.ppf(0.5, loc=1, scale=2)`
- d. `1 - norm.ppf(0.5, loc=1, scale=2)`
#### **7. A boxplot of exam scores provides which pieces of information?**
- a. The median
- b. The IQR
- c. The minimum and the maximum
- **d. All of the answer options are correct** ✅
#### **8. A positive association between high school dropout rates and infant mortality is most likely due to:**
- a. x causes y
- b. y causes x
- **c. Lurking variables are present (e.g., larger populations increase both x and y)** ✅
- d. The association is purely coincidental
#### **9. Based on boxplots, the mean age for horses with enteroliths is:**
- **a. Lower than the mean age for the controls** ✅
- b. Approximately the same as the mean age for the controls
- c. Higher than the mean age for the controls
- d. Cannot be determined from boxplots
#### **10. A soap box is labeled overweight if it's in the top 5% of weights (mean = 33 oz, standard deviation = 0.7 oz). What is the cutoff?**
- a. 31.60 oz
- b. 31.85 oz
- **c. 34.15 oz** ✅
- d. 34.40 oz
#### **11. A regression model explains 13.4% of variation in BMI due to marijuana use. This model is:**
- a. Extremely effective
- **b. Not effective** ✅
- c. Extremely effective (36.6%)
- d. Not effective (36.6%)
#### **12. Your test score (90) and your friend's test score (75) came from different distributions. Who performed better?**
- a. You clearly ranked better
- **b. You and your friend ranked equally well** ✅
- c. Your friend actually ranked better
- d. Nothing; the tests cannot be compared
#### **13. If we omitted the highest-value point in a scatterplot, the regression line slope would:**
- a. Increase
- **b. Decrease** ✅
- c. Change very little
- d. Not enough information
#### **14. Given statistical values, what is the intercept of the least-squares regression line?**
- a. 48.5
- b. 1.9
- **c. -8.5** ✅
- d. 12.875
#### **15. What proportion of students slept less than 6 hours?**
- a. 0.286
- **b. 0.292** ✅
- c. 0.25
- d. 0.333
#### **16. Among students who studied more than 4 hours, what proportion slept less than 6 hours?**
- a. 0.29
- b. 0.08
- **c. 0.4** ✅
- d. 0.2
#### **17. Which Python code correctly calculates the mean and visualizes `x`?**

- **d. Correct Python code** ✅

---

#### **18. Calculate the relative risk of developing lung cancer for smokers vs. non-smokers.**

- a. 37%
- b. 18%
- **c. 2.6** ✅
- d. 2.3

---

#### **19. Calculate the odds ratio of not developing lung cancer for non-smokers vs. smokers.**

- **a. 3.5** ✅
- b. 6
- c. 1.4
- d. 1.5

---

#### **20. Which of the following is a resistant measure?**

- a. Mean
- b. Standard deviation
- c. Correlation
- **d. Interquartile range** ✅

---

Let me know if you need any modifications or explanations! 😊