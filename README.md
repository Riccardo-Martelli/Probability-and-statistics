# Billionaires Net Worth Analysis

## Overview
This project presents a detailed analysis of the net worth of billionaires in the years 1996, 2001, and 2014. The study aims to explore whether the Pareto distribution, a well-known model for wealth inequality, holds true among the wealthiest individuals. The analysis includes both qualitative and quantitative assessments of wealth distribution, including the use of the Kolmogorov-Smirnov test, modified Pareto distribution, and the Gini coefficient. 

The hypothesis being tested is whether the distribution of wealth among billionaires follows the same Pareto principle observed in general populations, and if this distribution increases or decreases over time.

## Project Structure
- **Data Analysis**: The code analyzes the net worth of billionaires for the years 1996, 2001, and 2014 using various distributions.
- **Pareto Distribution Verification**: Verifying the validity of the Pareto distribution using statistical tests like the Kolmogorov-Smirnov test.
- **Wealth Inequality Analysis**: Uses the Lorenz curve and Gini coefficient to quantitatively measure wealth inequality.
- **Visualization**: Graphs and charts to visually represent the distribution of wealth.

## Libraries Used
The following libraries are utilized for data analysis, statistical modeling, and visualization:

- **pandas**: Data manipulation and analysis.
- **numpy**: Numerical computing.
- **scipy**: Scientific and technical computing (including statistical tests and curve fitting).
- **seaborn**: Statistical data visualization.
- **matplotlib**: Plotting and visualization.
- **sklearn**: Preprocessing for data scaling.
- **networkx**: Network analysis (optional, depending on your exploration).
- **openpyxl**: Excel file handling (for reading/writing `.xlsx` files).

## Key Concepts & Methodology
### 1. **Wealth Distribution and the Pareto Principle**
Wealth is defined as the total value of an individual’s assets minus their liabilities. The Pareto principle suggests that 80% of wealth is controlled by 20% of the population. This observation led to the development of the Pareto distribution, which is an inverse power law used to describe the distribution of wealth.

In this project, we explore whether billionaires follow the same Pareto distribution. The analysis includes:
- Fitting different distributions (Pareto, Exponential, and Modified Pareto) to the data.
- Conducting a Kolmogorov-Smirnov test to validate the best-fitting distribution.
  
### 2. **Statistical Testing**
The distribution fitting is followed by statistical tests. A p-value table summarizes the results of tests performed on the distributions:

| Year  | 1996 | 2001 | 2014 |
|-------|------|------|------|
| **Exponential p-value** | 1.067e-05 | 5.554e-20 | 5.073e-50 |
| **Pareto p-value** | 0.00065 | 0.00025 | 0.00069 |
| **Modified Pareto p-value** | 0.086 | 0.145 | 0.056 |

From this, the null hypothesis for the Exponential and Pareto distributions is rejected (p-value < α), while the Modified Pareto distribution fits well with p > α.

### 3. **Wealth Inequality Analysis**
- **Lorenz Curve**: The Lorenz curve visually demonstrates wealth inequality. A perfectly equal distribution results in a straight line, while an uneven distribution will form a concave curve.
- **Gini Coefficient**: The Gini coefficient quantifies wealth inequality. A value of 1 represents maximum inequality (one individual owns all wealth), while 0 represents complete equality.

### 4. **Conclusions**
From the analysis, it is evident that the wealth distribution among billionaires does not perfectly follow the classic Pareto distribution but aligns well with a modified version. The inequality in wealth distribution increases over time, and while there is growth in the number of billionaires, the overall wealth inequality also seems to increase.

It would be valuable to extend this research to individual countries and other wealth subgroups to check for patterns of inequality on a more granular level.

## Requirements
Ensure you have the following dependencies installed:

- Python 3.x
- pandas
- numpy
- scipy
- seaborn
- matplotlib
- sklearn
- networkx
- openpyxl

To install them, run:

```bash
pip install pandas numpy scipy seaborn matplotlib scikit-learn networkx openpyxl
```
## How to Run the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/Riccardo-Martelli/Probability-and-statistics.git
   ```
- Navigate to the project folder:

  ```bash
  cd billionaires-net-worth-analysis
  ```
- Open the Jupyter Notebook:

  ```bash
  jupyter notebook
  ```
- Open `Esame_17_02_Riccardo_Martelli.ipynb` to explore the full analysis and data visualizations.
## Dataset

This project uses publicly available data on the net worth of billionaires across three years: 1996, 2001, and 2014. More details on the dataset can be found in the notebook.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contributing

Feel free to fork this repository and contribute by submitting a pull request. For significant changes, please open an issue first to discuss the proposed changes.

## Acknowledgments

- Thanks to the data sources used for the project.
- Thanks to the open-source community for their contributions to data analysis and visualization tools.
