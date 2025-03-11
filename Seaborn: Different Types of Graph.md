# **Seaborn: Different Types of Graphs with Code Examples 🎨**

Seaborn is a **powerful visualization library** built on Matplotlib, designed for statistical graphics. Below are different types of graphs with **code examples** and **explanations**.

---

## **1️⃣ Line Plot 📈**
Used for **visualizing trends over time**.

### **Example:**
```python
import seaborn as sns
import matplotlib.pyplot as plt
import pandas as pd

data = pd.DataFrame({
    'Days': [1, 2, 3, 4, 5],
    'Sales': [10, 20, 25, 30, 40]
})

sns.lineplot(data=data, x='Days', y='Sales', marker='o')
plt.title('Daily Sales Trend')
plt.show()
```

---

## **2️⃣ Bar Plot 📊**
Used to compare **categorical data**.

### **Example:**
```python
data = pd.DataFrame({
    'Fruits': ["Apple", "Banana", "Orange", "Grapes"],
    'Sales': [50, 80, 30, 60]
})

sns.barplot(data=data, x='Fruits', y='Sales', palette='viridis')
plt.title('Fruit Sales Data')
plt.show()
```

---

## **3️⃣ Histogram 📊**
Used to show **distribution of continuous data**.

### **Example:**
```python
import numpy as np

data = np.random.randn(1000)
sns.histplot(data, bins=30, kde=True, color='blue')
plt.title('Histogram of Random Data')
plt.show()
```

---

## **4️⃣ Scatter Plot 🔵**
Used to show **relationships between two variables**.

### **Example:**
```python
data = pd.DataFrame({
    'Hours Studied': [5, 7, 8, 7, 6, 9, 5, 8, 9, 6],
    'Exam Score': [99, 86, 87, 88, 100, 86, 103, 87, 94, 78]
})

sns.scatterplot(data=data, x='Hours Studied', y='Exam Score', hue='Exam Score', palette='coolwarm')
plt.title('Study Hours vs Exam Score')
plt.show()
```

---

## **5️⃣ Pie Chart 🍕 (Using Matplotlib)**
Seaborn does not support **Pie Charts**, but we can use **Matplotlib**.

### **Example:**
```python
labels = ['Python', 'Java', 'C++', 'JavaScript']
sizes = [40, 25, 20, 15]
colors = sns.color_palette('pastel')

plt.pie(sizes, labels=labels, colors=colors, autopct='%1.1f%%', startangle=140)
plt.title('Programming Language Popularity')
plt.show()
```

---

## **6️⃣ Box Plot 📦**
Used for **visualizing distributions and detecting outliers**.

### **Example:**
```python
data = pd.DataFrame({'Values': [7, 8, 5, 6, 9, 15, 18, 20, 22, 23, 25]})
sns.boxplot(y=data['Values'], color='red')
plt.title('Box Plot Example')
plt.show()
```

---

## **7️⃣ Violin Plot 🎻**
Used to show **distribution density and probability**.

### **Example:**
```python
sns.violinplot(y=data['Values'], color='green')
plt.title('Violin Plot Example')
plt.show()
```

---

## **8️⃣ Heatmap 🔥**
Used to **visualize correlations or matrices**.

### **Example:**
```python
import numpy as np

corr_matrix = np.random.rand(5, 5)
sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
plt.title('Heatmap Example')
plt.show()
```

---

## **🔹 Summary Table**
| Graph Type   | Use Case |
|-------------|---------|
| **Line Plot** | Trends over time |
| **Bar Chart** | Categorical comparisons |
| **Histogram** | Distribution analysis |
| **Scatter Plot** | Relationship between two variables |
| **Pie Chart** | Percentage distribution |
| **Box Plot** | Distribution and outliers |
| **Violin Plot** | Density estimation |
| **Heatmap** | Matrix visualization |

---

🚀 **Now you can create statistical visualizations using Seaborn!**
