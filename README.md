# IER_2023
This is the GitHub repository for the ME41125 Introduction to Engineering Research course for 2023
# Step Height Variability Analysis

This repository contains a data analysis of step height variability in different avatar representations. The analysis is performed using a Jupyter notebook and data from an Excel file. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

- Python 3.7 or higher
- Jupyter notebook (or a python IDE)
- Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels

You can install the libraries using pip:
``` pip install pandas numpy matplotlib seaborn scipy statsmodels ``` 


### Installing

1. Clone the repository:
git clone https://github.com/MattiArlo/IER_2023.git

2. Navigate to the directory of the cloned repository in your terminal.

### Running the Analysis

1. Open the Jupyter notebook `data_analysis.ipynb` in your local development environment.
2. If the Excel file 'distances.xlsx' is not in the same folder as the notebook, adjust the path in the line that reads the Excel file:
```pythondf = pd.read_excel('data/distances.xlsx', sheet_name='Stepheight_corrected') ```

Run all cells in the Jupyter notebook to reproduce the analysis.

### Using Python Script
If you don't have Jupyter notebook installed, you can also run the analysis on any python IDE (e.g. Pycharm) using a Python script.
Convert the Jupyter notebook data_analysis.ipynb to a Python script. You can do this in Jupyter notebook by clicking on File > Download as > Python (.py). 

### Description of the Analysis

The analysis first separates the data according to the avatar representation condition, computes variance for each condition, and then creates a boxplot and histograms for each condition. Finally, it conducts a one-way ANOVA to compare the means of the three groups. If the ANOVA is significant, it further performs a Tukey's HSD post-hoc test.

### Results
Results include printed variance values, a boxplot visualization, histograms, and ANOVA results. If ANOVA is significant, the results of Tukey's HSD post-hoc test are also included.

### Authors

Matti Lang
