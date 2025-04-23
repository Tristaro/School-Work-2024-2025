Here are structured notes for **Chapter 8: Producing Data – Sampling** from _The Basic Practice of Statistics (9th ed)_, covering key terms, formulas, examples, and exam-relevant content.

---

## 📘 Chapter 8: Producing Data – Sampling

### 🎯 Key Concepts and Definitions

|Term|Definition|
|---|---|
|**Population**|The entire group of individuals about which we want information.|
|**Sample**|A part of the population from which we actually collect data.|
|**Census**|A survey that attempts to include the entire population.|
|**Sampling Design**|The method used to choose the sample from the population.|
|**Bias**|A systematic error in the sampling method that leads to an incorrect estimate.|
|**Random Sampling**|Using chance to determine which members of a population are selected.|

---

### 🔢 Types of Sampling

|Method|Description|Example|
|---|---|---|
|**Simple Random Sample (SRS)**|Every individual and every group of individuals has an equal chance of being selected.|Assign a number to each student, then use a random number generator to pick 10.|
|**Stratified Random Sample**|Divide the population into strata (groups) and take an SRS from each stratum.|Split by year of study (first-year, second-year...), sample from each.|
|**Cluster Sample**|Divide the population into clusters, randomly select clusters, then sample all individuals in selected clusters.|Select dorms as clusters and survey all students in selected dorms.|
|**Multistage Sample**|Combine several sampling methods (e.g., choose schools, then students).|Choose schools → choose classes → choose students.|

---

### 🚫 Sources of Bias

|Bias Type|Description|Example|
|---|---|---|
|**Undercoverage**|Some groups in the population are left out of the sampling frame.|Homeless people in a phone survey.|
|**Nonresponse**|Individuals selected for the sample don’t respond.|People not answering a mailed survey.|
|**Response Bias**|Respondents may lie or give inaccurate answers.|People underreporting illegal behavior.|
|**Question Wording**|The phrasing of questions may lead to bias.|“Do you agree that…” vs. “What is your opinion on…”|

---

### ⚙️ Techniques and Tools

#### 🧮 Random Number Table (Table B)

- Used for SRS selection.
    
- Randomly choose starting point and move in a consistent direction.
    
- Useful for exam short-answer questions.
    

**Example**:  
You want a random sample of 4 from a class of 50. Use Table B starting at line 101. Select 2-digit numbers between 01 and 50, skipping repeats and invalid numbers.

---

### 📌 Key Takeaways

1. **Random sampling** avoids bias and gives each individual a fair chance.
    
2. **Stratified sampling** improves accuracy when population has distinct subgroups.
    
3. **Cluster sampling** is cost-effective but may be less accurate.
    
4. **Biases** can seriously distort survey results and should be identified and minimized.
    
5. **Non-statistical issues** like question wording or data collection methods (internet vs. phone) affect quality.
    

---

### 🧠 Practice Concept

> **Q:** What is the main advantage of stratified random sampling over simple random sampling?  
> **A:** It ensures representation from each subgroup, which can reduce variability in the results.

---

Would you like me to continue with **Chapter 9** next, or would you prefer this exported into Obsidian/Markdown format first?

Here are notes for **Chapter 9: Producing Data – Experiments** from _The Basic Practice of Statistics (9th ed)_, tailored to your exam.

---

## 📘 Chapter 9: Producing Data – Experiments

### 🎯 Key Concepts

|Term|Definition|
|---|---|
|**Observational Study**|Observes individuals and measures variables without attempting to influence them.|
|**Experiment**|Deliberately imposes a treatment to measure responses and infer cause-and-effect.|
|**Treatment**|A specific condition applied to individuals in an experiment.|
|**Experimental Units**|Individuals on which the experiment is done (often called **subjects** when human).|
|**Factor**|An explanatory variable in an experiment.|
|**Level**|A specific value of a factor.|
|**Response Variable**|The outcome measured in the experiment.|

---

