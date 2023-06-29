# Amazon Customer Reviews Rating Prediction using Naive Bayes

This repository contains an implementation of a Naive Bayes classifier to predict the rating of a review based on its text.

## Project Overview

We have a dataset of customer reviews for different products on Amazon, each associated with a rating ranging from 1 to 5. The goal is to build a Naive Bayes classifier to predict the rating of a review based on the text of the review. 

This classifier works by first analyzing the training data, which includes reviews and their corresponding ratings. It calculates the prior probability of each rating occurring in the dataset and the likelihood of observing each word in the reviews given a specific rating. It then uses this information to predict the rating of new reviews.

## Files Description

- `AMAZON_FASHION.json.gz`: Dataset containing Amazon customer reviews.
- `naive_bayes_classifier.ipynb`: Jupyter Notebook file containing the code for the project.

## Implementation Details

The implementation involves several steps:

1. Loading and cleaning the dataset
2. Performing exploratory data analysis
3. Vectorizing the text data
4. Training the Naive Bayes model
5. Making predictions on the test set
6. Evaluating the model

## Evaluation Metrics

We evaluate the model using precision, recall, and F1 score with the `average='weighted'` parameter. The weighted average considers the number of samples in each class and calculates a weighted average, giving more weight to classes with a larger number of samples.

## Visualization

The project also includes visualizations such as the distribution of ratings and the Receiver Operating Characteristic (ROC) curve for each class.

## Libraries Used

- pandas
- gzip
- sklearn
- matplotlib
- numpy
- transformers
- torch

## Usage

To use this project, first clone the repository. Then open and run the Jupyter Notebook `naive_bayes_classifier.ipynb`.

## Future Enhancements

Future enhancements to this project could include tuning the parameters of the Naive Bayes classifier or trying different types of classifiers to compare their performance.

## Author

<Mina Mehdinia>

## License

This project is open source, under the MIT License.

