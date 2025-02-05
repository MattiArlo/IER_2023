# IER_2023
This is the GitHub repository for the ME41125 Introduction to Engineering Research course for 2023

# Original Dataset

The step data used in this analysis is taken from an open access source. The Excel file "distances.xlsx" is taken directly from this source. For any further reference please refer to the orignial data set here: Alex van den Berg, Bart de Vries, Zoe Breedveld, Annelouk van Mierlo,Marnix Tijuis, \& Laura Marchal-Crespo. (2023). Embodiment of virtual feet correlates with motor performance in a target-stepping task: A pilot study (1.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.7927391.


# Step Height Variability Analysis

This repository contains a data analysis of step height variability in different avatar representations. The analysis is performed using Python 3.7 and data from an Excel file. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

## Prerequisites

- Python 3.7 or higher. If not, you can download it from [Python's official website](https://www.python.org/downloads/).
- Libraries: pandas, numpy, matplotlib, seaborn, scipy, statsmodels
- Recommended: Jupyter notebook (or a python IDE such as Pycharm or Spyder)

You can install the libraries using pip:
``` pip install pandas numpy matplotlib seaborn scipy statsmodels ``` 


## Installing

1. Clone the repository:
git clone https://github.com/MattiArlo/IER_2023.git

2. Navigate to the directory of the cloned repository in your terminal: cd /path/to/directory

## Running the Analysis

### Method 1

Once you're in the correct directory, run the Python script using the python command followed by the script name:
```python data_analysis_python.py```
If you encounter a "Permission Denied" error, you might need to modify the file permissions to make the script executable. On Unix systems, you can use the chmod command:
```chmod +x data_analysis_python.py```

### Method 2

1. Open the Jupyter notebook `data_analysis.ipynb` in your local development environment.
2. If the Excel file 'distances.xlsx' is not in the same folder as the notebook, adjust the path in the line that reads the Excel file:
```pythondf = pd.read_excel('data/distances.xlsx', sheet_name='Stepheight_corrected') ```
3. Run all cells in the Jupyter notebook to reproduce the analysis.

### Method 3
If you don't have Jupyter notebook installed, you can also run the analysis on any python IDE (e.g. Pycharm) using a Python script.
1. Download the python script: data_analysis_python.py
2. Download the data folder with the distances.xlsx file
3. Open the python file in an IDE environement and run the file from there. 

## Description of the Analysis

The analysis first separates the data according to the avatar representation condition, computes variance for each condition, and then creates a boxplot and histograms for each condition. Finally, it conducts a one-way ANOVA to compare the means of the three groups. If the ANOVA is significant, it further performs a Tukey's HSD post-hoc test.

## Results
Results include printed variance values, a boxplot visualization, histograms, and ANOVA results. If ANOVA is significant, the results of Tukey's HSD post-hoc test are also included.

## Authors

Matti Lang
