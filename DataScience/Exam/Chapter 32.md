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