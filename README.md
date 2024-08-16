# Data Analysis and Performance Metrics Calculation

This repository contains an R script that performs data analysis and calculates various performance metrics for a given dataset. The script also generates visualizations and exports the results to an Excel file.

## Prerequisites

The script requires the following R packages. If they are not installed, the script will install them automatically:
- `readr`
- `readxl`
- `ggplot2`
- `plotly`
- `dplyr`
- `lubridate`
- `openxlsx`
- `htmlwidgets`
- `webshot`

- Make sure you have a working internet connection for the packages to be installed.

## How to Use

1. **Load the CSV File**: 
   -  Modify the line in the script where `data` is loaded to match your file path. For example, data <- read.csv("C:\\Users\\coron\\OneDrive\\Desktop\\data_analysis\\output_table.csv")

2. **User Input**:
   - The script includes a function to prompt the user to input benchmark data manually. Enter the data when prompted, typing `done` when you finish entering values.