### 🔬 Principles of Experimental Design

1. **Control**
    
    - Reduce effects of lurking variables.
        
    - Example: Keep environment consistent for all subjects.
        
2. **Randomization**
    
    - Use chance to assign treatments.
        
    - Avoids bias and balances out unknown factors.
        
3. **Replication**
    
    - Use enough subjects so treatment effects can be distinguished from chance variation.
        

---

### 🧪 Experimental Designs

|Design|Description|Example|
|---|---|---|
|**Completely Randomized Design**|All subjects are randomly assigned to treatment groups.|100 subjects randomly assigned to placebo or drug.|
|**Randomized Comparative Experiment**|Compares two or more treatments using random assignment.|Compare effectiveness of two study methods.|
|**Matched Pairs Design**|Each subject receives both treatments in a random order, or subjects are paired.|Taste test: each person tries both Coke and Pepsi.|
|**Block Design**|Subjects are grouped into blocks, and random assignment occurs within each block.|Group by gender before assigning treatments.|

---

### 🧠 Important Terms

|Term|Meaning|
|---|---|
|**Placebo**|A dummy treatment with no active ingredient.|
|**Placebo Effect**|Positive results due to belief in treatment.|
|**Blinding**|Subjects or experimenters do not know which treatment was received.|
|**Double-Blind**|Neither subjects nor experimenters know the treatment assignments.|
|**Confounding**|When effects of two variables cannot be distinguished from each other.|

---

### ⚠️ Common Pitfalls

- **Lack of random assignment** ➜ Cannot infer causation.
    
- **Observational studies** ➜ Can show association, not cause-and-effect.
    
- **Small sample size** ➜ Low power to detect effects, risk of over-interpreting chance variation.
    

---

### 🧠 Example Q&A for Practice

> **Q:** Why is replication important in an experiment?  
> **A:** To ensure that the observed effect is not due to random chance.

> **Q:** What's the difference between a block and a stratum?  
> **A:** In sampling (Chapter 8), you stratify. In experiments (Chapter 9), you block. Both control variation by grouping similar individuals — but one is for surveys, the other for treatment studies.

> **Q:** Can you infer causation from an observational study?  
> **A:** No. You can only infer association.

---

Let me know when you're ready to continue with **Chapter 12**.

Here are your tailored notes for **Chapter 12: Introducing Probability** from _The Basic Practice of Statistics (9th ed)_.

---

## 📘 Chapter 12: Introducing Probability

### 🎯 Why Probability?

Probability provides the foundation for **statistical inference**—since we often study a sample to understand a population, we need a way to **quantify the uncertainty** of our results.

---

### 🔑 Key Terms

|Term|Definition|
|---|---|
|**Probability**|A measure of how likely an event is to occur.|
|**Experiment**|A process that leads to a well-defined result.|
|**Sample Space (S)**|The set of all possible outcomes.|
|**Event**|A subset of the sample space; a collection of outcomes.|
|**Probability Model**|A description of a random phenomenon in the form of a sample space and probabilities.|
|**Law of Large Numbers**|As the number of repetitions increases, the relative frequency of an event approaches the true probability.|
|**Random Phenomenon**|An event where the outcome is uncertain but follows a pattern in many repetitions.|

---

### 📐 Rules of Probability

1. **Probability is a number between 0 and 1**
    
    - 0 = impossible, 1 = certain
        
2. **All outcomes together must have probability 1**
    
3. **Complement Rule**:
    
    P(Ac)=1−P(A)P(A^c) = 1 - P(A)
4. **Addition Rule (Disjoint Events)**:
    
    P(A∪B)=P(A)+P(B)if A and B are disjointP(A \cup B) = P(A) + P(B) \quad \text{if } A \text{ and } B \text{ are disjoint}
5. **General Addition Rule**:
    
    P(A∪B)=P(A)+P(B)−P(A∩B)P(A \cup B) = P(A) + P(B) - P(A \cap B)
