# ![Project Header Image](images/project_header_img.png)

## Food Price Inflation Analysis
***A data-driven analysis of food price inflation***

---

### Executive Summary
This project explores global food price inflation using the Monthly Food Price Estimates dataset from Kaggle.
Our goal was to understand the drivers of food inflation, test hypotheses about volatility and crisis effects, and evaluate the robustness of the data. The analysis provides an evidence-based foundation for communicating results through an interactive dashboard in Power BI.

Key findings:
A small set of countries face extreme inflation and volatility, often linked to crises.
Price volatility amplifies inflationary pressures, making markets unstable.
Data coverage does not bias results, increasing confidence in findings.

### Dataset Content


### Business Requirements
The analysis aims to:  
1. Identify **patterns and drivers** of food price inflation.  
2. Test whether **volatility and crises** are associated with higher inflation.  
3. Assess whether **data coverage** biases inflation outcomes.  
4. Provide an **evidence base for stakeholders** via an interactive dashboard.

### Hypotheses
In order to better understand the drivers of food price inflation, we propose the following hypotheses:

### H1 – Geopolitical Unrest and Inflation
- **Null Hypothesis:** There is no relationship between geopolitical unrest or crises and food inflation rates.  
- **Alternative Hypothesis:** Countries experiencing greater geopolitical unrest or crises will have higher food inflation rates.  
- **Rationale:** Conflict disrupts supply chains, weakens currencies, and raises import costs. Outliers such as Lebanon, South Sudan, and Syria suggest that crises may drive extreme inflation.

---

### H2 – Volatility and Inflation
- **Null Hypothesis:** Food price volatility is independent of food inflation rates.  
- **Alternative Hypothesis:** Countries with higher average annualized food price volatility will also have higher inflation rates.  
- **Rationale:** Unstable markets often face upward price pressures. Our scatter plot indicates a moderate positive relationship between volatility and inflation, with countries like Lebanon and Sudan showing both high inflation and volatility.

---

### H3 – Data Coverage and Inflation
- **Null Hypothesis:** Inflation outcomes are influenced by the level of data coverage.  
- **Alternative Hypothesis:** Inflation outcomes are independent of data coverage levels.  
- **Rationale:** If countries with low data coverage systematically showed extreme inflation, results would be questionable. However, our analysis shows extreme inflation even in countries with high coverage, suggesting that inflation results reflect real economic pressures.

---

**Summary:**  
- **H1** explores external, real-world drivers of inflation (geopolitical unrest).  
- **H2** tests an internal relationship within the dataset (volatility vs inflation).  
- **H3** checks data robustness by ruling out potential bias from coverage.

---

### Project Plan
- **Data Cleaning & Feature Engineering**  
  - Verified no missing values or duplicates.  
  - Converted date fields into usable formats.  
  - Engineered derived metrics (absolute drawdowns).  

- **Exploratory Data Analysis**  
  - Univariate analysis of inflation distributions and outliers.  
  - Bivariate testing for volatility, crises, and data coverage effects.  
  - Visual storytelling with bar charts, scatter plots, and boxplots.  

- **Hypothesis Testing**  
  - Assessed evidence qualitatively and quantitatively.  
  - Visualised extreme cases (e.g., Lebanon, Sudan).  

- **Dashboard Creation (Power BI)**  
  - Designed an interactive dashboard summarising inflation trends, country comparisons, and volatility patterns.  

# Data Analysis Summary

In this project, we explored a dataset on **food price inflation** across multiple countries.  
Our analysis followed these main steps:

1. **Data Cleaning & Preparation**
   - Loaded the dataset and parsed the '*date'* column into a usable format.
   - Checked for missing values and duplicates (none found).
   - Verified data types and created a new column for absolute drawdown values.
   - Confirmed data coverage and consistency across countries.

2. **Hypotheses Formulation**
   - **H1:** Countries facing geopolitical unrest will have higher food inflation.  
   - **H2:** Countries with higher food price volatility will also have higher inflation.  
   - **H3:** Inflation outcomes are independent of data coverage levels.

3. **Univariate Analysis**
   - Examined the distribution of food inflation: **positively skewed**, with most countries at low/moderate inflation but a few extreme outliers (e.g., Lebanon at 139%).  
   - Identified several countries in **deflation** (e.g., Burkina Faso, Somalia, Mali).  
   - Summarised key statistics for volatility, drawdown, and coverage.

4. **Bivariate Analysis & Hypothesis Testing**
   - **H1:** Visualised inflation by country, highlighting crisis nations. Found strong qualitative evidence that unrest is linked to high inflation.  
   - **H2:** Scatter plot of inflation vs volatility showed a positive trend, supporting the hypothesis.  
   - **H3:** Scatter plot of inflation vs data coverage showed no systematic bias, supporting data robustness.

5. **Conclusions**
   - Food inflation is highly uneven across countries: most are stable, but a few face extreme crises.  
   - High inflation is often paired with high volatility, compounding instability.  
   - Past drawdowns do not predict current inflation.  
   - Inflation outcomes are not explained by data coverage, strengthening confidence in results.

---

