# Association Rule Mining Lab – MSCS-634

##  Purpose
The purpose of this lab was to apply and compare two key data mining algorithms—**Apriori** and **FP-Growth**—to identify frequent itemsets and generate meaningful association rules from a real-world transactional dataset. This lab helped reinforce concepts in market basket analysis and provided hands-on experience in transforming raw data, mining patterns, and visualizing insights using Python.

##  Key Insights
- **Frequent Itemsets**: Using a minimum support of 0.01, both Apriori and FP-Growth identified common product groupings such as Milk, Auto, Snacks, and Grocery.
- **Association Rule**: A meaningful rule `{Train} → {Auto}` was discovered with a support of ~1.2%, confidence of ~26%, and a lift of 2.59, indicating a strong relationship between these items.
- **Performance**: On a small dataset, the **Apriori algorithm performed faster** than FP-Growth. Although FP-Growth is optimized for larger datasets, its overhead in tree construction can make it slower on smaller datasets.

##  Challenges and Decisions
- **Data Cleaning**: Some entries had missing subcategories, which required dropping rows to ensure algorithm compatibility.
- **Sparse Rule Generation**: Only one strong rule was discovered at the initial confidence threshold. Lowering the confidence might reveal additional patterns.
- **Algorithm Choice**: Maintaining consistent thresholds between Apriori and FP-Growth was essential for fair comparison. It was also a conscious decision to use visualizations (e.g., barplots, scatter plots) to make pattern interpretation easier.

##  Summary
This lab not only demonstrated the technical implementation of association rule mining but also highlighted the importance of preprocessing, algorithm selection, and evaluation metrics (support, confidence, lift) in uncovering valuable insights from data.
