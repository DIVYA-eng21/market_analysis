🛒 Market Basket Analysis with Apriori & FP-Growth

This project performs Market Basket Analysis (MBA) using two powerful algorithms:
Apriori Algorithm
FP-Growth (Frequent Pattern Growth)

Both are used to extract frequent itemsets and generate association rules from a grocery transaction dataset.

📂 Dataset
A transaction-based dataset, where each row represents a transaction and contains items bought together (comma-separated).

Example:

milk,bread,eggs
bread,butter
milk,diapers,beer,eggs

⚙️ Requirements
Install required libraries with:

pip install pandas mlxtend

🧠 Algorithms Used
Apriori

Based on breadth-first search
Generates frequent itemsets from 1-item to k-item sets
Time-consuming for large datasets

FP-Growth (Frequent Pattern Growth)

Uses a tree-based structure (FP-Tree)
More efficient than Apriori on large datasets
Does not generate candidate itemsets
Both are implemented using mlxtend.

📝 How to Run
Load the grocery dataset
Use TransactionEncoder to one-hot encode transactions
Apply both Apriori and FP-Growth to find frequent itemsets
Generate and analyze association rules using support, confidence, and lift metrics

📊 Output
Frequent Itemsets using Apriori & FP-Growth
Association Rules showing relationships like:


With metrics:

Support
Confidence
Lift

📁 Project Structure
Copy
Edit
├── groceries.csv
├── mba_analysis.py
└── README.md

✅ Use-Cases
Product bundling
Recommender systems
Store layout optimization
Market strategy insights

