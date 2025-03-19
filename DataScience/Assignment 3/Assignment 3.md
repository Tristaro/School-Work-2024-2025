# Part 1
## Question 1
![[20250318_213149.jpg]]
![[20250318_213155.jpg]]
![[20250318_213200.jpg]]
## Question 2 & 3
![[20250318_213206.jpg]]
# Part 2
## Question 4
a) The scatterplot of **fish length (x-axis) vs. weight (y-axis)** shows a **positive linear relationship**. As the length of the fish increases, its weight also increases. The pattern appears to be **strong and linear**, meaning the two variables are highly correlated.

b) The Pearson correlation coefficient r between fish length and weight is 0.996.
Since r ≈ 1, there is a very strong positive linear relationship between length and weight.
This means that as fish length increases, weight also increases almost perfectly linearly.

c) After changing the length of ID = 10 to 49.2 cm, the new Pearson correlation coefficient (r) is 0.923.

d) Yes, the correlation decreased from 0.996 to 0.923 after modifying the length of ID = 10.
The new length value (49.2 cm) is much larger than the original (19.74 cm) for that fish.
This change disrupts the natural trend in the data, making it less linear.
The outlier (a fish with an unusual length-to-weight ratio) weakens the overall correlation.
The correlation is still strong but not as perfect as before.
This demonstrates how outliers can significantly affect correlation values.
### Code
```python
# Load dataset
file_path = "Fish.csv"
fish_data = pd.read_csv(file_path)

# Extract length and weight
length = fish_data["Length (in cm)"].values
weight = fish_data["Weight (in grams)"].values

# Part (a): Scatterplot of Length vs. Weight
plt.figure(figsize=(8, 6))
plt.scatter(length, weight, color='orange', edgecolors='black', alpha=0.7)
plt.xlabel("Length (cm)")
plt.ylabel("Weight (grams)")
plt.title("Scatterplot of Fish Length vs. Weight")
plt.show() 

# Part (b): Compute Pearson correlation coefficient
r_value, _ = pearsonr(length, weight)
print(f"Original Pearson correlation coefficient: {r_value:.6f}")  

# Part (c): Modify length for ID = 10 and recalculate r
fish_data.loc[fish_data["ID"] == 10, "Length (in cm)"] = 49.2
modified_length = fish_data["Length (in cm)"].values
modified_r_value, _ = pearsonr(modified_length, weight)
print(f"Modified Pearson correlation coefficient: {modified_r_value:.6f}")

# Part (d): Scatterplot after modification (extra I did for visualization)
plt.figure(figsize=(8, 6))
plt.scatter(modified_length, weight, color='blue', edgecolors='black', alpha=0.7)
plt.xlabel("Length (cm)")
plt.ylabel("Weight (grams)")
plt.title("Scatterplot of Fish Length vs. Weight (Modified)")
plt.show()
```
### Output
![[Screenshot 2025-03-18 221833.png]]
![[Screenshot 2025-03-18 221845.png]]
![[Screenshot 2025-03-18 221902.png]]

## Question 5
a) The slope (m) represents how much the height of a tree increases per year.
The intercept (b) represents the predicted height of a tree when its age is zero.

b) The **coefficient of determination (r<sup>2</sup>)** measures how well the model explains the variation in height based on age.
- A value of **r<sup>2</sup>= 1** means the model **perfectly predicts height**, while **r2=0r^2 = 0r2=0** means age does not explain height at all.
- If r<sup>2</sup>is **high** (close to 1), it means ree height is strongly correlated with age
- If r<sup>2</sup> is **low**, it means other factors affect height more than age does.
### Code

### Output


## Question 6

### Code

### Output