This analysis provides a **clear evidence base** for communicating global food inflation patterns and supports the development of an accessible dashboard for stakeholders.

- **Hypothesis Testing Summary**

We tested three hypotheses using our dataset. The results are summarised below:

### H1 - Geopolitical Unrest and Inflation
- **Result:** Supported qualitatively.  
- Crisis-affected countries (**Lebanon, South Sudan, Syria, Myanmar, Haiti**) are clustered at the top of the inflation distribution.  
- This aligns with global reporting that political/economic instability drives food inflation.  
- Even without a direct “conflict” variable, the evidence suggests unrest is strongly linked to extreme inflation outcomes.

![H1 Plot](images/h1_food_inflation_by_crisis_countries.png)
---

### H2 - Volatility and Inflation
- **Result:** Supported.  
- A moderate positive trend is observed: higher food price volatility is associated with higher inflation.  
- Example: **Lebanon, South Sudan, and Sudan** show both high inflation and high volatility, while stable markets like **Cameroon and Iraq** show low levels of both.  
- This reinforces that **price surges often come with instability**.

![H2 Plot](images/h2_inflation_vs_food_price_volatility.png)
---

### H3 - Data Coverage and Inflation
- **Result:** Supported.  
- Extreme inflation outcomes appear even in countries with relatively high coverage.  
- Low coverage countries do not systematically show more extreme values.  
- Suggests that results are **robust** and not driven by data artefacts.

![H3 Plot](images/h3_inflation_vs_data_coverage.png)
---

## Overall Conclusion
- **Food inflation is not evenly distributed**: most countries are stable, but a small set of crisis-affected nations face extreme inflation and volatility.  
- **Volatility amplifies inflation pressures**, highlighting that price surges are also unstable and unpredictable.  
- **Data coverage does not bias results**, increasing confidence in our findings.  

These insights provide a clear, evidence-based foundation for communicating results in our dashboard, showing both the **drivers of food inflation** and the **robustness of the dataset**.

---

### Analysis Techniques Used
## Data Analysis Techniques Used

- **Data Cleaning**
  - Checked and confirmed no missing values or duplicate rows.
  - Converted *'date'* column to datetime format and verified data types.
  - Created derived features (e.g., absolute drawdown values).

- **Univariate Analysis**
  - Summary statistics (mean, median, quartiles, skewness).
  - Histograms and boxplots to show distributions and outliers.
  - Ranking of countries by inflation (top/bottom performers).

- **Bivariate Analysis**
  - Correlation analysis between inflation and other numeric variables.
  - Scatter plots (inflation vs volatility, drawdown, and data coverage).
  - Highlighted extreme cases and outliers with country-level context.

- **Hypothesis Testing (Exploratory)**
  - H1: Compared inflation levels across crisis vs non-crisis countries (qualitative evidence).  
  - H2: Assessed relationship between inflation and volatility (scatter + regression trend).  
  - H3: Checked for bias by comparing inflation against data coverage (scatter).

- **Visualisation**
  - Bar charts (inflation by country, top/bottom 5 comparisons).
  - Scatter plots (with interactive Plotly for hover-based exploration).
  - Boxplots to illustrate skewness and outliers.

### Ethical Considerations
- Data coverage and accuracy vary by country, so results should be interpreted with caution.  
- Food inflation is closely linked to human well-being; presenting results without context risks oversimplifying human suffering.  
- Countries with limited statistical capacity may appear more volatile, introducing bias.  
- This analysis is exploratory and educational, not a policy tool, and findings should not be used in isolation to guide interventions.  

### Dashboard Design
The Power BI dashboard was designed to:  
- Provide **quick global insights** through KPIs (average inflation, top/bottom countries).  
- Allow **interactive exploration** with slicers (country, time).  
- Use **scatter plots and bar charts** to show relationships.  
- Apply a **consistent, high-contrast colour scheme** for readability.  
**Due to limitations with the version of PowerBI being used, a link cannot be provided, however, a file is available in the 'dashboard' folder labelled *food_analysis_dashboard*

The design balances clarity for non-technical users with depth for analysts.

### Unfixed Bugs


### Limitations


### Deployment
- Analysis performed in Jupyter Notebook (Python).  
- Dashboard created and deployed in **Power BI**.  
- Repository hosted on **GitHub** for transparency and reproducibility.  

### Main Data Analysis Libraries
- Python
- Pandas
- NumPy
- Seaborn
- Plotly
- MatPlotLib

### Credits
- **ChatGPT:** Supported with code guidance, data exploration ideas, markdown writing, and error troubleshooting  
- **GitHub Copilot:** Assisted with syntax and repetitive code blocks during Python scripting  
- **Kaggle:** - Dataset: [Monthly Food Price Estimates](https://www.kaggle.com/datasets/anshtanwar/monthly-food-price-estimates)  
- **Code Institute:** For the project structure and teamwork framework  
- **Team Members:** Harpreet, Aaminah and Richard
-   
### Acknowledgements
Thanks to:
* Code Institute for the project structure
* Kaggle for providing the dataset
* OpenAI for ChatGPT
* GitHub Copilot for coding support
* Code Institute peers for being supportive along the way
