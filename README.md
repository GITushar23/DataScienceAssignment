# Forest Fire Data Analysis and Prediction

This repository contains an exploratory data analysis (EDA) of a dataset related to forest fires, with the goal of understanding the key factors contributing to fire size and intensity. The project includes data cleaning, visualization, and preliminary modeling insights.

## Table of Contents

- [Overview](#overview)
- [Data Source](#data-source)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Repository Structure](#repository-structure)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project performs EDA on a forest fire dataset, aiming to identify patterns and correlations between various environmental and locational attributes and the resulting burned area. The analysis includes assessing distributions of individual variables, examining relationships between variables, and uncovering patterns using visual techniques.

## Data Source

The dataset used in this analysis is stored in `forestfires.csv`. It includes attributes such as coordinates (X, Y), month, day of the week, and various meteorological indices (FFMC, DMC, DC, ISI, temp, RH, wind, rain), alongside the burned area.

## Data Cleaning

The data cleaning process involved:

*   **Missing Value Handling:** Verifying and documenting any missing values in the dataset.
*   **Duplicate Removal:** Eliminating duplicate records to ensure the accuracy of subsequent analyses.
*   **Categorical Standardization:** Standardizing the categorical features (`month` and `day`) by converting all values to lowercase and stripping whitespace, ensuring consistency.
*   **Outlier Management:** Using the Interquartile Range (IQR) method to cap extreme values in numerical columns.

## Exploratory Data Analysis (EDA)

The EDA included:

*   **Univariate Analysis:**  Examining individual variables using histograms, frequency distributions, and descriptive statistics.
*   **Bivariate Analysis:** Analyzing relationships between two variables at a time using correlation matrices, scatter plots, bar plots, and violin plots.
*   **Multivariate Analysis:** Assessing the combined effects of several factors, such as the combined impact of month and day on the average burned area.

## Repository Structure

```
└──forest-fire-analysis/
   ├── forestfires.csv        # Raw dataset
   ├── 23321032.ipynb # Jupyter Notebook with code for data cleaning and EDA
└── README.md             
```

## Dependencies

The following Python libraries are required:

*   pandas
*   numpy
*   matplotlib
*   seaborn

You can install these using pip:

```bash
pip install pandas numpy matplotlib seaborn
```

## Usage

1.  Clone this repository:

   ```bash
   git clone https://github.com/GITushar23/DataScienceAssignment.git
   cd forest-fire-analysis
   ```

2.  Install the dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3.  Open and execute `23321032.ipynb` in Jupyter Notebook or JupyterLab.

## Contributing

Contributions are welcome! If you find issues or have improvements, please submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

