## 📚 The Basic Practice of Statistics – Chapters 8–9, 12–13, 15–16, 32 Notes



### Chapter 8: Producing Data – Sampling
Population: Entire group we want information about.  
Sample: Subset of population actually studied.  
Census: Survey of the entire population.  
Sampling Design: How the sample is chosen.  
Bias: Systematic error in design leading to misleading results.  
Random Sampling: Uses chance to select subjects.

Types of Sampling:
- Simple Random Sample (SRS): Equal chance for all individuals/groups.
- Stratified Random Sample: Split population into strata (groups), sample each.
- Cluster Sample: Divide into clusters, randomly choose clusters.
- Multistage Sample: Combines multiple sampling methods.

Sources of Bias:
- Undercoverage: Some groups left out.
- Nonresponse: Selected individuals don’t respond.
- Response Bias: Inaccurate or dishonest answers.
- Question Wording: Leading or unclear questions.

Random Number Table (Table B): Used for SRS selection in exams.



### Chapter 9: Producing Data – Experiments
Observational Study: Observes individuals without influence.  
Experiment: Applies treatment to study cause-and-effect.  
Treatment: Condition applied in an experiment.  
Experimental Units: Subjects of the experiment.  
Factor: Explanatory variable.  
Level: Specific value of a factor.  
Response Variable: Outcome measured.

Principles of Experimental Design:
- Control: Reduce variability.
- Randomization: Use chance.
- Replication: Use enough subjects to detect effects.

Designs:
- Completely Randomized: Random assignment to groups.
- Randomized Comparative: Compare treatments.
- Matched Pairs: Each subject gets both treatments.
- Block Design: Subjects grouped and randomized within blocks.

Key Terms:
- Placebo: Dummy treatment.
- Placebo Effect: Psychological impact of receiving treatment.
- Blinding: Subject/experimenter unaware of treatment.
- Double-Blind: Both unaware.
- Confounding: When variables' effects can't be separated.



### Chapter 12: Introducing Probability
Probability: Likelihood of an event.  
Experiment: Process with outcomes.  
Sample Space (S): All possible outcomes.  
Event: Subset of outcomes.  
Random Phenomenon: Uncertain outcome, predictable pattern.  
Law of Large Numbers: With more trials, observed frequency approaches probability.

Rules of Probability:
- 0 ≤ P ≤ 1
- P(Sample Space) = 1
- Complement Rule: P(Aᶜ) = 1 - P(A)
- Addition Rule (Disjoint): P(A ∪ B) = P(A) + P(B)
- General Addition Rule: P(A ∪ B) = P(A) + P(B) - P(A ∩ B)
- Multiplication Rule (Independent): P(A ∩ B) = P(A) × P(B)
- Conditional Probability: P(A | B) = P(A ∩ B) / P(B)

Discrete vs Continuous:
- Discrete: Countable values (e.g., # of emails).
- Continuous: Measurable range (e.g., time, height).



### Chapter 13: General Rules of Probability
General Addition Rule: For overlapping events.  
Conditional Probability: Probability of A given B.  
General Multiplication Rule: For dependent events.  
Independence: One event doesn’t affect the other.

Key Formulas:
- P(A ∪ B) = P(A) + P(B) - P(A ∩ B)
- P(A | B) = P(A ∩ B) / P(B)
- P(A ∩ B) = P(A) × P(B|A)
- If Independent: P(A ∩ B) = P(A) × P(B)
- Bayes' Rule: P(A|B) = (P(B|A)×P(A)) / P(B)

Tree Diagrams: Visualize probability of compound events.



### Chapter 15: Sampling Distributions
Parameter: Describes population (μ, σ).  
Statistic: Describes sample (x̄).  
Sampling Distribution: Distribution of a statistic over all samples.

Central Limit Theorem (CLT): When n ≥ 30, x̄ ~ Normal regardless of population distribution.

Formulas:
- Mean of x̄: μₓ̄ = μ
- SD of x̄: σₓ̄ = σ / √n
- Z-score: z = (x̄ - μ) / (σ / √n)

Takeaways:
- Larger n → smaller spread
- CLT justifies using Normal models in inference



### Chapter 16: Confidence Intervals
Confidence Interval (CI): Range likely to contain true population parameter.  
Confidence Level: Success rate of the method (e.g., 95%).  
Margin of Error (ME): Max likely error.

CI Formula:
- x̄ ± z × (σ / √n)

Common z Values:
- 90%: 1.645
- 95%: 1.960
- 99%: 2.576

To reduce ME:
- Increase n
- Decrease σ
- Lower confidence level

Conditions:
- SRS
- Normal population or n ≥ 30
- σ known



### Chapter 32: Resampling – Bootstrap and Permutation Tests
Resampling: Use sample data to simulate many hypothetical repetitions.

Bootstrap:
- Draw samples with replacement
- Calculate statistic (e.g., mean)
- Use percentiles to form CI
- 90% CI → 5th to 95th percentiles

Permutation Test:
- Shuffle labels
- Use distribution of shuffled statistics to test H₀

When to Use:
- Bootstrap: Estimating confidence intervals
- Permutation: Hypothesis testing when traditional assumptions fail

Comparison

| Method      | CI  | Hypothesis Test | Assumes Normality |
| ----------- | --- | --------------- | ----------------- |
| Bootstrap   | ✅   | ❌               | ❌                 |
| Permutation | ❌   | ✅               | ❌                 |

Python Example:
```python
import numpy as np
from scipy.stats import norm

# Bootstrap CI
sample = np.array([4, 5, 6, 7])
means = [np.mean(np.random.choice(sample, size=4, replace=True)) for _ in range(1000)]
ci = np.percentile(means, [2.5, 97.5])

# Permutation Test
group1 = np.array([4, 5, 6])
group2 = np.array([7, 8, 9])
obs_diff = np.mean(group1) - np.mean(group2)
combined = np.concatenate([group1, group2])
p_diffs = []
for _ in range(1000):
    np.random.shuffle(combined)
    new_g1 = combined[:3]
    new_g2 = combined[3:]
    p_diffs.append(np.mean(new_g1) - np.mean(new_g2))
p_value = np.mean(np.abs(p_diffs) >= np.abs(obs_diff))
```



