## To-DO
I am Person D and am responsible for the areas of the project listed below. This notebook should contain clean, well-commented code and brief markdown explanations for each step. Focus on clear, correct implementation of statistical methods at an undergraduate level.

---

### Renovation Impact Analysis

Create a feature representing **years since last renovation**:
- Derive this using `Year Built` and `Year Remod/Add`
- Replace `Year Remod/Add` with this new feature in the analysis (to avoid redundancy)

Fit a **multiple linear regression model** to predict **log(SalePrice)**:
- Use `log(SalePrice)` instead of raw SalePrice
- Include all relevant predictors (as done in Person B’s notebook) to control for confounding variables
- Ensure preprocessing is applied consistently before modeling

After fitting the model:
- Report the coefficient for the “years since renovation” feature
- Interpret this coefficient as the **association between time since renovation and sale price, holding other variables constant**
- Note: this is an association, not a causal relationship

---

### Temporal Trend Analysis

This section should focus on **clear visual analysis**, not complex modeling.

#### Yearly Trends
- Compute and plot **median sale price by year**
- Use a line plot to visualize how housing prices change over time
- Briefly comment on visible trends (e.g., increases, decreases, possible market shifts)

#### Monthly Trends
- Create **box plots of sale price by month**
- This helps visualize seasonal variation in housing prices
- Optionally, also plot median price by month for a clearer trend line

Keep this section simple, visual, and easy to interpret.

---

### Unsupervised Learning (Clustering)

Perform **K-Means clustering** to identify structure in the housing data.

#### Feature Selection
- Do NOT blindly use all features
- Select a subset of meaningful variables based on dataset documentation, such as:
  - Sale price
  - Living area
  - Overall quality
  - Age / renovation-related features
- Avoid irrelevant or redundant variables (e.g., IDs, sparse categorical features)

#### Preprocessing
- Standardize all selected features before applying K-Means (required)

#### Choosing Number of Clusters (K)
- Use the **elbow method**:
  - Compute within-cluster sum of squares (inertia) for multiple values of K
  - Plot inertia vs K
  - Select K based on the “elbow” point where improvements diminish

#### Model and Interpretation
- Fit K-Means using the chosen K
- For each cluster:
  - Compute summary statistics (mean, standard deviation, quartiles)
- Based on these summaries:
  - Interpret what each cluster represents (e.g., higher-priced vs lower-priced homes)
  - Do NOT assign labels before analyzing results

#### Visualization
- Include scatter plots (if feasible) to visualize cluster separation

---