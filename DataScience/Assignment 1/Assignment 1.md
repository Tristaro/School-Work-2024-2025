# Part 1


# Part 2

## Question 5

```python
[import matplotlib.pyplot as plt

# (b) Drink Pie Chart
# Given soft drink purchase data
soft_drinks = ["Coca-Cola", "Diet Coke", "Dr. Pepper", "Pepsi", "Sprite"]
percentages = [30, 20, 10, 30, 10]  # Percentage distribution of soft drinks
colors = ["red", "brown", "green", "blue", "yellow"]  # Assigning colors to each drink

# Create the pie chart
plt.figure(figsize=(6,6))  # Set figure size
plt.pie(percentages, labels=soft_drinks, autopct='%1.1f%%', colors=colors, startangle=140)

# Add a title
plt.title("Distribution of Soft Drink Purchases")

# Display the pie chart
plt.show()](<# Part (a): Can we use a pie chart?
'''
Yes, you can using a pie chart to show the data because the data represent proportions of a whole (total purchases sum to 100%).
A pie chart is appropriate for showing how each category contributes to the total.
'''
import matplotlib.pyplot as plt

# (b): Drink Pie Chart
# Given soft drink purchase data
soft_drinks = ["Coca-Cola", "Diet Coke", "Dr. Pepper", "Pepsi", "Sprite"]
percentages = [30, 20, 10, 30, 10]  # Percentage distribution of soft drinks
colors = ["red", "brown", "green", "blue", "yellow"]  # Assigning colors to each drink

# Create the pie chart
plt.figure(figsize=(6,6))  # Set figure size
plt.pie(percentages, labels=soft_drinks, autopct='%1.1f%%', colors=colors, startangle=140)

# Add a title
plt.title("Distribution of Soft Drink Purchases")

# Display the pie chart
plt.show()>)
```

## Question 6

```python
[import numpy as np
import matplotlib.pyplot as plt

# Given smartphone ownership data
age_groups = ["18-24", "25-34", "35-44", "45-54", "55-64", "65+"]
smartphone = [55, 70, 67, 32, 25, 18]
other_phone = [30, 26, 36, 32, 51, 24]
no_phone = [2, 5, 7, 11, 17, 53]

# Create a bar chart for age group 25-34
plt.figure(figsize=(6,4))
plt.bar(["Smartphone", "Other Phone", "No Phone"], [70, 26, 5], color=['blue', 'orange', 'gray'])

# Labels and title
plt.xlabel("Phone Type")
plt.ylabel("Percentage")
plt.title("Cell Phone Ownership (Age 25-34)")

# Display the bar chart
plt.show()](<import numpy as np
import matplotlib.pyplot as plt

# Given smartphone ownership data
age_groups = ["18-24", "25-34", "35-44", "45-54", "55-64", "65+"]
smartphone = [55, 70, 67, 32, 25, 18]
other_phone = [30, 26, 36, 32, 51, 24]
no_phone = [2, 5, 7, 11, 17, 53]

# Part (a): Bar Chart for Age Group 25-34
plt.figure(figsize=(6,4))
plt.bar(["Smartphone", "Other Phone", "No Phone"], [70, 26, 5], color=['blue', 'orange', 'gray'])

# Labels and title
plt.xlabel("Phone Type")
plt.ylabel("Percentage")
plt.title("Cell Phone Ownership (Age 25-34)")

# Display the bar chart
plt.show()

# Part (b): Bidimensional Bar Chart for All Age Groups
x = np.arange(len(age_groups))  # X positions

plt.figure(figsize=(8,5))
plt.bar(x - 0.2, smartphone, width=0.2, label="Smartphone", color="blue")
plt.bar(x, other_phone, width=0.2, label="Other Phone", color="orange")
plt.bar(x + 0.2, no_phone, width=0.2, label="No Phone", color="gray")

# Labels and title
plt.xticks(x, age_groups)
plt.xlabel("Age Group")
plt.ylabel("Percentage")
plt.title("Cell Phone Ownership by Age Group")
plt.legend()

# Display the bar chart
plt.show()

# Part (c): Observations
'''
- Younger groups (18-44) have high smartphone ownership (55-70%).
- Older groups (55+) have lower smartphone use and higher "Other Phone" or "No Phone" categories.
- The 65+ group has the highest "No Phone" percentage (53%).
- Overall, smartphone usage declines with age.
'''

print("Younger people use more smartphones, while older age groups have fewer or no cell phones.")>)
```

