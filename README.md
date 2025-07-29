# World Wealth Data Analysis: Bridging the Wealth Disparity

## Executive Summary

The "Global Wealth Distribution Analysis" project investigates the uneven distribution of wealth across various countries and continents. By analyzing extensive data from multiple sources, it uncovers significant disparities in global wealth allocation. The insights derived from this study are crucial for understanding economic imbalances and offer valuable guidance for policymakers and academic researchers alike. This report emphasizes the study's importance in contributing to discussions on achieving global economic fairness.

## 1. Introduction

The objective of this study is to meticulously examine the distribution of wealth on a global scale. Leveraging comprehensive datasets that encompass economic, demographic, and geographical dimensions, the analysis aims to unveil the intricate variations and inequities in wealth among different nations and regions. This project also reviews existing scholarly work on worldwide wealth distribution, highlighting significant research and perspectives that contribute to the understanding of economic inequalities between various nations and regions.

## 2. Highlights of Project

The "Global Wealth Disparity Analysis" initiative deeply focused on mapping pronounced variations in wealth accumulation worldwide, offering an insightful view into the disparate states of global economic health and inequality. Key highlights include:

* **Comprehensive Comparative Study:** The project involved a thorough comparison of economic statuses across a wide range of countries and continents, moving beyond total wealth to delve into distribution dynamics within these regions. This provided essential insights into varying levels of economic inequality and overall prosperity.
* **Detailed Methodology:** The research employed a comprehensive and exacting methodology, involving detailed gathering and analysis of wide-ranging datasets (including economic metrics, demographics, and geographical aspects). Advanced statistical techniques and visual representation tools were utilized for effective data interpretation, crucial for uncovering trends, anomalies, and significant patterns in global wealth distribution.
* **Enlightening Outcomes:** A notable finding was the extreme imbalance in wealth distribution, evident both within individual nations and across continents. The analysis revealed a disproportionate concentration of global wealth in a minimal number of countries, with many other areas significantly lagging in economic prosperity. This discrepancy underscores the irregularities in economic development and its wider implications for global economic stability and growth.
* **Driving Factors:** The study explored factors contributing to economic disparities, scrutinizing the influence of political, social, and economic policies on wealth distribution patterns. It also highlighted the role of historical, geographical, and cultural elements in shaping economic conditions.

## 3. Methodology

The approach to gathering and analyzing the data involved several methodical steps:

### 3.1. Data Collection

The primary data was sourced from the World Bank, an organization that collects and disseminates a wide range of economic, social, and environmental indicators from countries globally. The World Bank collaborates with other international bodies like the International Monetary Fund (IMF) and the United Nations (UN) to ensure data validation. Access to this data was facilitated through the World Bank's Open Data Initiative.

### 3.2. Data Cleaning and Preparation

* **Handling Missing Values:** Redundant entries were removed, and missing or invalid values in the dataset were imputed using either the mean or median, grouped by `Region`. If any missing values remained after regional imputation, they were filled with the overall mean of their respective columns.
* **Data Type Conversion:** Attributes that were initially numerical but assigned as objects were converted to numerical values to ensure suitability for analysis.
* **Feature Selection and Renaming:** A subset of relevant columns was selected for the analysis. Columns like 'Country Name' and 'climate' were renamed to 'Country' and 'Climate' for consistency.
* **Feature Engineering:** A new variable, `Total_GDP ($)`, was created by multiplying `GDP ($ per capita)` and `Population`. This allowed for an analysis of the absolute economic output of countries.
* **Categorical Encoding:** Categorical features such as `Region` and `Climate` were label encoded to prepare them for machine learning models.

### 3.3. Exploratory Data Analysis (EDA)

EDA was conducted to gain a broad understanding of the dataset and identify potential research questions. This involved:

