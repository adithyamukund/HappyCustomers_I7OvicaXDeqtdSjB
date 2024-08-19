# Customer Satisfaction Prediction for Food Delivery Service

This project is designed to help a food delivery company improve customer satisfaction by analyzing survey responses. The company conducts a survey with six questions, each rated on a scale from 1 to 5 (where a higher number indicates a more positive response). Additionally, customers indicate whether they are happy with the service by responding with a simple yes or no.

## Project Overview

The goals of this project are:

1. Predict whether a customer is happy with the service based on their responses to the survey questions.
2. Identify which of the six survey questions are the best predictors of customer happiness, allowing the company to focus on the most impactful areas for improvement.

## Data Description

- 126 rows (126 customers responded to survey).
- 6 columns (one column per question, one column for satisfaction response)
- About 50% of the customer base is dissatisfied with the service.

## Business Impact

1. App Improvement: The findings will suggest ways to enhance the app to convert unhappy customers into happy ones.
2. Survey Optimization: By identifying the most important questions, the company can reduce the length of the survey, making it easier to distribute and collect at scale.

## Methodology

- Evaluate various machine learning classifiers to determine which model best predicts customer happiness based on their survey responses.
- Measure model performance with precision, because incorrectly predicting a happy customer is dangerous, while incorrectly predicting an unhappy customer is inconvenient.
- The selected model inputs the most important survey question responses for a single customer and outputs a prediction of whether that customer is happy.

## Installation

To run the notebook, simply clone the repository and open it with your preferred notebook editor (VSCode recommended).

## Conclusion

- GradientBoostingClassifier(min_samples_leaf=2, min_samples_split=10) is the best model because the median precision is high, and the standard deviation of the precision is low.
- These two questions give the most information about a customer's happiness, and should be of utmost importance to the company to improve current customer experience. Also, the company should simplify the survey to these two questions to scale its distribution:
    - Was my order delivered on time?
    - Did the app make ordering easy for me?