6. **Multiplication Rule (Independent Events)**:
    
    P(A∩B)=P(A)×P(B)if A and B are independentP(A \cap B) = P(A) \times P(B) \quad \text{if } A \text{ and } B \text{ are independent}
7. **Conditional Probability**:
    
    P(A∣B)=P(A∩B)P(B)P(A | B) = \frac{P(A \cap B)}{P(B)}

---

### 🎲 Probability Models

- **Finite Sample Space**: e.g., rolling a die:
    
    S={1,2,3,4,5,6},P(i)=16S = \{1, 2, 3, 4, 5, 6\},\quad P(i) = \frac{1}{6}
- **Continuous Sample Space**: e.g., time, height
    
    - Use **density curves**.
        
    - Probability is an **area under the curve**.
        
    - Total area under the curve = 1.
        

---

### 📊 Discrete vs Continuous

|Type|Description|Example|
|---|---|---|
|**Discrete Random Variable**|Takes on countable values|# of calls in an hour|
|**Continuous Random Variable**|Takes values in an interval|Height, time, weight|

---

### 🔢 Example

**Example:**  
A spinner has equal sections labeled 1 through 5.

- What’s the probability of spinning a 2 or a 4?
    
- P(2∪4)=P(2)+P(4)=15+15=25P(2 \cup 4) = P(2) + P(4) = \frac{1}{5} + \frac{1}{5} = \frac{2}{5}
    

---

### 📐 Table Summary: Rules & Formulas

