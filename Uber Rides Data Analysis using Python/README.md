# Uber Rides Data Analysis using Python

This project analyzes Uber ride data using Python, focusing on data preprocessing, visualization, and extracting insights from ride patterns.

## Overview

The analysis covers:
- Data cleaning and preprocessing (handling nulls, date formatting, feature engineering)
- Exploratory data analysis (EDA) and visualization using Matplotlib and Seaborn
- Insights into ride purposes, categories, time-of-day, days of the week, months, and ride distances

## Steps Performed

1. **Import Libraries**  
   Utilizes `pandas`, `numpy`, `matplotlib`, and `seaborn` for data manipulation and visualization.

2. **Load Dataset**  
   Reads the Uber rides dataset from `UberDataset.csv`.

3. **Data Exploration**  
   - Checks dataset shape and info
   - Handles missing values in the `PURPOSE` column
   - Converts date columns to datetime format

4. **Feature Engineering**  
   - Extracts date and time features
   - Categorizes rides by time of day (Morning, Afternoon, Evening, Night)
   - Drops rows with nulls and duplicates

5. **Visualization**  
   - Count plots for ride categories and purposes
   - Time-of-day analysis
   - Correlation heatmap
   - Monthly and weekday ride trends
   - Distribution and boxplots for ride distances

6. **Encoding**  
   - Applies one-hot encoding to categorical columns

7. **Insights**  
   - Most rides are for business purposes
   - Peak ride times are afternoons
   - Most rides are short distances (0-20 miles)
   - Seasonal and weekly trends observed

## How to Run

1. Ensure you have Python 3.x installed.
2. Install required libraries:
   ```sh
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Place `UberDataset.csv` in the same directory as the notebook.
4. Open and run the notebook:  
   `Uber_Rides_Data_Analysis_using_Python.ipynb`

## File Structure

- [`Uber_Rides_Data_Analysis_using_Python.ipynb`](Uber_Rides_Data_Analysis_using_Python.ipynb): Main analysis notebook
- `UberDataset.csv`: Source dataset 

## Results
The notebook provides visual and statistical insights into Uber ride patterns, helping understand user behavior and trends.
