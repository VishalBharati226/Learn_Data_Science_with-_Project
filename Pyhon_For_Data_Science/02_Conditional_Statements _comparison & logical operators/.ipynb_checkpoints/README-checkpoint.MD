# ⚡ Electricity Bill Analysis (EDA Mini Project)

## 📌 Project Overview

This is a simple Python project where I built a basic electricity bill calculator using a **slab-based pricing system**.
The goal was to understand how real-world billing works and apply **conditional statements** to solve it.

---

## 🎯 What this project does

* Takes electricity units as input
* Calculates the bill based on slab rates
* Displays the total bill clearly
* Helps understand how billing logic works in real life

---

## 🧠 Concepts I used

* Variables
* `if-elif-else` (conditional statements)
* Basic calculations

---

## ⚙️ Billing Logic

| Units Consumed | Rate         |
| -------------- | ------------ |
| 0 – 100        | ₹5 per unit  |
| 101 – 200      | ₹7 per unit  |
| Above 200      | ₹10 per unit |

💡 Instead of applying a flat rate, this project uses **slab-based calculation**, just like actual electricity bills.

---

## 💻 Code

```python
unit = int(input("Enter electricity units consumed: "))

if unit < 0:
    print("Invalid electricity unit")

elif unit <= 100:
    bill = unit * 5 

elif unit <= 200:
    bill = (100 * 5) + (unit - 100) * 7

else:
    bill = (100 * 5) + (100 * 7) + (unit - 200) * 10

print("Electricity unit consumed is:", unit)
print("Total Electricity Bill is: ₹", bill)
```

---

## 📥 Example

```
Input: 100  
Output: Total Electricity Bill is: ₹500
```

---

## 📊 What I observed

* As units increase, the total bill increases
* Higher usage leads to higher cost
* Slab system makes billing more realistic

---

## ✅ Conclusion

This project helped me understand how to use **conditional logic in a practical scenario**.
It’s a small project, but it builds a strong foundation for solving real-world problems using Python.

---

## 🚀 What I can improve next

* Handle multiple users
* Store and analyze data
* Add graphs using libraries like matplotlib
* Convert it into a proper EDA project

---

## 👨‍💻 Author

**Vishal**
