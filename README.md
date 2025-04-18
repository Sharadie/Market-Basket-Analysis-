# Market-Basket-Analysis-
# 🛒 Market Basket Analysis using Association Rule Mining

This project applies **Market Basket Analysis** using the **Apriori algorithm** to discover association rules between products (in this case, *aisles*) for targeted marketing strategies.

Since the provided dataset (`10. Market Basket Analysis.csv`) includes only aisle categories, we simulate transactions to demonstrate the association rule mining process.

---

## 📁 Dataset

The dataset contains the following columns:

- `aisle_id`: Unique identifier for each aisle
- `aisle`: Name/description of the aisle (e.g., "energy granola bars", "instant foods")

> ⚠️ Note: This dataset does not contain real transactional data, so transactions are synthetically generated for demo purposes.

---

## ⚙️ How It Works

1. **Load and Preview Data**  
   Load the CSV file and view the list of aisle names.

2. **Simulate Transactions**  
   Randomly generate 100 transactions with 2–5 aisles each.

3. **Preprocessing**  
   Convert the transactions to one-hot encoding format.

4. **Apply Apriori Algorithm**  
   Identify frequent itemsets with a minimum support threshold.

5. **Generate Association Rules**  
   Extract rules using `lift` as the primary metric.

6. **Display Results**  
   View the top 10 association rules with support, confidence, and lift.

---

## 📌 Libraries Used

- `pandas` – Data manipulation
- `mlxtend` – Apriori and association rule mining
- `random` – Simulate transactions
- `google.colab` – File upload handling

Install required packages:

```bash
pip install mlxtend
Top 10 Association Rules:
antecedents         consequents        support  confidence  lift
---------------     -------------      -------  ----------  ------
('item A')          ('item B')         0.15     0.70        1.50
('item C', 'D')     ('item E')         0.12     0.65        2.10
...

---


