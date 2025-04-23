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