# Data-Driven Market Analysis and Recommendation System for Strategic Decision Support

## Project Overview

This project was developed as part of my Master's thesis titled:

**Data-Driven Market Analysis and Visualization for Supporting Strategic Decisions**

This thesis shows a data-driven analytical framework designed to support strategic decision-making by integrating data management, statistical analysis, visualization, and predictive modeling. The case study that used is video game market to explain how market data can be transformed to practical managerial insights.

The main objective of the study was building a framework to help decision-makers to better understand market structure, identify sales patterns, evaluate influential factors, and assess potential market opportunities.

Overall, this thesis shows that combining database design, statistical analysis, machine learning, dashboard visualization, and a recommendation system can produce a practical analytical framework to support strategic decision-making.

## Project Objective

This thesis primarily aims to design and implement a data-driven analytical framework for evaluating market performance and supporting strategic decision-making through data analysis, visualization, and forecasting.

In addition, the thesis aims to demonstrate how historical market data can be transformed into supportive management insights and indicators by combining data preparation, exploratory analysis, data visualization in a dashboard, and the use of predictive modelling.

## Specific Objectives

- Collecting, cleaning, and systematically preparing market sales data suitable for statistical analysis, analytical processing, and forecasting.
- Analysing the key characteristics of the selected market in the case study and identifying significant relationships between variables.
- Studying market trends and demand variations to identify patterns relevant to strategic decision-making that supports managers.
- Presenting the results of the analyses through dashboards that provide a clear visual overview of the market structure, performance indicators, and significant variations.
- Utilizing and comparing forecasting models and transforming the forecast outputs into a recommendation system that supports managers in evaluating hypothetical market opportunities, identifying promising market segments, and improving product planning decisions.

## Dataset

The case study utilizes the **Video Game Sales with Reviews** dataset, which combines sales data with review-related variables.

The video game market was used as a case study due to its wealth of important data and indicators, such as global and regional sales figures, as well as game-related characteristics like release year, game type, and the platforms on which the games were published. Critic and user reviews were also included, allowing for an analysis of the impact of game characteristics and their evaluation on the global and regional markets.

The main analytical sample was taken from **2000 to 2016** to focus on the most recent structure of the video game market based on the available dataset.

## Methodology

This thesis employs a data-driven analytical framework to support strategic decision-making, using video game sales data as a case study. The systematic design integrates database organization, proactive data processing, descriptive and inferential statistics, predictive modeling, and data visualization in a dashboard. A recommendation layer is also integrated into a comprehensive workflow.

The first phase of the methodology focused on data structuring and preparation. MySQL was used to create a relational database to store and organize the data from the case study dataset prior to analysis.

In the second phase, the selected data was cleaned and prepared using Python and libraries such as NumPy and Pandas. This included removing duplicate data, addressing missing or inconsistent values, converting certain variables to formats different from their defaults to prepare them for various analytical processes, and limiting the sample used in applying the framework to the period between 2000 and 2016.

In the third stage, statistical inference was employed. Analysis of variance (ANOVA) was used to compare means across more than two groups, such as different types or platform groups. The chi-squared test for independence was used to examine relationships between categorical variables. In addition to hypothesis testing, regression analysis was used to examine the relationship between the selected explanatory variables and sales results.

Predictive modeling was then applied, and several machine learning techniques were compared: Random Forest, Neural Network, and CatBoost. The aim of this comparison was to identify the model that achieved the best predictive performance for sales estimation.

The CatBoost model was ultimately selected, as it was particularly well-suited to this study due to the dataset containing numerous categorical variables.

Following the model evaluation process, the final CatBoost model was integrated into a recommendation system that combines sales forecasts, market demand, competition, publisher market control position, and regional sales patterns to support strategic management decision-making.

In the final stage, data visualization was implemented using Microsoft Power BI. Dashboards were designed to display key analytical findings related to sales distribution, market trends, regional variations, and publisher performance.

