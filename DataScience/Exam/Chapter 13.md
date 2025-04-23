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