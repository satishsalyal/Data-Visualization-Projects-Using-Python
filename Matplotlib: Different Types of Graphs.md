# **Matplotlib: Different Types of Graphs with Code Examples 📊**

Matplotlib is a powerful Python library for creating various types of plots. Below are different types of graphs with **code examples** and **explanations**.  

---

## **1️⃣ Line Plot 📈**
Used for **visualizing trends over time**.

### **Example:**
```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 40]

plt.plot(x, y, marker='o', linestyle='-', color='b', label="Sales Trend")
plt.xlabel("Days")
plt.ylabel("Sales")
plt.title("Daily Sales Trend")
plt.legend()
plt.show()
```

---

## **2️⃣ Bar Chart 📊**
Used to compare **categorical data**.

### **Example:**
```python
x = ["Apple", "Banana", "Orange", "Grapes"]
y = [50, 80, 30, 60]

plt.bar(x, y, color=['red', 'yellow', 'orange', 'green'])
plt.xlabel("Fruits")
plt.ylabel("Sales")
plt.title("Fruit Sales Data")
plt.show()
```

---

## **3️⃣ Histogram 📊**
Used to show **distribution of continuous data**.

### **Example:**
```python
import numpy as np

data = np.random.randn(1000)  # 1000 random numbers

plt.hist(data, bins=30, color='blue', edgecolor='black')
plt.xlabel("Value")
plt.ylabel("Frequency")
plt.title("Histogram of Random Data")
plt.show()
```

---

## **4️⃣ Scatter Plot 🔵**
Used to show **relationships between two variables**.

### **Example:**
```python
x = [5, 7, 8, 7, 6, 9, 5, 8, 9, 6]
y = [99, 86, 87, 88, 100, 86, 103, 87, 94, 78]

plt.scatter(x, y, color='red', marker='o')
plt.xlabel("Hours Studied")
plt.ylabel("Exam Score")
plt.title("Study Hours vs Exam Score")
plt.show()
```

---

## **5️⃣ Pie Chart 🍕**
Used to show **percentage distribution**.

### **Example:**
```python
labels = ['Python', 'Java', 'C++', 'JavaScript']
sizes = [40, 25, 20, 15]
colors = ['gold', 'blue', 'red', 'green']

plt.pie(sizes, labels=labels, colors=colors, autopct='%1.1f%%', startangle=140)
plt.title("Programming Language Popularity")
plt.show()
```

---

## **6️⃣ Box Plot 📦**
Used for **visualizing distributions and detecting outliers**.

### **Example:**
```python
data = [7, 8, 5, 6, 9, 15, 18, 20, 22, 23, 25]

plt.boxplot(data)
plt.title("Box Plot Example")
plt.show()
```

---

## **7️⃣ Area Plot 📉**
Used to show **cumulative data over time**.

### **Example:**
```python
days = [1, 2, 3, 4, 5]
sales = [100, 200, 300, 250, 400]

plt.fill_between(days, sales, color='skyblue', alpha=0.5)
plt.plot(days, sales, color='blue', linestyle='dashed')
plt.xlabel("Days")
plt.ylabel("Sales")
plt.title("Sales Growth Over Days")
plt.show()
```

---

## **8️⃣ Heatmap 🔥**
Used to **visualize correlations or matrices**.

### **Example:**
```python
import seaborn as sns
import numpy as np

data = np.random.rand(5, 5)
sns.heatmap(data, cmap="coolwarm", annot=True)
plt.title("Heatmap Example")
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
| **Area Plot** | Cumulative trends |
| **Heatmap** | Matrix visualization |

---

🚀 **Now you can visualize data effectively using Matplotlib!**
