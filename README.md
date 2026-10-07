# Neural Network
Neural network model for predicting graduate admission using one hidden layer with 1, 2, and 3 neurons.

## Overview
This project builds neural networks with varying architectures (one hidden layer with 1, 2, and 3 neurons) to predict graduate admission outcomes. The analysis explores how the number of hidden neurons affects prediction accuracy on normalized, structured admissions data.

## Dataset
- **Source:** Graduate Admission dataset
- **Key variables:** GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research Experience

## Methods
- Min-Max normalization of all numeric features
- 80/20 train-test split for model evaluation
- Neural networks with one hidden layer of 1, 2, and 3 neurons using the `neuralnet` package
- Model comparison across architectures

## Key Findings
- CGPA, GRE Score, and SOP were used as the three inputs; they are the top three predictors by MeanDecreaseGini in the Bagging model from the Tree_Based_Models project
- All features were min-max normalized before training
- Adding hidden neurons did not improve test accuracy: all three sizes reached the same test accuracy (0.875)
- On the same test set, the logistic model from the Classification_Model project still had the lowest misclassification error (0.1125), ahead of the neural networks (0.125), the decision tree and Bagging (0.1375), and Random Forest (0.15)

## Tools & Libraries
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=R&logoColor=white)
![neuralnet](https://img.shields.io/badge/neuralnet-276DC3?style=flat-square&logo=r&logoColor=white)
![caret](https://img.shields.io/badge/caret-276DC3?style=flat-square&logo=r&logoColor=white)

## How to Run
1. Clone the repository: `git clone https://github.com/BronsonBagwell/Neural_Network.git`
2. Open the HTML file in a browser, or run the R Markdown file in RStudio
3. Required packages: `neuralnet`, `caret`