|Rule|Formula|
|---|---|
|Complement|P(Ac)=1−P(A)P(A^c) = 1 - P(A)|
|Disjoint Addition|P(A∪B)=P(A)+P(B)P(A \cup B) = P(A) + P(B)|
|General Addition|P(A∪B)=P(A)+P(B)−P(A∩B)P(A \cup B) = P(A) + P(B) - P(A \cap B)|
|Multiplication (Indep.)|P(A∩B)=P(A)⋅P(B)P(A \cap B) = P(A) \cdot P(B)|
|Conditional|( P(A|

---

Let me know when you're ready to continue to **Chapter 13**.

Here are notes for **Chapter 13: General Rules of Probability** from _The Basic Practice of Statistics (9th ed)_—building on the basics from Chapter 12 to handle **compound events, conditional probabilities, and independence**.

---

## 📘 Chapter 13: General Rules of Probability

### 🔑 Key Topics Covered

|Concept|Description|
|---|---|
|**General Addition Rule**|For overlapping events|
|**Conditional Probability**|Probability of an event given another has occurred|
|**General Multiplication Rule**|For dependent events|
|**Independence**|When knowing one event does not change the probability of the other|
|**Tree Diagrams**|Visual tool for sequential probabilities|
|**Bayes' Rule**|Reverse conditional probability calculation|

---

### ➕ General Addition Rule

Use this when events **A and B are not disjoint**:

P(A∪B)=P(A)+P(B)−P(A∩B)P(A \cup B) = P(A) + P(B) - P(A \cap B)

- Subtract P(A∩B)P(A \cap B) to correct for double-counting.
    

---

### 📐 Conditional Probability

The probability of **event A given B has occurred**:

P(A∣B)=P(A∩B)P(B)P(A|B) = \frac{P(A \cap B)}{P(B)}

- Think of it as **restricting** the sample space to event B.
    

---

### ✖️ General Multiplication Rule

No assumption of independence:

P(A∩B)=P(A)⋅P(B∣A)P(A \cap B) = P(A) \cdot P(B|A)

Compare this to **independent case**:

P(A∩B)=P(A)⋅P(B)P(A \cap B) = P(A) \cdot P(B)

---

### 🧠 Independence

- **Independent** events: Knowing one does not change the probability of the other.
    
- Check:
    
    P(B)=P(B∣A)andP(A∩B)=P(A)⋅P(B)P(B) = P(B|A) \quad \text{and} \quad P(A \cap B) = P(A) \cdot P(B)

---

### 🌳 Tree Diagrams

- Show **all outcomes** and **probabilities** for sequential events.
    
- Multiply along branches for **joint probabilities**.
    
- Can show conditional structure clearly.
    

---

### 📊 Bayes' Rule

Used when reversing conditional probability (e.g., updating beliefs):

P(A∣B)=P(B∣A)⋅P(A)P(B)P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}

Where:

P(B)=P(B∣A)⋅P(A)+P(B∣Ac)⋅P(Ac)P(B) = P(B|A) \cdot P(A) + P(B|A^c) \cdot P(A^c)

---

### 🧮 Example

**Example:**  
In a class, 60% are male, 40% female. 70% of males and 90% of females pass.  
What's the probability a student who passed is female?

Let:

- M=maleM = \text{male}
    
- F=femaleF = \text{female}
    
- P=passP = \text{pass}
    

P(F∣P)=P(P∣F)⋅P(F)P(P∣M)⋅P(M)+P(P∣F)⋅P(F)=0.90⋅0.400.70⋅0.60+0.90⋅0.40=0.360.42+0.36=0.360.78≈0.46P(F|P) = \frac{P(P|F) \cdot P(F)}{P(P|M) \cdot P(M) + P(P|F) \cdot P(F)} \\ = \frac{0.90 \cdot 0.40}{0.70 \cdot 0.60 + 0.90 \cdot 0.40} = \frac{0.36}{0.42 + 0.36} = \frac{0.36}{0.78} \approx 0.46

---

### 📌 Summary Table

|Rule|Formula|
|---|---|
|General Addition|P(A∪B)=P(A)+P(B)−P(A∩B)P(A \cup B) = P(A) + P(B) - P(A \cap B)|
|Conditional|( P(A|
|General Multiplication|( P(A \cap B) = P(A) \cdot P(B|
|Independence|P(A∩B)=P(A)⋅P(B)P(A \cap B) = P(A) \cdot P(B)|
|Bayes' Rule|( P(A|

---

Let me know when to continue with **Chapter 15**!

Here are your exam-focused notes for **Chapter 15: Sampling Distributions** from _The Basic Practice of Statistics (9th ed)_.

---

## 📘 Chapter 15: Sampling Distributions

### 🧠 Why This Matters

Sampling distributions link **probability** with **inference**: they describe how a statistic (like a sample mean) varies across samples. This is key for estimating population parameters and measuring uncertainty.

---

### 🔑 Key Terms

|Term|Definition|
|---|---|
|**Parameter**|A number that describes the population (e.g., μ for mean).|
|**Statistic**|A number that describes a sample (e.g., xˉ\bar{x}).|
|**Sampling Distribution**|The distribution of a statistic across all possible samples of a given size.|
|**Unbiased Estimator**|A statistic whose sampling distribution is centered on the true parameter.|
|**Variability**|Refers to how spread out the sampling distribution is.|
|**Standard Deviation of xˉ\bar{x}**|σxˉ=σn\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}, where σ is population SD and n is sample size.|

---

### 📈 The Central Limit Theorem (CLT)

One of the most important results in statistics:

> **If the sample size n is large enough**, the distribution of xˉ\bar{x} will be approximately **Normal**, even if the population distribution is not.

- This is the **foundation** of many inference techniques.
    
- A common rule of thumb: **n ≥ 30** is usually large enough.
    

---

### 🧮 Key Formulas

|Concept|Formula|
|---|---|
|Mean of sampling distribution|μxˉ=μ\mu_{\bar{x}} = \mu|
|SD of sampling distribution|σxˉ=σn\sigma_{\bar{x}} = \frac{\sigma}{\sqrt{n}}|
|Standardized z-score|z=xˉ−μσ/nz = \frac{\bar{x} - \mu}{\sigma/\sqrt{n}}|

---

### 📊 Example

A population has μ = 50, σ = 10. A sample of size n = 25 is taken.

- What is the mean and SD of xˉ\bar{x}?
    
    - Mean = 50
        
    - SD = 1025=2\frac{10}{\sqrt{25}} = 2
        
- What is the probability that xˉ≥54\bar{x} \geq 54?
    
    - z=54−502=2z = \frac{54 - 50}{2} = 2
        
    - Use **Table A**: P(xˉ≥54)=P(z≥2)=1−0.9772=0.0228P(\bar{x} \geq 54) = P(z \geq 2) = 1 - 0.9772 = 0.0228
        

---

### ⚠️ Important Ideas

- The **larger the sample size**, the **smaller** the variability in the sampling distribution.
    
- **Bias** affects **center**, **variability** affects **spread**.
    
- The **CLT** lets us use normal probability to model sample means when n is large.
    

---

### 🔍 Quick Review: Terms Summary

|Term|Symbol|Description|
|---|---|---|
|Population Mean|μ|Center of the population|
|Sample Mean|xˉ\bar{x}|Estimate of μ|
|Population SD|σ|Spread of the population|
|Sample SD of mean|σxˉ\sigma_{\bar{x}}|Spread of the sampling distribution|
|Sampling Distribution Shape|~Normal if n is large|Thanks to the CLT|

---

Let me know when you're ready for **Chapter 16**!

Here are your focused notes for **Chapter 16: Confidence Intervals – The Basics** from _The Basic Practice of Statistics (9th ed)_.

---

## 📘 Chapter 16: Confidence Intervals – The Basics

### 🎯 Goal of the Chapter

To **estimate a population parameter** (like the mean) using a **sample statistic** and to **quantify uncertainty** with a **margin of error**.

---

### 🔑 Key Terms

|Term|Definition|
|---|---|
|**Statistical Inference**|Drawing conclusions about a population from a sample.|
|**Confidence Interval (CI)**|A range of values likely to contain the population parameter.|
|**Confidence Level**|The success rate (e.g., 95%) of the method over many samples.|
|**Margin of Error (ME)**|The maximum expected difference between the statistic and the true parameter.|

---

### 📐 Structure of a Confidence Interval

Estimate±Margin of Error\text{Estimate} \pm \text{Margin of Error}

For a population mean (μ) when population σ is known:

xˉ±z∗⋅σn\bar{x} \pm z^* \cdot \frac{\sigma}{\sqrt{n}}

- xˉ\bar{x}: sample mean
    
- σ\sigma: population standard deviation
    
- nn: sample size
    
- z∗z^*: critical value from standard normal (Z) table for given confidence level
    

---

### 📊 Common z∗z^* Values

|Confidence Level|z∗z^*|
|---|---|
|90%|1.645|
|95%|1.960|
|99%|2.576|

---

### 🧮 Example

Suppose:

- Sample mean = 72
    
- σ = 8
    
- n = 36
    
- 95% CI
    

ME=1.96⋅836=1.96⋅86=1.96⋅1.33≈2.61ME = 1.96 \cdot \frac{8}{\sqrt{36}} = 1.96 \cdot \frac{8}{6} = 1.96 \cdot 1.33 \approx 2.61 CI=72±2.61=(69.39, 74.61)\text{CI} = 72 \pm 2.61 = (69.39,\ 74.61)

---

### ✅ Conditions for Using This Method

1. **SRS** from population
    
2. Population is **Normal**, or n is **large (≥30)**
    
3. Population standard deviation σ\sigma is **known** (this is a simplification – often not true in real life)
    

---

### 📉 How to Reduce Margin of Error

|Strategy|Result|
|---|---|
|Increase confidence level (e.g., from 90% → 95%)|Increases ME|
|Decrease σ (less variability)|Decreases ME|
|Increase n (larger sample size)|Decreases ME|

---

### 🧠 Key Ideas

- Confidence intervals don't tell you the probability the parameter is in the interval—they tell you how confident you are in your method.
    
- Wider intervals = more confidence, less precision.
    
- Smaller intervals = less confidence, more precision.
    

---

Let me know when you're ready to move on to the final chapter for your exam: **Chapter 32**!

Here are your exam-ready notes for **Chapter 32: Resampling – Bootstrap and Permutation Tests** from _The Basic Practice of Statistics (9th ed)_.

---

## 📘 Chapter 32: Resampling – Bootstrap and Permutation Tests

### 🎯 Why This Chapter Matters

This chapter introduces **modern computational inference** techniques—**bootstrap** and **permutation** methods—that allow statistical inference **without strong assumptions** like normality or known formulas.

---

### 🔑 Key Terms

|Term|Definition|
|---|---|
|**Resampling**|Using the sample data to simulate many hypothetical repetitions.|
|**Permutation Test**|Tests the null hypothesis by randomly reassigning group labels.|
|**Bootstrap Method**|Estimates sampling distribution by sampling with replacement from the sample.|
|**Bootstrap Distribution**|The distribution of a statistic from many bootstrap samples.|
|**Bootstrap Percentile Interval**|Confidence interval based on percentiles of the bootstrap distribution.|

---

### 🔁 Permutation Tests

- Used in **randomized experiments**.
    
- Idea: If the null hypothesis is true, the **group labels don't matter**.
    
- Randomly shuffle group labels many times and recompute the test statistic.
    
- Compare the observed statistic to this **permutation distribution**.
    

**Use when**:

- Comparing two groups (means, medians, etc.)
    
- Traditional assumptions (e.g., Normality) are not met
    

---

### 📊 Bootstrap Method

- Simulates the sampling distribution of a statistic by **resampling with replacement** from the observed sample.
    
- We use this distribution to build **confidence intervals** or test hypotheses.
    

#### Steps:

1. Take **many samples with replacement** from your data (same size as original).
    
2. Compute the statistic (e.g., mean) for each sample.
    
3. Use the distribution of those statistics as an approximation of the sampling distribution.
    

#### Bootstrap Percentile Interval:

- A **confidence interval** using cutoffs from the bootstrap distribution.
    
- For 95% CI → Use the 2.5th and 97.5th percentiles.
    

---

### 🧮 Example (Bootstrap CI)

You want a 90% CI for the mean:

- Bootstrap 10,000 samples
    
- Sort the means
    
- CI = [5th percentile, 95th percentile] of those bootstrap means
    

---

### ✅ Benefits

|Feature|Bootstrap|Permutation|
|---|---|---|
|Doesn’t assume Normality|✅|✅|
|Good for small samples|⚠️ (can be unstable)|⚠️|
|Tests hypotheses|❌ (used for estimation)|✅|
|Builds confidence intervals|✅|❌|

---

### 🧠 Important Concepts

- Traditional inference assumes specific formulas; these methods are **data-driven**.
    
- Both methods use the **observed data** as a **model of the population**.
    
- Rely on **software** for calculations due to repetition.
    

---

### 🧪 Python-Style Usage (for MC/Python parts)

```python
import numpy as np

# Bootstrap
sample = np.array([4, 5, 6, 7])
bootstrap_means = [np.mean(np.random.choice(sample, size=len(sample), replace=True)) for _ in range(1000)]
ci_lower, ci_upper = np.percentile(bootstrap_means, [2.5, 97.5])

# Permutation test
group1 = np.array([4, 5, 6])
group2 = np.array([7, 8, 9])
observed_diff = np.mean(group1) - np.mean(group2)

combined = np.concatenate([group1, group2])
permuted_diffs = []
for _ in range(1000):
    np.random.shuffle(combined)
    new_g1 = combined[:len(group1)]
    new_g2 = combined[len(group1):]
    permuted_diffs.append(np.mean(new_g1) - np.mean(new_g2))

p_value = np.mean(np.abs(permuted_diffs) >= np.abs(observed_diff))
```

---

Let me know if you want a **condensed cheat sheet**, **Obsidian export**, or want to run through some **sample exam questions** next!****

