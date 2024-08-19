[![Codacy Badge](https://app.codacy.com/project/badge/Grade/4b4a1db8e2ed4b5bb4e7dbd94f3237f3)](https://app.codacy.com/gh/Abhinav330/911-Emergency-Calls-analysis/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/911-Emergency-Calls-analysis/matplotlib?color=red)
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/911-Emergency-Calls-analysis/numpy?color=green)   
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/911-Emergency-Calls-analysis/pandas?color=beige)  
![GitHub Pipenv locked dependency version](https://img.shields.io/github/pipenv/locked/dependency-version/Abhinav330/911-Emergency-Calls-analysis/seaborn?color=red)   
![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/Abhinav330/911-Emergency-Calls-analysis?color=dark%20green)
![GitHub repo size](https://img.shields.io/github/repo-size/Abhinav330/911-Emergency-Calls-analysis)

# Exploratory Data Analysis on 911 Dataset
Source : https://www.kaggle.com/datasets/mchirico/montcoalert?select=911.csv

# Code Summary

This Python script analyzes emergency call data from the '911.csv' dataset. It uses various data visualization techniques to explore and gain insights into the emergency call data, including the types of calls, reasons for calls, and call patterns over time.

## Data Loading and Exploration

The script starts by importing necessary libraries, including NumPy, Pandas, Matplotlib, Seaborn, and Plotly. It loads the '911.csv' dataset and explores its contents. Key steps in this section include:
- Checking the dataset information with `df.info()`.
- Creating a new column 'call_type' by extracting the call type from the 'title' column.
- Visualizing the distribution of call types using a bar plot.

## Call Types and Reasons

The script further analyzes the reasons for calls by:
- Extracting the actual reasons from the 'title' column and creating a new column 'Actual_reason'.
- Visualizing the most common reasons for calls using a bar plot.
- Converting the 'timeStamp' column to a datetime format.
- Extracting additional date and time-related columns, such as 'day,' 'month,' 'year,' and 'hour.'

## Temporal Analysis

The script performs temporal analysis of calls, including:
- Counting and visualizing call types by month using a count plot.
- Counting and visualizing call types by year using a count plot.
- Counting and visualizing call types by hour using a count plot.

## Location Analysis

The script explores the locations of calls by:
- Displaying the top 20 townships ('twp') with the highest call counts.
- Displaying the last 5 townships with the lowest call counts.
- Visualizing the top 100 townships with the highest call counts using a bar plot.
- Visualizing the last 10 townships with the lowest call counts using a bar plot.
- Exploring call locations by analyzing the 'addr' and 'twp' columns.

## Data Transformation

The script maps call types to numeric values by defining a function and applying it to the 'call_type' column. It then drops the unnecessary 'e' column.

## Correlation Analysis

The script calculates and visualizes the correlation between numeric columns in the dataset using a heatmap. This helps identify potential relationships between variables.

## Refrerences:
- Corral-De-Witt, D., Carrera, E., Muñoz-Romero, S. and Rojo-Álvarez, J. (2018). Statistical, Spatial and Temporal Mapping of 911 Emergencies in Ecuador. Applied Sciences, 8(2), p.199. doi:https://doi.org/10.3390/app8020199.
- Google Books. (2019). Advances in Emerging Trends and Technologies. [online] Available at: https://books.google.co.uk/books?hl=en&lr=&id=wdW1DwAAQBAJ&oi=fnd&pg=PA136&dq=911+emergency+dataset+analysis&ots=6lIcetO2I0&sig=zMa-eG9iBPggmz8CmT-nRomcRxA&redir_esc=y#v=onepage&q=911%20emergency%20dataset%20analysis&f=false [Accessed 18 Aug. 2024].

‌
