# World Wealth Data Analysis

This repository contains the **World Wealth Data Analysis** project, focusing on **Bridging the Wealth Disparity**. This project utilizes data engineering and machine learning techniques to analyze global wealth distribution.

## Abstract

The "Global Wealth Distribution Analysis" report delves into the uneven distribution of wealth among various countries and continents. By analyzing data from multiple sources, it uncovers significant disparities in how wealth is distributed globally. The insights provided are vital for comprehending economic imbalances and offer valuable guidance to both policymakers and academic researchers. This project aims to develop a predictive model for heart disease. Early prediction can significantly aid in timely diagnosis and intervention, potentially improving patient outcomes. We explore various machine learning algorithms, focusing on their accuracy and performance in classifying individuals at risk of heart disease. The project involves data exploration, preprocessing, model training, and evaluation. This brief overview highlights the importance of the study in informing discussions about achieving global economic fairness.

## Methodology

The project's methodology involved a comprehensive approach to data analysis:

1.  **Data Collection**: The World Bank collects and disseminates a wide range of data on various economic, social, and environmental indicators from countries around the world. The World Bank collaborates with other international organizations, such as the International Monetary Fund (IMF) and the United Nations (UN), to gather and validate data. Its Open Data Initiative aims to make this data freely available to the public.

2.  **Data Cleaning**: Redundant entries were removed, and missing or invalid values in the dataset were replaced with the mean or median. Numerical attributes initially assigned as objects were converted to numerical values, and new variables were created for analysis.

3.  **Exploratory Data Analysis (EDA)**: To gain a broad understanding of the dataset and identify potential research inquiries, exploratory data analysis was conducted. Scatter plots, histograms, and descriptive statistics were used to examine variable distributions and interrelationships.

4.  **Modeling**: Linear Regression and Random Forest Regressor models were employed to assess linearity and classification accuracy. Model precision was evaluated using root mean squared error and mean squared log error.

5.  **Visualization**: A range of visuals, including bar charts, heatmaps, and scatterplots, were created to illustrate the distribution, correlation, and connections among different variables, ensuring accessibility for diverse audiences.

6.  **Conclusion**: The analysis identified key factors influencing country economies, discussed the limitations and implications of the findings, and provided recommendations for future research.

## Key Findings & Project Highlights

The "Global Wealth Disparity Analysis" focused on mapping pronounced variations in wealth accumulation globally, offering insights into economic health and inequality.

  * **Top Countries with Highest GDP**: Luxembourg led with a significant margin, and France's GDP was 2.5 times the world average.
  * **Factors Affecting GDP**: Scatter plots visualized the correlation between GDP and various factors, shedding light on their nuanced relationships with economic performance.
  * **Model Visualization**: Scatter plots demonstrated that model predictions aligned commendably with actual data, indicating reliable performance.
  * **Total GDP Analysis**: The top 10 countries accounted for approximately two-thirds of the global GDP. A notable finding was the disparity between countries with high total GDP and those with high average GDP. China and India significantly increased their rank when considering total GDP compared to GDP per capita. The United States was the only country in the top 2 for both total and average GDP.
  * **Factors Affecting Total GDP**: Correlation analysis indicated that population and area were pivotal in influencing total GDP, consistent with their impact on GDP per capita.
  * **Economic Structure Comparison**: Scrutiny of the top 10 countries with the highest total GDP highlighted the significant impact of services and industry on their economies.
  * **Wealth Imbalance**: The research revealed an extreme imbalance in wealth distribution, both within nations and across continents, with a minimal number of countries holding the majority of global wealth.
  * **Policy and Historical Influences**: The study scrutinized the influence of political, social, and economic policies, as well as historical, geographical, and cultural elements, in shaping wealth distribution patterns.

The technical report was submitted on December 4, 2023.

## Files in this Repository

  * [`Countries_and_continents_of_the_world.csv`](https://www.google.com/search?q=rashrana/world-wealth-data-analysis/World-Wealth-Data-Analysis-789b6286c905cd76d307b7a23d7d0910d37ab82d/Countries_and_continents_of_the_world.csv): The dataset containing country and continent data, including various economic and geographical indicators.
  * [`Team 09 Technical Report.docx`](rashrana/world-wealth-data-analysis/World-Wealth-Data-Analysis-789b6286c905cd76d307b7a23d7d0910d37ab82d/Team 09 Technical Report.docx): The technical report in DOCX format.
  * [`Team 09 Technical Report.pdf`](rashrana/world-wealth-data-analysis/World-Wealth-Data-Analysis-789b6286c905cd76d307b7a23d7d0910d37ab82d/Team 09 Technical Report.pdf): The technical report in PDF format.
  * [`World-Wealth-Bridging.ipynb`](https://www.google.com/search?q=rashrana/world-wealth-data-analysis/World-Wealth-Data-Analysis-789b6286c905cd76d307b7a23d7d0910d37ab82d/World-Wealth-Bridging.ipynb): Jupyter Notebook containing the complete code for data loading, preprocessing, model training, and evaluation for world wealth analysis.

## How to Use

1.  **Clone the repository**:

    ```bash
    git clone https://github.com/rashrana/World-Wealth-Data-Analysis
    ```

2.  **Navigate to the project directory**:

    ```bash
    cd World-Wealth-Data-Analysis
    ```

3.  **Install dependencies**:
    Common dependencies for this type of project include `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`.

    ```bash
    pip install pandas numpy seaborn matplotlib scikit-learn
    ```

4.  **Run the Jupyter Notebook**:

    ```bash
    jupyter notebook "World-Wealth-Bridging.ipynb"
    ```

    This will open the notebook in your web browser, where you can execute the cells to reproduce the analysis and model training.

## Contributors

  * [Prashant Rana](https://www.google.com/search?q=https://github.com/rashrana)
  * Himagiri Bhavani Appisetty
  * Manne Dharanidhar
  * Anjalipriya Rajulagiri

## References

  * [Credit Suisse Global Wealth Report 2022](https://www.credit-suisse.com/about-us-news/en/articles/news-and-expertise/credit-suisse-global-wealth-report-2022-fast-wealth-growth-in-times-of-uncertainty-202209.html)
  * [UBS Global Wealth Report 2023](https://www.ubs.com/global/en/family-office-uhnw/reports/global-wealth-report-2023.html)
  * [Visual Capitalist: Distribution of Global Wealth Chart](https://www.visualcapitalist.com/distribution-of-global-wealth-chart/)
  * [Kaggle: World Data 2023](https://www.kaggle.com/code/uzmatabassum/world-data2023#-Task-of-Analysis-)
  * [Github Repository Link](https://github.com/rashrana/World-Wealth-Data-Analysis)
