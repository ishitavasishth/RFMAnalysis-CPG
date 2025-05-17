# 🛍️ RFM-Based Consumer Segmentation 

This project performs **RFM (Recency, Frequency, Monetary)** analysis using **simulated consumer transaction data** in the CPG space. 

---

## 🧠 Business Goal

To help marketing teams:
- Understand customer purchasing behavior
- Identify valuable, loyal, and at-risk customers
- Enable targeted promotions, retention campaigns, and loyalty programs

---

## 📊 What is RFM?

| Metric     | Definition                                | Why It Matters                       |
|------------|--------------------------------------------|---------------------------------------|
| **Recency**  | Days since the customer’s last purchase     | More recent = more engaged            |
| **Frequency**| Number of purchases made                  | Frequent = loyal                      |
| **Monetary** | Total money spent                         | High spenders = more valuable         |

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy)
- Matplotlib & Seaborn (for visualization)
- Google Colab (runtime environment)
- No APIs or external files — everything is simulated

---

## 📁 Project Workflow

### 1. Simulate Transactional Data
- Created 1000 customers with 1–20 transactions each
- Randomized purchase dates and transaction amounts over 2 years

### 2. RFM Metric Calculation
- **Recency**: Days since the last transaction
- **Frequency**: Total number of purchases
- **Monetary**: Total amount spent

### 3. RFM Scoring
- Each R, F, M score was assigned from 1 (low) to 5 (high) using quantiles

### 4. Customer Segmentation
- RFM scores combined into:
  - `RFM_Score` (sum of all three)
  - `RFM_Segment` (e.g., '545')
- Segments:
  - **Champions** (Score ≥13)
  - **Loyal Customers** (10–12)
  - **Potential Loyalists** (6–9)
  - **At Risk** (<6)

### 5. Visualization
- Countplot showing segment distribution
- Sample RFM table with assigned labels

---

## 📈 Results Snapshot

![RFM Segment Bar Chart](insert-bar-chart-image-path)

| CustomerID | Recency | Frequency | Monetary | RFM Segment | Segment         |
|------------|---------|-----------|----------|-------------|------------------|
| CUST0001   | 264     | 7         | $698.39  | 122         | At Risk          |
| CUST0004   | 84      | 12        | $1213.53 | 234         | Potential Loyalist |
| CUST0005   | 1       | 15        | $1722.59 | 545         | Champions        |

---

## 📌 Key Insights

- Most customers fell into the **Potential Loyalist** and **Loyal Customer** segments.
- **Champions** spent the most and bought frequently with recent activity.
- **At Risk** customers need reactivation strategies (discounts, retargeting).

---

## 🤝 Let’s Connect

Made with curiosity and consumer love by [Ishita Vasishth](https://www.linkedin.com/in/ishitavasishth/)  
🧠 “Marketing without data is like driving with your eyes closed.”

