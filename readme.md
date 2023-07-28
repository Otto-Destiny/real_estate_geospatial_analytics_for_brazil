# Real Estate Geospatial Analytics For Brazil

![Brazil Real Estate](images/geospatial.jpg)

## Overview

This project aims to perform geospatial analytics on real estate data in Brazil. The dataset used in this analysis consists of information about properties available for rent in different regions of Brazil. The project utilizes Python and various data analysis libraries to clean, visualize, and analyze the data to gain insights into the real estate market.

## Dataset

The dataset used for this analysis is a combination of two CSV files:

1. `BR-properties-data-rent.csv`: This file contains real estate data for rental properties in Brazil.
2. `brasil-real-estate-2.csv`: This file provides additional real estate data for properties in Brazil.

## Project Structure

The project follows the following structure:

- `data/`: Contains the CSV files with real estate data(removed).
- `images/`: Stores images generated during the data visualization process.
- `Real_Estate_Geospatial_Analytics.ipynb`: Jupyter Notebook containing the Python code for the analysis.
- `README.md`: This README file providing project information and documentation.

## Setup and Dependencies

To run the project code, you will need the following Python libraries:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Scikit-learn

You can install these dependencies using `pip` by running:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

## Analysis Steps

The project's Jupyter Notebook, `Real_Estate_Geospatial_Analytics.ipynb`, performs the following steps:

1. Data Loading and Preprocessing:
   - Load data from the CSV files.
   - Drop rows with missing latitude and longitude values.
   - Split the `lat-lon` column into separate `lat` and `lon` columns.
   - Convert the `lat` and `lon` columns to float data type.
   - Calculate the price in USD for one of the datasets.
   - Drop unnecessary columns.

2. Data Visualization:
   - Plot properties on a scatter map to visualize their geospatial distribution.
   - Generate histograms to understand the distribution of home prices.
   - Build box plots to visualize the distribution of home sizes.
   - Create bar charts to display the mean home price by region.
   - Perform regression analysis with scatter plots and trend lines.

3. Region-Specific Analysis:
   - Subset the data for properties in the South region of Brazil.
   - Calculate summary statistics for properties in the South region.
   - Visualize correlations between property size and price for specific states in the South region.

## Results and Insights

Throughout the analysis, the following insights are obtained:

- The geospatial scatter map reveals the distribution of properties for rent across Brazil.
- The histogram of home prices shows the majority of properties have prices below a certain threshold.
- The box plot of home sizes illustrates the spread of property sizes, with some outliers.
- The bar chart of mean home prices by region provides insights into the regional variations in property prices.
- The regression analysis and trend lines demonstrate the relationship between property size and price for specific states in the South region.

## How to Run the Code

To reproduce the analysis, follow these steps:

1. Clone the repository to your local machine.

```bash
git clone <repository-url>
cd Real-Estate-Geospatial-Analytics-Brazil
```
2. Install the required dependencies.
```bash
Copy code
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```
or
```pip install -r requirements.txt
```

3. Open the Jupyter Notebook.
```bash
Copy code
jupyter notebook Real_Estate_Geospatial_Analytics.ipynb
```
4. Execute the code cells in the notebook to perform the analysis step-by-step.

## Contribution and Issues
Contributions to this project are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## Acknowledgments
The dataset used in this project is sourced from real-estate-data on Kaggle. Special thanks to Kaggle and the data contributors for providing the data.

## License
This project is licensed under the MIT License.