# Programming Language Popularity Trends Analysis (2004-2024)

## Abstract
This analysis explores programming language popularity trends from 2004 to 2024, using a Kaggle dataset. Through data cleaning, time series analysis, and visualization, we identify growth and decline patterns among programming languages, offering insights for developers, organizations, and educators.

## Introduction
The popularity of programming languages reflects technology industry trends, guiding decisions in project selection, skill development, and tech stack choices. Understanding these trends can highlight emerging technologies and shifts in developer preferences. Our dataset includes annual popularity metrics for various languages, providing a basis for long-term trend analysis and insights into programming language lifecycle.

## Dataset
The dataset, compiled by Muhammad Khalid on Kaggle, documents annual popularity metrics for various programming languages from 2004 to 2024. Key fields include:
- **Year**: Time of each popularity record
- **Language**: Programming language name
- **Popularity**: Popularity metric (e.g., ranking or score)

This format enables time-series analysis to study shifts and trends in programming language usage.

## Methodology

1. **Data Preparation**:  
   Libraries used:
   - `pandas` for data manipulation
   - `numpy` for numerical operations
   - `matplotlib` and `seaborn` for visualization  
   The dataset was loaded, cleaned, and prepared for analysis.

2. **Visualization and Trend Analysis**:
   - **Line Chart**: Shows long-term popularity trends of the top 10 languages.
   - **Yearly Comparisons**: Bar charts for the most popular languages in 2004 and the latest year, illustrating shifts in popularity.

3. **Advanced Analysis**:
   - **Correlation Heatmap**: Examines correlations in language popularity trends, identifying languages with similar trajectories.
   - **Volatility Analysis**: Standard deviation chart reveals stability or fluctuation in popularity.
   - **Stacked Area Chart**: Displays relative popularity over time, normalized by year.
   - **PCA**: Reduces dimensionality to reveal relationships and clusters among languages with similar trends.

## Repository Structure


