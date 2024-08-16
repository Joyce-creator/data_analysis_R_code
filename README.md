# Data Analysis and Performance Metrics

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
   -  Modify the line in the script where `data` is loaded to match your file path. For example, `data <- read.csv("C:\\Users\\coron\\OneDrive\\Desktop\\data_analysis\\output_table.csv")`.
   -  Please ensure that your input file is correctly formatted. The first column should be named "YearMonth," and the second column should be named "NetReturn". Please delete any additional rows that may have been added, as sometimes extra information is provided unintentionally. Additionally, ensure the accuracy of the data extracted, as there might be instances where YTD data is included incorrectly or the order of data may be disrupted.

2. **User Input**:
   - The script includes a function to prompt the user to input benchmark data manually. Enter the data when prompted, typing `done` when you finish entering values.Please ensure that the number of rows in your benchmark data matches exactly with the number of rows in the input file. Avoid pressing Enter or adding whitespace, as these will be treated as data entries.

3. **Calculations**:
   - The script calculates several financial metrics including:
     - Upside Capture
     - Downside Capture
     - PnL (Profit and Loss)
     - Drawdown
     - Year-to-Date (YTD) Returns
     - Monthly Return Distribution
     - Various performance metrics like Sharpe Ratio, Correlation, Beta, and more.

4. **Visualizations**:
   - The script generates plots to visualize:
     - PnL changes over time using `plotly`.
     - Monthly Return Distribution using `ggplot2`.

5. **Export Results**:
   - All the calculated data, including the performance metrics and visualizations, are saved to an Excel file named `combined_data_and_plots.xlsx`.
  
## Outputs

- **`combined_data_and_plots.xlsx`**: The main output file containing:
  - Performance metrics
  - YTD data
  - Monthly return distribution summary
  - Raw data
  - Embedded images of the generated plots

- **`plot_PnLchange.html`**: An HTML file containing the interactive PnL change plot.

- **`monthly_return_plot.png`** and **`plot_PnLchange.png`**: Images of the generated plots.

## Additional Information

- **PhantomJS**: The script uses `webshot` to capture the interactive plot as an image, which requires `PhantomJS`. The script will install `PhantomJS` automatically if not present.

- **Customization**: You can customize the input file, metrics, and plots by modifying the script.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
