# Part 1
## Question 1
![[20250318_213149.jpg]]
![[20250318_213155.jpg]]
![[20250318_213200.jpg]]
## Question 2 & 3
![[20250318_213206.jpg]]
# Part 2
## Question 4

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

# Part (d): Scatterplot after modification (optional)
plt.figure(figsize=(8, 6))
plt.scatter(modified_length, weight, color='blue', edgecolors='black', alpha=0.7)
plt.xlabel("Length (cm)")
plt.ylabel("Weight (grams)")
plt.title("Scatterplot of Fish Length vs. Weight (Modified)")
plt.show()
```