* **Descriptive Statistics:** Calculation of descriptive statistics for all variables to summarize their distribution.
* **Bar Plots:** Visualization of the top countries with the highest GDP per capita, revealing Luxembourg as a frontrunner and notable differences compared to the world mean.
* **Heatmaps:** Generation of a heatmap to visualize the correlation between all numerical variables, providing insights into their interrelationships.
* **Scatter Plots:** Creation of scatter plots to visualize the correlation between GDP per capita and six highly correlated features (e.g., Phones (per 1000), Birthrate, Infant mortality (per 1000 births), Service, Literacy (%), Net migration), shedding light on nuanced relationships affecting economic performance.
* **Total GDP Analysis:** Analysis of `Total_GDP ($)` to identify the top 10 countries contributing approximately two-thirds of the global GDP. A comparison highlighted the disparity between countries with high total GDP versus those with high average GDP, with China and India showing significant jumps in rank when considering total GDP.

### 3.4. Modeling

To assess the linearity and classification accuracy of the data, two regression models were employed:

* **Linear Regression:** A basic linear model was applied, and its performance was evaluated using Root Mean Squared Error (RMSE) and Mean Squared Log Error (MSLE).
* **Random Forest Regressor:** Recognizing non-linear relationships in the data, a Random Forest Regressor was used. This ensemble model with `n_estimators=50`, `max_depth=6`, `min_weight_fraction_leaf=0.05`, and `max_features=0.8` demonstrated improved performance compared to linear regression.

### 3.5. Model Visualization

Scatter plots were utilized to visually assess the predictive performance of the models. These visualizations showed a commendable alignment between model predictions and actual data, indicating reasonable and reliable model performance, with data points generally clustering around the y=x line.

## 4. Key Findings

* **Top GDP Countries:** Luxembourg leads significantly in GDP per capita, with other nations showing catch-up trends. France's GDP was notably 2.5 times greater than the world average.
* **Total GDP Insights:** The top 10 countries contribute about two-thirds of the global GDP, highlighting a disparity between countries with high total GDP and those with high average GDP. China and India, in particular, show a significant rise in rank when considering total GDP due to their large populations.
* **Factors Affecting GDP:** Population and area were identified as pivotal factors influencing total GDP, aligning with factors affecting GDP per capita. Correlation analysis revealed relationships between GDP and features like phone penetration, literacy rates, and sector contributions (Agriculture, Industry, Service).
* **Low Birthrate & Low GDP Countries:** Countries with low birth rates (<14%) and low GDP per capita (<$10,000) often exhibit high literacy rates, a lesser reliance on services, limited phone penetration, and negative net migration. These countries are predominantly found in Eastern Europe or the Commonwealth of Independent States (C.W. of IND. STATES), making `Region` a crucial differentiating factor.
* **Economic Structure:** The economic structures of the top 10 countries by total GDP underscore the significant impact of services and industry on their economies, offering valuable insights into diverse economic landscapes.

## 5. Conclusion

This analysis encapsulates key discoveries concerning worldwide wealth distribution, underscoring pronounced disparities. The insights gained are vital for grasping global economic inequalities. Moving forward, future studies are recommended to delve deeper into advanced modeling techniques and consider additional variables. Furthermore, an exploration of specific economic policies that contribute to observed patterns could provide a more comprehensive understanding of the dynamics at play, aiding in the development of more equitable economic strategies and measures.

## 6. Repository Structure
├── World-Wealth-Bridging.ipynb  # Jupyter Notebook containing the data analysis code
├── Countries_and_continents_of_the_world.csv # Dataset used for the analysis
├── Team 09 Technical Report.docx  # Technical report in DOCX format
└── Team 09 Technical Report.pdf   # Technical report in PDF format

Here is a detailed README file for your GitHub repository, incorporating information from all the provided files:

