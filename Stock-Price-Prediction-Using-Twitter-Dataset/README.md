# Stock Price Prediction Using Twitter Dataset

This project predicts stock prices using sentiment analysis of tweets and machine learning models. It uses a GUI built with Tkinter to allow users to upload a dataset, preprocess tweets, split data, train models, and visualize results.

## Features

- Upload and preview a Twitter stock dataset
- Preprocess tweets using spacy and vadersentiment analysis
- Split data into training and testing sets
- Train and evaluate SVM and Random Forest regression models
- Visualize predictions and compare RMSE errors

## Project Structure


- `StockPricePrediction.py`: Main Python GUI application
- `Dataset/tweets_dataset.csv`: Sample dataset of tweets and stock prices
- `model/data.csv`: Preprocessed data (generated after preprocessing)
- `run.bat`: Batch file to run the application

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib
- spacy (`en_core_web_sm` model)
- vaderSentiment
- tkinter

## Install dependencies with:

```sh
pip install pandas numpy scikit-learn matplotlib spacy vaderSentiment
python -m spacy download en_core_web_sm
```

## Usage

1. Place your dataset in the Dataset/ folder as tweets_dataset.csv.
2. Run the application:
python ```StockPricePrediction.py```
Or double-click ```run.bat```.
3. Use the GUI to:
  -Upload the dataset
  -Preprocess tweets
  -Split data
  -Train models (SVM, Random Forest)
  -View prediction results and RMSE comparison

## Notes
The application uses only the first 600 rows of the dataset for demonstration.
Preprocessing uses spaCy for NLP and VADER for sentiment scoring.
Results are displayed in the GUI and as plots.

## License
This project is for educational purposes.
