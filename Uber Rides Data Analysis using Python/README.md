## Iris Flower Classification
This project implements a machine learning solution for classifying iris flowers into species using the famous Iris dataset. The workflow includes data exploration, visualization, model building, evaluation, and user prediction.

## Features
Loads and explores the Iris dataset
Visualizes data using Seaborn pairplots
Splits data into training and testing sets
Trains a K-Nearest Neighbors (KNN) classifier
Evaluates model accuracy and provides a detailed classification report
Allows user input for real-time species prediction

## Requirements
Python 3.x
pandas
matplotlib
seaborn
scikit-learn

## Usage
Place ```IRIS.csv``` in the project directory.
Open and run the notebook Iris.ipynb cell by cell.
Follow the prompts for user testing to predict the species of a new iris flower.

## Project Structure
Iris.ipynb: Main Jupyter notebook containing all code and explanations.
IRIS.csv: Dataset file.

## How it works
The notebook loads and explores the dataset.
Data is visualized to understand feature relationships.
The dataset is split into training and testing sets.
A KNN classifier is trained and evaluated.
The user can input new flower measurements to predict the species.

## Example
```
Enter sepal_length : 5.1
Enter sepal_width : 3.5
Enter petal_length : 1.4
Enter petal_width : 0.2
species is  setosa
```

## License
This project is for educational purposes. The Iris dataset is  available in Kaggle.
