# Association Rule mining from transaction dataset

This project performs Association Rule mining on the "Online Retail" dataset from the UCI Machine Learning Repository. It uses the Apriori and FP-Growth algorithms to identify frequent itemsets and generate association rules.

---

### Notebook

The main analysis is contained in the Colab notebook:

* **[Association Rule Mining -  Apriori and FP-Growth.ipynb](Association Rule Mining -  Apriori and FP-Growth.ipynb)**

---

### Project Overview

The 7-step process followed in the notebook is:
1.  **Environment Setup:** Importing `pandas`, `mlxtend`, and `openpyxl`.
2.  **Data Loading:** Reading the data from the `.xlsx` file.
3.  **Data Cleaning:** Removing null values, stripping spaces, and filtering out returns ('C' invoices) and non-product items ('POSTAGE' or 'Manual').
4.  **Data Transformation:** Converting the data into a one-hot encoded transactional format for the 'France' subset.
5.  **Apriori Algorithm:** Finding frequent itemsets with 'min_support=0.01'.
6.  **FP-Growth Algorithm:** Finding the same itemsets more efficiently.
7.  **Association Rule Generation:** Creating rules and filtering them by `lift` and `confidence` to find meaningful patterns.

### Dataset
* **Source:** [UCI Machine Learning Repository: Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

### Key Libraries Used
* pandas
* mlxtend (for Apriori, FP-Growth, and association_rules)
