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