## Tools and Technologies

- Python
- Pandas
- NumPy
- SciPy
- Statsmodels
- Scikit-learn
- CatBoost
- MySQL
- SQL
- Power BI
- Matplotlib
- Seaborn
- Jupyter Notebook

## Main Project Stages

### 1. Data Management and Database Design

A relational database was created using MySQL to organize the gaming market data in a more structured way. The database's purpose was to store and prepare the data prior to the analytical, conceptual, and predictive phases of this study.

### 2. Data Preprocessing and Cleaning

The data was cleaned, filtered, and prepared for analysis. The main analytical sample was taken from 2000 to 2016 to focus on the most recent structure of the video game market.

The preprocessing stage included:
- Duplicate record detection
- Handling missing values
- Temporal filtering of the dataset
- Removal of inconsistent records
- Dataset preparation for analytical modeling

### 3. Descriptive and Exploratory Analysis

Descriptive analysis was made to summarize the information taken from the dataset and to provide the initial understanding of the market composition in terms of genre, platform groups, sales distribution, and review indicators.

The exploratory analysis included:
- Distribution of games by genre
- Distribution of games by platform
- Temporal distribution of game releases
- Correlation analysis

### 4. Statistical Analysis

The inferential analytical stage used several statistical methods to examine whether differences and relationships in the data were statistically meaningful.

The statistical methods included:
- ANOVA
- Chi-square test
- Regression analysis

### 5. Predictive Modeling

Several machine learning models were implemented and compared in the predictive stage:

- Random Forest
- Neural Network
- CatBoost

CatBoost was selected because it has strong suitability for the dataset, and also because of its ability to handle categorical variables.

The final CatBoost model achieved an R² of approximately **0.60–0.62** on the test set.

### 6. Recommendation System

The recommendation system was built based on the final CatBoost model.

This system was designed as a hybrid decision-support tool that combines predicted sales with market indicators such as market demand, competition intensity, publisher position, and regional sales patterns.

The predictive outputs were transformed into more practical strategic recommendations through this process, including identifying concepts, estimating risk, evaluating opportunity, and suggesting target regions.

### 7. Dashboard Visualization

Microsoft Power BI was used to develop dashboards that present the main market in a visual way.

These dashboards provided interactive views of:
- Sales trends
- Regional performance
- Genre distribution
- Platform evolution
- Publisher presence
- Relationship between reviews and sales

The dashboard layer complemented the analytical and predictive stage by making the results easier to interpret from a managerial perspective.

## Project Structure

```text
data-driven-market-analysis-recommendation-system/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── market_analysis_recommendation_system.ipynb
│
├── data/
│   └── Video_Games_Sales_as_at_22_Dec_2016.csv
│
├── sql/
│   └── database_schema.sql
│
├── dashboards/
│   └── dashboard screenshots
│
└── reports/
    └── thesis_project_summary.pdf
```

## How to Run the Project

1. Clone or download this repository.

2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Place the dataset inside the `data/` folder.

4. Open the notebook:

```text
notebooks/market_analysis_recommendation_system.ipynb
```

5. Run the notebook step by step.

## Dataset Note

The dataset used in this project is the **Video Game Sales with Reviews** dataset from Kaggle. The dataset is licensed under **CC0: Public Domain**, so it is included in this repository for reproducibility.

The dataset file is located in the `data/` folder:

`data/Video_Games_Sales_as_at_22_Dec_2016.csv`

## Business Value

The findings suggest that such a framework can help managers to better understand historical market behavior and also evaluate hypothetical future opportunities in a more structured and evidence-based way.

The project demonstrates how market data can be transformed into structured insights that support strategic decision-making through data cleaning, statistical analysis, predictive modeling, dashboard visualization, and recommendation mechanisms.

## Author

**Wajd Saeid**  
Master's student in Economics and Management  
Bachelor's Degree in Computer Engineering and Automatic Control