```markdown
# World Wealth Data Analysis: Bridging the Wealth Disparity

## Executive Summary

The "Global Wealth Distribution Analysis" project investigates the uneven distribution of wealth across various countries and continents. By analyzing extensive data from multiple sources, it uncovers significant disparities in global wealth allocation. The insights derived from this study are crucial for understanding economic imbalances and offer valuable guidance for policymakers and academic researchers alike. This report emphasizes the study's importance in contributing to discussions on achieving global economic fairness.

## 1. Introduction

The objective of this study is to meticulously examine the distribution of wealth on a global scale. Leveraging comprehensive datasets that encompass economic, demographic, and geographical dimensions, the analysis aims to unveil the intricate variations and inequities in wealth among different nations and regions. This project also reviews existing scholarly work on worldwide wealth distribution, highlighting significant research and perspectives that contribute to the understanding of economic inequalities between various nations and regions.

## 2. Highlights of Project

The "Global Wealth Disparity Analysis" initiative deeply focused on mapping pronounced variations in wealth accumulation worldwide, offering an insightful view into the disparate states of global economic health and inequality. Key highlights include:

* **Comprehensive Comparative Study:** The project involved a thorough comparison of economic statuses across a wide range of countries and continents, moving beyond total wealth to delve into distribution dynamics within these regions. This provided essential insights into varying levels of economic inequality and overall prosperity.
* **Detailed Methodology:** The research employed a comprehensive and exacting methodology, involving detailed gathering and analysis of wide-ranging datasets (including economic metrics, demographics, and geographical aspects). Advanced statistical techniques and visual representation tools were utilized for effective data interpretation, crucial for uncovering trends, anomalies, and significant patterns in global wealth distribution.
* **Enlightening Outcomes:** A notable finding was the extreme imbalance in wealth distribution, evident both within individual nations and across continents. The analysis revealed a disproportionate concentration of global wealth in a minimal number of countries, with many other areas significantly lagging in economic prosperity. This discrepancy underscores the irregularities in economic development and its wider implications for global economic stability and growth.
* **Driving Factors:** The study explored factors contributing to economic disparities, scrutinizing the influence of political, social, and economic policies on wealth distribution patterns. It also highlighted the role of historical, geographical, and cultural elements in shaping economic conditions.

## 3. Methodology

The approach to gathering and analyzing the data involved several methodical steps:

### 3.1. Data Collection

The primary data was sourced from the World Bank, an organization that collects and disseminates a wide range of economic, social, and environmental indicators from countries globally. The World Bank collaborates with other international bodies like the International Monetary Fund (IMF) and the United Nations (UN) to ensure data validation. Access to this data was facilitated through the World Bank's Open Data Initiative.

### 3.2. Data Cleaning and Preparation

* **Handling Missing Values:** Redundant entries were removed, and missing or invalid values in the dataset were imputed using either the mean or median, grouped by `Region`. If any missing values remained after regional imputation, they were filled with the overall mean of their respective columns.
* **Data Type Conversion:** Attributes that were initially numerical but assigned as objects were converted to numerical values to ensure suitability for analysis.
* **Feature Selection and Renaming:** A subset of relevant columns was selected for the analysis. Columns like 'Country Name' and 'climate' were renamed to 'Country' and 'Climate' for consistency.
* **Feature Engineering:** A new variable, `Total_GDP ($)`, was created by multiplying `GDP ($ per capita)` and `Population`. This allowed for an analysis of the absolute economic output of countries.
* **Categorical Encoding:** Categorical features such as `Region` and `Climate` were label encoded to prepare them for machine learning models.

### 3.3. Exploratory Data Analysis (EDA)

EDA was conducted to gain a broad understanding of the dataset and identify potential research questions. This involved:

* **Descriptive Statistics:** Calculation of descriptive statistics for all variables to summarize their distribution.
* **Bar Plots:** Visualization of the top countries with the highest GDP per capita, revealing Luxembourg as a frontrunner and notable differences compared to the world mean.
* **Heatmaps:** Generation of a heatmap to visualize the correlation between all numerical variables, providing insights into their interrelationships.
* **Scatter Plots:** Creation of scatter plots to visualize the correlation between GDP per capita and six highly correlated features (e.g., Phones (per 1000), Birthrate, Infant mortality (per 1000 births), Service, Literacy (%), Net migration), shedding light on nuanced relationships affecting economic performance.
* **Total GDP Analysis:** Analysis of `Total_GDP ($)` to identify the top 10 countries contributing approximately two-thirds of the global GDP. A comparison highlighted the disparity between countries with high total GDP versus those with high average GDP, with China and India showing significant jumps in rank when considering total GDP.

### 3.4. Modeling

To assess the linearity and classification accuracy of the data, two regression models were employed:

* **Linear Regression:** A basic linear model was applied, and its performance was evaluated using Root Mean Squared Error (RMSE) and Mean Squared Log Error (MSLE).
* **Random Forest Regressor:** Recognizing non-linear relationships in the data, a Random Forest Regressor was used. This ensemble model with `n_estimators=50`, `max_depth=6`, `min_weight_fraction_leaf=0.05`, and `max_features=0.8` demonstrated improved performance compared to linear regression.

### 3.5. Model Visualization

Scatter plots were utilized to visually assess the predictive performance of the models. These visualizations showed a commendable alignment between model predictions and actual data, indicating reasonable and reliable model performance, with data points generally clustering around the y=x line.

## 4. Key Findings

* **Top GDP Countries:** Luxembourg leads significantly in GDP per capita, with other nations showing catch-up trends. France's GDP was notably 2.5 times greater than the world average.
* **Total GDP Insights:** The top 10 countries contribute about two-thirds of the global GDP, highlighting a disparity between countries with high total GDP and those with high average GDP. China and India, in particular, show a significant rise in rank when considering total GDP due to their large populations.
* **Factors Affecting GDP:** Population and area were identified as pivotal factors influencing total GDP, aligning with factors affecting GDP per capita. Correlation analysis revealed relationships between GDP and features like phone penetration, literacy rates, and sector contributions (Agriculture, Industry, Service).
* **Low Birthrate & Low GDP Countries:** Countries with low birth rates (<14%) and low GDP per capita (<$10,000) often exhibit high literacy rates, a lesser reliance on services, limited phone penetration, and negative net migration. These countries are predominantly found in Eastern Europe or the Commonwealth of Independent States (C.W. of IND. STATES), making `Region` a crucial differentiating factor.
* **Economic Structure:** The economic structures of the top 10 countries by total GDP underscore the significant impact of services and industry on their economies, offering valuable insights into diverse economic landscapes.

## 5. Conclusion

This analysis encapsulates key discoveries concerning worldwide wealth distribution, underscoring pronounced disparities. The insights gained are vital for grasping global economic inequalities. Moving forward, future studies are recommended to delve deeper into advanced modeling techniques and consider additional variables. Furthermore, an exploration of specific economic policies that contribute to observed patterns could provide a more comprehensive understanding of the dynamics at play, aiding in the development of more equitable economic strategies and measures.

## 6. Repository Structure

```

