```markdown
# 📂 CSV Files with Pandas (Day 17)

Learned how to save and load data in **CSV format** with Pandas.  
CSV = Comma-Separated Values, a simple text-based format for tables.

---

## 📌 Features
- Create DataFrame with product data
- Save DataFrame to `products.csv`
- Load CSV back into Python
- Print loaded data

---

## ▶️ Example run
```python
import pandas as pd

data = {
    "Product": ["Apple", "Banana", "Orange"],
    "Price": [1.2, 0.8, 1.5],
    "Quantity": [10, 25, 15]
}

df = pd.DataFrame(data)
df.to_csv("products.csv", index=False)

new_df = pd.read_csv("products.csv")
print(new_df)
📊 Example output
mathematica
Copy code
  Product  Price  Quantity
0   Apple    1.2        10
1  Banana    0.8        25
2  Orange    1.5        15
✨ This project is part of my Python learning journey (Day 17).