## Question 7

```python
import pandas as pd
import matplotlib.pyplot as plt

# Load the students' marks dataset
file_path = "students_marks.csv"
students_marks = pd.read_csv(file_path)

# Extract the average marks column
marks = students_marks["Average"]

# (a) Create a histogram with 18 bins
plt.figure(figsize=(8,5))
plt.hist(marks, bins=18, edgecolor='black', alpha=0.7)

# Labels and title
plt.xlabel("Average Marks")
plt.ylabel("Number of Students")
plt.title("Histogram of Students' Average Marks")

# Display the histogram
plt.show()

# (b) Determine the shape of the distribution and count students with marks > 90
shape_description = "Right-skewed" if marks.skew() > 0 else "Left-skewed" if marks.skew() < 0 else "Approximately Normal"
count_above_90 = (marks > 90).sum()

# (c) Compute minimum, maximum, mean, and median marks
min_marks = marks.min()
max_marks = marks.max()
mean_marks = marks.mean()
median_marks = marks.median()

# Print results
print("Distribution Shape:", shape_description)
print("Number of students with marks > 90:", count_above_90)
print("Minimum Marks:", min_marks)
print("Maximum Marks:", max_marks)
print("Mean Marks:", mean_marks)
print("Median Marks:", median_marks)
```

## Question 8

```Python
import pandas as pd
import matplotlib.pyplot as plt

# Load the family size dataset
file_path = "family_size.csv"
family_size_data = pd.read_csv(file_path)

# Extract family sizes for both groups
less_educated = family_size_data.iloc[:, 0].dropna()  # Mothers with ≤6 years of education
more_educated = family_size_data.iloc[:, 1].dropna()  # Mothers with ≥7 years of education

# (a) Side-by-side Boxplots (Fixed Matplotlib Deprecation Warning)
plt.figure(figsize=(8, 5))
plt.boxplot([less_educated, more_educated], tick_labels=["≤6 Years Education", "≥7 Years Education"], patch_artist=True)

# Labels and title
plt.ylabel("Family Size")
plt.title("Comparison of Family Sizes Based on Mother's Education Level")

# Display the boxplot
plt.show()

# (b) Compute Five-Number Summary, Mean, Std Dev, Count
def summary_stats(data):
    return {
        "Min": float(data.min()),
        "Q1": float(data.quantile(0.25)),
        "Median": float(data.median()),
        "Q3": float(data.quantile(0.75)),
        "Max": float(data.max()),
        "Mean": float(data.mean()),
        "Std Dev": float(data.std()),
        "Count": int(data.count())
    }

less_educated_summary = summary_stats(less_educated)
more_educated_summary = summary_stats(more_educated)

# (c) Identifying Outliers using the IQR Rule
def find_outliers(data):
    Q1 = data.quantile(0.25)
    Q3 = data.quantile(0.75)
    IQR = Q3 - Q1
    lower_bound = Q1 - 1.5 * IQR
    upper_bound = Q3 + 1.5 * IQR
    outliers = data[(data < lower_bound) | (data > upper_bound)]
    return sorted(outliers.tolist())

less_educated_outliers = find_outliers(less_educated)
more_educated_outliers = find_outliers(more_educated)

# (d) Interpretation of Education & Family Size Relationship
relationship_observation = (
    "Mothers with less education tend to have larger families, "
    "while those with more education have smaller family sizes on average."
)

# Print results in a clean format
print("\nFamily Size Statistics Based on Mother's Education Level\n")

print("Mothers with ≤6 Years of Education")
for key, value in less_educated_summary.items():
    print(f"   {key}: {value}")

print("\nMothers with ≥7 Years of Education")
for key, value in more_educated_summary.items():
    print(f"   {key}: {value}")

print("\nOutliers in Family Sizes")
print(f"   Mothers with ≤6 Years of Education: {less_educated_outliers if less_educated_outliers else 'None'}")
print(f"   Mothers with ≥7 Years of Education: {more_educated_outliers if more_educated_outliers else 'None'}")

print("\nConclusion:")
print(relationship_observation)
```