.
├── World-Wealth-Bridging.ipynb  \# Jupyter Notebook containing the data analysis code
├── Countries\_and\_continents\_of\_the\_world.csv \# Dataset used for the analysis
├── Team 09 Technical Report.docx  \# Technical report in DOCX format
└── Team 09 Technical Report.pdf   \# Technical report in PDF format

````

## 7. How to Run the Project

To set up and run this project, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/rashrana/World-Wealth-Data-Analysis.git](https://github.com/rashrana/World-Wealth-Data-Analysis.git)
    cd World-Wealth-Data-Analysis
    ```

2.  **Set up a Python environment:**
    It is recommended to use a virtual environment.
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: `venv\Scripts\activate`
    ```

3.  **Install dependencies:**
    The project relies on standard Python data science libraries. You can install them using pip:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

4.  **Run the Jupyter Notebook:**
    Launch Jupyter Notebook from the project root directory:
    ```bash
    jupyter notebook
    ```
    Once Jupyter opens in your browser, navigate to and open `World-Wealth-Bridging.ipynb`. You can then run all cells to execute the data analysis and visualize the results.

## 8. Team Members

* Prashant Rana
* Himagiri Bhavani Appisetty
* Manne Dharanidhar
* Anjalipriya Rajulagiri

## 9. Contributions & References

This project was developed as part of the Distributed and Scalable Data Engineering (DSCI-6007) course in Fall 2023 at the University of New Haven.

The data and research were informed by the following sources:

* [Credit Suisse Global Wealth Report 2022](https://www.credit-suisse.com/about-us-news/en/articles/news-and-expertise/credit-suisse-global-wealth-report-2022-fast-wealth-growth-in-times-of-uncertainty-202209.html)
* [UBS Global Wealth Report 2023](https://www.ubs.com/global/en/family-office-uhnw/reports/global-wealth-report-2023.html)
* [Visual Capitalist: Distribution of Global Wealth Chart](https://www.visualcapitalist.com/distribution-of-global-wealth-chart/)
* [Kaggle: World Data 2023 - Task of Analysis](https://www.kaggle.com/code/uzmatabassum/world-data2023#-Task-of-Analysis-)
````
