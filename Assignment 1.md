# Part 2

## Question 5

### (a) Can we use a pie chart?
Yes, you can use a pie chart to show the data because the data represents proportions of a whole (total purchases sum to 100%).  
A pie chart is appropriate for showing how each category contributes to the total.

```python
import matplotlib.pyplot as plt

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
plt.show()

import numpy as np
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
plt.xticks(x, age_groups
