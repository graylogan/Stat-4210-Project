# Ames Housing Project (Person D)

## Project Overview
This project uses the Ames Housing dataset, which contains thousands of residential home sales with dozens of features describing physical attributes, quality, location, and sale conditions.

The overall project includes:
- Predicting sale prices using regression models
- Identifying structure in the data using clustering
- Analyzing temporal trends in housing prices
- Additional exploratory and predictive tasks

Your role is **strictly limited to completing the Person D notebook**.

---

## Scope (STRICT)
- Only work inside the **Person D `.ipynb` notebook**
- Only complete the tasks explicitly described in that notebook
- Treat the notebook’s TODO/instructions as the **primary source of truth**
- Do **not** add extra analyses, models, or features unless explicitly requested

If something is unclear, ambiguous, or missing:
> **STOP and ask for clarification before proceeding**
Do NOT make assumptions.

---

## Project Structure & Available Resources

You have access to the following:

### `/src/Dataset/`
- Contains the Ames Housing dataset (`.csv`)
- Includes documentation describing:
  - Feature meanings
  - Valid values
  - Data types
- Use this as the authoritative reference for understanding variables

### `/src/*.ipynb`
- **Person D notebook (your working file)**  
  - Contains TODOs and instructions you must complete  
- **Person B notebook (reference)**  
  - Use this as a guide for:
    - Data preprocessing
    - General workflow patterns

### `/lab-examples`
- Notebooks from *An Introduction to Statistical Learning with Python*
- Use these as references for:
  - Linear regression
  - Clustering methods
  - General modeling patterns
- Reuse patterns, not entire code blindly

### `/agenda.md`
- Contains overall project scope, roles, and required methods
- Use this only for high-level context if needed

---

## Implementation Requirements

### Language & Libraries
- Use **Python**
- Use libraries consistent with lab examples:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `statsmodels`
  - `ISLP`
- Do not introduce unnecessary or advanced libraries

---

## Data Preprocessing Rules (REQUIRED)

The dataset is **not preprocessed**. You must:

1. Drop the following columns:
   - `Order`
   - `PID`

2. Handle missing values:
   - Coerce problematic values to `NaN` if necessary
   - Drop columns that become entirely `NaN`
   - Fill remaining missing values with **column median**

3. Follow **Person B’s notebook** as the reference for preprocessing approach

---

## Code & Notebook Style

### Code
- Write **clear, well-commented code**
- Keep it **simple and readable** (undergraduate level)
- Prefer correctness and clarity over complexity

### Markdown
- Include **brief explanations** between steps:
  - What you are doing
  - Why you are doing it
- Do NOT over-explain or write long essays

---

## Analysis Requirements

### Linear Models
- When fitting regression models:
  - Report **RMSE**
  - Report **model coefficients**
- Use appropriate methods from lab examples (`statsmodels`, etc.)

### Clustering
- Perform clustering as required in the notebook
- Include **visualizations** (e.g., scatter plots of clusters)

### Temporal Analysis
- Analyze trends over time as specified
- Include **clear plots** showing temporal patterns

---

## Ambiguity Handling (VERY IMPORTANT)

If any of the following occur:
- Instructions are unclear
- Multiple valid approaches exist
- Required information is missing

You MUST:
> Ask the user for clarification before proceeding

Do NOT:
- Guess
- Assume intent
- Invent requirements

---

## General Guidance

- Follow instructions in this order of priority:
  1. Person D notebook (highest priority)
  2. This prompt
  3. Person B notebook (reference only)
  4. Lab examples (pattern reference)

- Keep solutions **simple, direct, and functional**
- Avoid unnecessary complexity or advanced techniques

---