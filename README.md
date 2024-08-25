# R-code-for-dissertation
Overview
This project focuses on analyzing environmental data from Linfen and other cities in China, with a particular emphasis on air quality metrics such as PM2.5, SO2, and NO2 levels. The goal is to assess how these pollutants impact public health, examine the influence of socio-economic factors, and explore the role of urban planning in environmental justice. The results of this analysis aim to provide valuable insights into the distribution of pollution across different socio-economic groups and the overall effectiveness of air quality policies.

Project Structure
The project is organized into several key directories and files. The data/ directory contains the datasets used in the analysis, including the main xcy.csv file, which holds daily air quality readings. The scripts/ directory houses all R scripts necessary for loading, cleaning, analyzing, and visualizing the data. Specifically, you will find load_data.R for loading the data, data_cleaning.R for preparing the data, analysis.R for performing statistical analysis, and visualization.R for generating plots. The results of these analyses, including visualizations and summary tables, are saved in the output/ directory. This README file provides instructions and information about the project, and there is also a .RData file included, which contains saved R environment objects such as data frames and models used in the analysis.

Prerequisites
To run the R scripts in this project, you need to have R and RStudio installed on your machine. Additionally, several R packages must be installed to ensure the code runs smoothly. These include dplyr, ggplot2, tidyr, readr, lubridate, and broom. You can install these packages by running the following command in your R console:
install.packages(c("dplyr", "ggplot2", "tidyr", "readr", "lubridate", "broom"))

Data Description
The primary data used in this project consists of air quality measurements and socio-economic indicators for various cities in China. The dataset includes variables such as the date of observation, the city where measurements were taken, and concentrations of pollutants like PM2.5, SO2, and NO2. Additional variables include the daily average temperature, population density, and average health literacy levels in the population. This data is critical for understanding the spatial distribution of pollution and its correlation with socio-economic factors.

Loading Data
To begin working with the data, you should run the load_data.R script located in the scripts/ directory. This script loads the xcy.csv file as well as any objects saved in the .RData file into the R environment. Make sure that your working directory is set to the root of the project before executing this script to avoid any path-related issues.

Data Cleaning
Once the data is loaded, the next step is to clean it by running the data_cleaning.R script. This script is designed to handle missing values, remove outliers, and correct any inconsistencies in the dataset. The cleaned dataset will be saved as cleaned_data.csv in the output/ directory, ready for analysis.

Statistical Analysis
The core analysis of this project is conducted in the analysis.R script. This script performs various statistical analyses, including regression modeling to explore the relationship between air quality and socio-economic factors such as population density, income levels, and health literacy. The results of these analyses provide insights into how these factors influence pollution levels and public health outcomes. Summary statistics and model results will be saved in the output/ directory, allowing for further inspection and interpretation.

Visualization
Visualizing the data is crucial for interpreting the results and communicating findings effectively. The visualization.R script generates a series of plots, including time series of PM2.5 levels across different cities, scatter plots illustrating the relationship between air quality and socio-economic variables, and bar charts comparing pollution levels between cities. These visualizations are automatically saved as PNG files in the output/ directory.

Expected Output
After running the analysis and visualization scripts, you should expect several outputs, including the cleaned dataset (output/cleaned_data.csv), a regression model summary (output/model_summary.txt), and a variety of visualizations (e.g., pm25_trend.png, pollution_vs_income.png). These outputs collectively provide a comprehensive view of the environmental data and the factors affecting air quality in the studied cities.
