# Programming Language Popularity Trends Analysis (2004-2024)

## Abstract
This analysis aims to explore the popularity trends of programming languages between 2004 and 2024, revealing shifts in language usage within the technology sector. The dataset, sourced from Kaggle, contains annual popularity metrics for various programming languages. Through data cleaning, time series analysis, and visualization, we analyze each language's performance over time to identify trends and stages in technology development. Key findings indicate significant growth in certain languages and a decline in legacy languages, providing valuable insights for developers and organizations in technology selection and future planning.

## Introduction
Programming language popularity reflects the technology industry's evolution, highlighting changing trends in tools and technology preferences among developers, businesses, and educational institutions. As the technology landscape advances, language preferences show cyclical patterns influenced by application domains. For instance, Python’s rise is driven by data science and machine learning applications, while JavaScript remains dominant in front-end development. Analyzing these trends offers insights into emerging technologies and informs decisions on project selection, talent development, and technology stack updates.

The dataset, spanning 2004-2024, records annual popularity changes for multiple programming languages, enabling a long-term trend study. By examining trends, declines, and domain-specific migrations in language use, we gain insights into the lifecycle and market needs of programming languages.

## Dataset
The dataset used in this analysis was sourced from Kaggle, compiled by data author Muhammad Khalid. It documents annual popularity rankings for various programming languages, allowing for a detailed analysis of long-term trends. Key attributes in the dataset include:
- **Year**: The year of each record, covering data from 2004 to 2024.
- **Programming Language**: The name of the programming language, covering a broad range of languages used across diverse technology fields.
- **Popularity**: The yearly popularity metric, often expressed as a ranking or score.

The dataset's tabular format facilitates time-series analysis, enabling us to explore trends, fluctuations, and shifts in language popularity among the developer community. This structure also simplifies data cleaning, formatting, and visualization, supporting multidimensional EDA (Exploratory Data Analysis).

## Literature Review

### Programming Language Popularity Trends
Tools like the TIOBE Index and RedMonk rankings provide annual or quarterly insights into programming language popularity but lack the granularity to capture monthly changes. This dataset, covering 2004-2024, includes monthly data, offering a unique opportunity to analyze both short-term and long-term trends.

### The Use of Time Series Analysis
Hyndman and Athanasopoulos (2018) in *Forecasting: Principles and Practice* emphasize time series analysis for identifying trends and fluctuations. In this study, time series methods decompose changes in language popularity, helping identify technology shifts and changes in developer interests.

### The Driving Role of Industry Demand
Studies indicate that language popularity often correlates with specific application domains—Python’s popularity in data science and JavaScript’s dominance in front-end development. This analysis explores these trends across different fields, revealing the demand-driven forces shaping language usage.

## Architecture/Methodology

### 1. Data Preparation and Library Imports
The analysis was conducted in Google Colab. The initial step involved uploading the dataset and importing essential libraries:
- **pandas**: For data loading, cleaning, and processing.
- **numpy**: For numerical calculations and array operations.
- **matplotlib.pyplot**: For basic chart generation.
- **seaborn**: For enhanced visualizations.

The dataset was loaded with `pd.read_csv()` and verified using `data.head()` to ensure data integrity.

### 2. Initial Visualization of Data Trends
The first visualization was a line chart showing the popularity trends of each programming language over time. To improve readability, we focused on the most recent data and identified the top ten most popular languages, creating a refined line chart for these languages.

### 3. Data Processing Steps
- **Date Conversion**: The `Date` column was converted to a standardized datetime format ("Year-Month-Day") for accurate time series analysis.
- **Selection of Top Languages**: We extracted the top ten languages based on the latest year’s data.
- **Revised Trend Chart**: The line chart for these top languages allowed for clearer trend analysis.

### 4. Comparison of Language Popularity in Specific Years
We created bar charts comparing the popularity of the top ten languages in the latest available year and 2004, highlighting how popularity has evolved. Font size and angle adjustments ensured clarity.

### 5. In-depth Data Analysis
With an initial understanding of the dataset, we conducted more advanced analyses to uncover relationships and patterns.

- **Heat Map for Correlation Analysis**: We generated a heat map to examine correlations between language popularity trends, identifying languages with similar trends.
- **Standard Deviation Analysis**: A standard deviation chart revealed the stability of each language's popularity, indicating which languages experienced significant fluctuations.

### 6. Advanced Analysis: Relative Popularity and Principal Component Analysis (PCA)
Further analyses provided insights into the competitive landscape and relative positioning of languages.

- **Dynamic Stacked Area Chart**: This chart visualized each language’s relative popularity as a proportion of total industry usage over time, effectively displaying each language’s “market share.”
- **PCA Visualization**: PCA was used to reduce dimensionality and reveal relationships between languages. By clustering languages with similar popularity trends, we identified languages with unique or overlapping usage trajectories.

## Repository Structure

