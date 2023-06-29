# Amazon Reviews Rating Prediction

## Introduction

This project involves the development of a Naive Bayes classifier for predicting the rating of a product on Amazon based on the text of a customer's review. The rating range is from 1 to 5, and the goal is to accurately predict this rating using the words and phrases in the review text.

## Methodology

The Naive Bayes classifier begins by analyzing training data which consists of reviews and their corresponding ratings. It calculates the prior probability of each rating occurring in the dataset. For example, it determines the likelihood of a rating being between 1 and 5 based on the proportions of these ratings in the training data.

In addition, the classifier calculates the likelihood of observing each word in the reviews given a specific rating. For example, it determines the probability of seeing the word "great" in a review with a rating of 5.

The classifier uses the test data to predict the ratings. It calculates the probability of the review belonging to each rating category based on the words and phrases present in the review. It does this by multiplying the prior probability of each rating with the likelihood of observing the words in the review given that rating. Finally, it assigns the review to the rating category with the highest probability.

When calculating the precision, recall, and F1 score, the 'weighted' parameter is used. This considers the number of samples in each class, and calculates a weighted average of precision and recall, giving more weight to classes with a larger number of samples. This means that classes with more samples will have a greater impact on the overall performance metric.

## Installation

1. Clone this repository
2. Install the required packages (Python 3.x, pandas, sklearn, matplotlib)
3. Download the dataset and place it in the `data/` folder

## Usage

Open the `main.ipynb` file in Jupyter Notebook to see the steps taken to implement the Naive Bayes classifier and interpret the results.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Figures

Here are some figures from our analysis:

![Figure 1](figures/figure1.png)
![Figure 2](figures/figure2.png)

## License

This project is open source, under the MIT License.

